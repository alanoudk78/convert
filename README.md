# convert
example convert by MIPS

.data
inum1: .word 42
fnum: .float 0.0


.text
lw $t0,inum1
mtc1 $t0,$f6
cvt.s.w $f8,$f6

li $v0,10
syscall
