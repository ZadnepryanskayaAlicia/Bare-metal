pull_core:
	aria2c --file-allocation=none -c -x 10 -s 10 https://github.com/limitedeternity/qemu-bootloader/releases/download/v1.0.0/Core.iso

run:
	qemu-system-i386 -m 256M -rtc base=localtime -drive file=main.bin,index=0,media=disk,format=raw -drive file=fat:rw:data/,index=2,format=raw -s

clean:
	rm -f *.o
	rm -f *.bin
	rm -f *.elf
