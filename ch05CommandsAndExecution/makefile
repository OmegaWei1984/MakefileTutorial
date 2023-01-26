SHELL=/bin/bash

new_contents = "hello:\n\ttouch inside_file \$$(cooly)"

cooly = "The subdirectory can see me!"

export cooly

all:
	@echo "This make line will not be printed"
	echo "But this will"
	cd ..
	echo `pwd`
	mkdir -p subdir
	printf $(new_contents) | sed -e 's/^ //' > subdir/makefile
	cd subdir && cat makefile
	cd subdir && $(MAKE)

clean:
	rm -rf subdir

