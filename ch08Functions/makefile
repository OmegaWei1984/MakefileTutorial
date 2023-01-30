bar := ${subst not, totally, "I am not superman"}

comma := ,
empty := 
space := $(empty) $(empty)
abc := a b c
abc_comma := $(subst $(space), $(comma), $(abc))

objects := a.o b.o c.o

test1 := $(patsubst %.o,%.c,$(objects))
test2 := $(objects:%.o=%.c)
test3 := $(objects:.o=.c)

sentence := who are you
sentence2 := $(foreach word,$(sentence),$(word)!)

test4 := $(if this-is-not-empty,then!,else!)
test5 := $(if $(empty),then!,else!)

test_function = Variable Name: $(0) First: $(1) Second: $(2) Empty Variable: $(3)

all:
	echo $(bar)
	echo $(abc_comma)
	echo $(test1)
	echo $(test2)
	echo $(test3)
	echo $(sentence2)
	echo $(test4)
	echo $(test5)
	echo $(call test_function, go, tigers)
	echo $(shell ls -la)

