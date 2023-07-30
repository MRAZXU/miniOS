openocd -f jlink.cfg -f raspi4.cfg

$ telnet localhost 4444
> halt
> load_image ./benos.bin 0x80000
> step 0x80000

gdb-multiarch --tui benos