CFLAGS = -Wall

default: myexe
myexe: fileio.o utils.o proj_refactor_file.o
	g++ $(CFLAGS) -o myexe fileio.o utils.o proj_refactor_file.o
	
fileio.o: ../fileio/fileio.cpp ../includes/fileio.h ../includes/constants.h
	g++ $(CFLAGS) -c ../fileio/fileio.cpp
	 
utils.o: ../utils/utils.cpp ../includes/utils.h ../includes/constants.h
	g++ $(CFLAGS) -c ../utils/utils.cpp
	
proj_refactor_file.o: ../src/proj_refactor_file.cpp ../includes/constants.h ../includes/utils.h ../includes/fileio.h	
	g++ $(CFLAGS) -c ../src/proj_refactor_file.cpp

clean: rm -f *.o myexe