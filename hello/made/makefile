CXX = g++
DEV = -g
HOME = ../
HEAD = $(HOME)headers/
O_HI = hello.o world.o
C_FLAGS = $(DEV) -c
L_FLAGS = $(DEV)

all: hi2u

hi2u: $(O_HI)
	$(CXX) $(L_FLAGS) $(O_HI) -o hi2u

hello.o: $(HEAD)hello.h $(HOME)hello.cpp
	$(CXX) $(C_FLAGS) $(HOME)hello.cpp

world.o: $(HOME)world.cpp $(HEAD)hello.h
	$(CXX) $(C_FLAGS) $(HOME)world.cpp

clean: 
	\rm *.o
