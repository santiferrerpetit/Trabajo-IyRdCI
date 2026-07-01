# 1. ADD
## Descripción
Sumar los contenidos de dos registros y guardar el resultado en un tercer registro
## Instrucctions:
> ADD r1, r2, r3
## Precondiciones: 
Setear los registros que quiero sumar con sus valores arbitrarios
> set pc 0 s r2 1 s r3 2
## Code
- Opcode : 00000
- rs : 00010
- rt : 00011
- rd : 00001
- aux : 00000
- funct : 011100 


Binario: 0000 0000 1000 0110 0001 0000 0001 1100

Hexa:    0     0     8     6     1     0     1     C

> s [0x0] 0x0086101C 00000 opcode 00010 $2 00011 $3 00001 $1 000000 aux funct 011100

## Postcondiciones: 
- r1 = 0x00000000
- r2 = 0x00000001
- r3 = 0x00000002

1 + 2 = 3 = 0x00000003

## Conclusiones:

La operacion funciona, suma efectivamente a r2 con r3 y lo guarda en r1
