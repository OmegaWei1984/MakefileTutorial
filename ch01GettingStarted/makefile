hello:
	echo "hello, makefile"

blah: blah.o
	cc blah.o -o blah

blah.o: blah.c
	cc -c blah.c -o blah.o 

blah.c:
	echo "int main() { return 0; }" > blah.c

some_file: other_file
	touch some_file

other_file:
	# nothing

files = file1 file2

some_file2: $(files)
	echo "files is " $(file)
	touch some_file2

file1:
	touch file1

file2:
	touch file2

clean:
	rm -f $(files) some_file2

x = dude
dude:
		echo $(x)
		echo ${x}

