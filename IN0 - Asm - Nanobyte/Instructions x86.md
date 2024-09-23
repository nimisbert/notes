Convertis en code machine pour être exécuté par le CPU.
### HLT
Stop l'exécution du CPU. Peut être relancer par interruption.
```asm
main:
	hlt
```
### JMP
Saute vers une zone mémoire du code.
```
.halt:
	jmp .halt
```


