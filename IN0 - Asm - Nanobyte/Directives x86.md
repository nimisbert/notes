Donne à l'assembleur des informations d'interprétations du code.
### ORG
Indique à l'assembleur que l'on souhaite chargé le code dans une adresse en mémoire RAM.
```asm
org 0x7C00
```
### BITS
Indique à l'assembleur de générer du code pour un système 16-bits.
```asm
bits 16
```
### DB
Déclare un octet ou groupe d'octet constant.
```x86_64
db 0
```
### DW 
Déclare un word (2 octets)
```asm
dw 0AA55h
```
### TIMES
Répète une zone mémoire (octets ou instructions) un certains nombre de fois.
```asm
times 510-($-$$) db 0
```
### $ 
Offset en mémoire courante du segment.
### $\$
Offset en mémoire du début de segment.
```asm
($-$$)
```
Donne la taille du programme en octets. En soustrayant l'offset de l'instruction à l'offset de début du segment.