include foo.mk

vpath %.h ../headers ../other-directory

some_binary: ../headers blah.h
	touch some_binary

../headers:
	mkdir ../headers

blah.h:
	touch ../headers/blah.h

clean:
	rm -rf ../headers
	rm -f some_binary

all:
	echo $(tag)
	echo This line is too long, so \
		it is broken up into multiple lines

