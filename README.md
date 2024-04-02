#include<iostream>
#include<random>
using namespace std;


void pet();

int main() { //starting point of program!
	srand(time(NULL));
	char input = 'g';
	while (1) {//game loop
		cout << "press f to fish" << endl;
		cin >> input; //gets user input
		if (input == 'f')
			pet();
	}
}
void pet() {
	int num = rand() % 100; //0-99

	if (num < 33) //33% chance
		cout << "Carp";
	else if (num < 66) //33% chance
		cout << "Woodsjup";
	else if (num < 99) //33% chance
		cout << "Catfish";
}
