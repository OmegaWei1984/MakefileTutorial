print: $(wildcard *.o)
	ls -la $?

things := $(wildcard *.o)
	
hey: one two
	echo $@
	echo $?
	echo $^

one:
	touch one

two:
	touch two

clean:
	rm one two

