main: main.o fifo.o rr.o sjf.o psjf_2.o util.o
	gcc -o $@ $^

main.o: main.c
	gcc -c main.c

fifo.o: fifo.c
	gcc -g -c fifo.c

rr.o: rr.c
	gcc -c rr.c

sjf.o: sjf.c
	gcc -c sjf.c

util.o: util.c
	gcc -c util.c

clean:
	rm *.o
test:
	gcc main.c test_psjf.c sjf.c fifo.c rr.c util.c -o main
