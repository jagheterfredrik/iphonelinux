all:	AndroidPNG.h AndroidSelectedPNG.h BackgroundPNG.h ConsolePNG.h ConsoleSelectedPNG.h iPhoneOSPNG.h iPhoneOSSelectedPNG.h

bin2c:	bin2c.c
	$(CC) bin2c.c -o $@

%PNG.h:	%.png bin2c
	./bin2c data$*PNG < $< > $@

clean:
	-rm *.o
	-rm bin2c
	-rm *.h
