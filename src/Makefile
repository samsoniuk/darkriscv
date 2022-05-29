APPLICATION = darksocv


default: all


all:
	make -C $(APPLICATION) all

ifdef HARVARD
	cp -a $(APPLICATION)/*.rom.mem ./darksocv.rom.mem
	cp -a $(APPLICATION)/*.ram.mem ./darksocv.ram.mem
else
	cp -a $(APPLICATION)/*.mem ./darksocv.mem
endif

clean:
	make -C darksocv clean
	make -C coremark clean
	rm -r *.mem