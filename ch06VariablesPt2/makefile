one = one ${later_variable}
two := two ${later_variable}

later_variable = later

three = hello

three := ${three} world

four = hello four
four ?= will not be set
five ?= will be set

nullstring =
space = $(nullstring) 

str := $(three)
str += "!"

override opt_one = did_override
opt_two = not_override

foo = export blah="I was set"; echo $$blah

define bar
export blsh=set
echo $$blah
endef

all: not_other = cool

%.c: cfile = "%.c"

foo.c:
	echo $(cfile)

all:
	echo $(one)
	echo $(two)
	echo $(three)
	echo $(four)
	echo $(five)
	echo "=="$(space)"==>"
	echo $(str)
	# make opt_one=test opt_two=test2
	echo $(opt_one)
	echo $(opt_two)
	$(foo)
	$(bar)
	echo $(not_other)

other:
	echo $(not_other)
	echo $(cfile)

