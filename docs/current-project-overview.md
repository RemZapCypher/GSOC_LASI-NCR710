# This is an Executive Summary of the current project progress report.

- Okay So for the 82596 only the RX and TX datastructure is left.

For the NCR710
--------------
- Fix Endiness issue and make it uninversal
- Revert and compare the changes
- Make fifo into Queue
		- Same for the scsi fifo
		- Adjust the drain functions
		- Adapt the scripts according to the todo hooks





- [FIX ME] In the initial stage we hade the LE and be conversion issue for the ncr710 read. So the issue was something like the 0x0004(0384) <- This is the garbage value ie 
the set/get was having an issue not anything else.
- [STEPS] Check if FIFO is issue and implement a FUCKING QUEUE and not a STACK [ME IDIOT].
- [STEPS] Put changes in patch
- [STEPS] INTERRUPT MASKING ISSUE is their some kind.
- [STEPS] Adapt scripts JUMP instead of JWT or something.

