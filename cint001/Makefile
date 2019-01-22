FC=ifort
LIBS=-lcint
INCLUDES=
FFLAGS=

TARGET=cint001
SRCS=main.f90
OBJS=$(SRCS:.f90=.o)

%.o: %.f90
	$(FC) -o $@ -c $< $(FFLAGS) $(INCLUDES)

$(TARGET): $(OBJS)
	$(FC) -o $(TARGET) $(OBJS) $(FFLAGS) $(LIBS) 

$(OBJS): $(SRCS)

clean:
	rm $(OBJS) $(TARGET)

