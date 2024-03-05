#include<iostream>
using namespace std;
int main()
{

	double num1, num2;
	char operation;
	cout << "enter first number" << endl;
	cin >> num1;
	cout << "enter second number" << endl;
	cin >> num2;
	cout << "choice an operation (+,-,*,/)" << endl;
	cin >> operation;

	double result{};
	switch (operation) {
	case '+':
		result = num1 + num2;
		break;
	case'-':
		result = num1 - num2;
		break;
	case'*':
		result = num1 * num2;
		break;
	case'/':
		if (num2 != 0) {
			result = num1 / num2;
		}
		else {
			cout << "Error: Cannot divide by zero." << endl;
		}
		break;

	default:
		cout << "Invalid choice. Please choice an operation (+,-,*,/)" << endl;
	}

	cout << "result = " << result << endl;
	return 0;






}
