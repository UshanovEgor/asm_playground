; Simple example
; Writes Hello World to the output

JMP start
hello: DB "Hello World!" ; Variable


start:
MOV C, hello ; Point to var
MOV D, 232 ; Point to output
CALL print


print: ; print(C:*from, D:*to)
PUSH A
PUSH B
MOV B, 0
.loop:
MOV A, [C] ; Get char from var
MOV [D], 1 ; Write to output
INC C
INC D
CMP B, [C] ; Check if end
JNZ .loop ; jump if not

POP B
POP A
RET
