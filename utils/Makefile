CC = gcc 
CXX = g++ 
CFLAGS = -Wall -Wextra -O2 -g
CXXFLAGS = -Wall -Wextra -O2 -g
LDFLAGS = -ldl -lpthread
RM = rm -f

SRCS=$(shell ls *.cpp)
OBJS=$(patsubst %.cpp,%.o,$(SRCS))
 
.PHONY: all
all: main
 
main: $(OBJS)
	@echo "build utils done"

%.o: %.cpp
	-$(CXX) ${CXXFLAGS} -c -o $@ $^
 
.PHONY: clean
clean:
	-${RM} *.o
