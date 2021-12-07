# Summative-Assessment-2-
#loops
#include<iostream>
#include<math.h>
using namespace std;
int main()
{
	string firstname, secondname;
	int number, factorial=1;
	int table;
	int i = 1;
	cout << "Enter your full name: ";
	cin >> firstname >> secondname;
	cout << "\nEnter a number: ";
	cin >> number;
	while (cin.fail() != 0)
	{
		cout << "\aInvalid command\nEnter a number: ";
		cin.clear();
		cin.ignore();
		cin >> number;
	}
	do
	{
		factorial = factorial * i;
		i++;
	} while (i <= number);
	
	cout << "\nFactorial of " << number << " is : " << factorial << endl;
	cout << "\nTable of " << number << " is: " << endl;
	for (int j = 50; j >= 40; j--)
	{
		cout << number << " X " << j << " = " << number * j << endl;
	}
	cout << "\nThe exponent power of " << number << " from 5-0 is: \n";
	cout << number<<"^5 is : " << pow(number, 5) << endl;
	cout << number<<"^4 is : " << pow(number, 4) << endl;
	cout << number<<"^3 is : " << pow(number, 3) << endl;
	cout << number<<"^2 is : " << pow(number, 2) << endl;
	cout << number<<"^1 is : " << pow(number, 1) << endl;
	cout << number<<"^0 is : " << pow(number, 0) << endl;
	return 0;
}
