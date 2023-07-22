There were errors in the mtvec_handler

unnecessary branch statement was removed

there was no increment in the exeption occured address
an increment of 8 was introduced as it is mentioned .align 8
 addi t1, t1, 8

there was no updates in the cause address (mpec)
a statement was introduced to update the address
 csrw mepc, t1

 After correcting this It worked properly