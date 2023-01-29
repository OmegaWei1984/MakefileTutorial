foo = ok

nullstring=
space = $(nullstring) 

bar = 
baz = $(bar)

all:
ifeq ($(foo), ok)
	echo "is ok"
else
	echo "nope"
endif

ifeq ($(strip $(space)),)
	echo "space is empty after being stripped"
endif
ifeq ($(nullstring),)
	echo "nullstring doesn't even have spaces"
endif
ifdef baz
	echo "baz is defined"
endif
ifdef bar
	echo "but bar is not"
endif
ifneq (,$(findstring i, $(MAKEFLAGS)))
	echo "i was passed to MAKEFLAGS"
endif

