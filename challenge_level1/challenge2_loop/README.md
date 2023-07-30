The issue was of infinite loop 
The logic of statements in the loop was wrong

Inroduced new set of commands
loop:
	lw t1, (t0)
  lw t2, 4(t0)
  lw t3, 8(t0)
  add t4, t1, t2
  addi t0, t0, 12
  beq t0, t6, out
  j pass
  beq t3, t4, loop        # check if sum is correct
  j fail
out:

after using this command the BUG was resolved
![Alt text](image.png)