myprog: myprog.c libmylib.a
	gcc myprog.c -L. -lmylib -o myprog

show.o:	show.c mylib.h
	gcc -c show.c -o show.o

sum.o: sum.c mylib.h
	gcc -c sum.c -o sum.o

libmylib.a:	show.o sum.o
	ar rs libmylib.a sum.o show.o

clean:
	rm sum.o show.o myprog
