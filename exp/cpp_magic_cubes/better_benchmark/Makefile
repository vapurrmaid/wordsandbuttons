all: gcc run clean
.PHONY: gcc
gcc:
	g++ -O2 -std=c++14 empty_run.cpp -o empty_run
	g++ -O2 -std=c++14 naive.cpp -o naive
	g++ -O2 -std=c++14 numbers.cpp -o numbers
	g++ -O2 -std=c++14 numbers_permutation_shifts.cpp -o numbers_permutation_shifts			
	g++ -O2 -std=c++14 numbers_5_heuristic.cpp -o numbers_5_heuristic		
.PHONY: s
s:
	g++ -O2 -S -std=c++14 empty_run.cpp -o empty_run.s
	g++ -O2 -S -std=c++14 naive.cpp -o naive.s
	g++ -O2 -S -std=c++14 numbers.cpp -o numbers.s
	g++ -O2 -S -std=c++14 numbers_permutation_shifts.cpp -o numbers_permutation_shifts.s
	g++ -O2 -S -std=c++14 numbers_5_heuristic.cpp -o numbers_5_heuristic.s
.PHONY: run
run:
	./empty_run
	./naive
	./numbers
	./numbers_permutation_shifts
	./numbers_5_heuristic
.PHONY: clean
clean:	
	rm ./empty_run	
	rm ./naive
	rm ./numbers
	rm ./numbers_permutation_shifts
	rm ./numbers_5_heuristic

