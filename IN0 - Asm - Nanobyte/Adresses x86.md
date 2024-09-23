Les zones mémoires en x86 sont adressées par deux mots de 16-bits. Un mot pour le segment et un mot pour l'offset. Tel que, les adresses réelles sont accessibles par l'équation suivante:
$$
Address = Segment \times 16 + Offset
$$
Un exemple avec l'adresse du premiers secteur de boot:
$$
\begin{align}
0000_h:7C00_h \quad&|\quad 7C00_h = 0000_h \times 16 + 7C00_h \\
0001_h:7BF0_h \quad&|\quad 7C00_h = 0001_h \times 16 + 7BF0_h \\
\end{align}
$$
Avec la connaissances des [[Registres x86]], l'accès à une zone mémoire en assembleur se fait avec une instructions du type:
$$
segment:[base + index \times scale + displacement]
$$
Tel que:
- $segment$: CS, DS, ES, FS, GS, SS, DS si non spécifié
- $base$: BP, BX (16-bits), ou tout autre registre général (32/64-bits)
- $index$: SI, DI (16-bits), ou tout autre registre général (32/64-bits)
- $scale$: en mode 32/64-bits, uniquement (1, 2, 4, 8)
- $displacement$: un entier signé constant

Exemples:
```asm
var: dw 100       ; delcare var 16-bit contant equal to 100d
...
	mov ax, var   ; copy var offset to ax
	mov ax, [var] ; copy var to DS
```

```asm 
array: dw 100, 200, 300
...
	mov bx, array     ; copy offset of array to bx
	mov si, 2 * 2     ; array[2], 0-index 2-bytes wide addressing
	mov bx, [bx + si] ; copy memory contents
```