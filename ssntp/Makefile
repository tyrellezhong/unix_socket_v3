include ../Make.defines

PROGS =	ssntp

all:	${PROGS}

ssntp:	main.o sntp_proc.o
		${CC} ${CFLAGS} -o $@ main.o sntp_proc.o ${LIBS} 

clean:
		rm -f ${PROGS} ${CLEANFILES}\
		cd build && rm -f ${PROGS} ${CLEANFILES}
install:
		mv ${PROGS} ${CLEANFILES} build/
