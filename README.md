# OOP.29.03

#include <iostream>
using namespace std;

class Fraction
{
public:
	int a, b;
	int c, d;
	int e, f;
	void Output()
	{
		cout << "Enter values for the first fraction: " << endl;
		cout << "\tNumerator - ";
		cin >> a;
		cout << "\tDenominator - ";
		cin >> b;
		cout << "Enter values for the second fraction:" << endl;
		cout << "\tNumerator - ";
		cin >> c;
		cout << "\tDenominator - ";
		cin >> d;
	}
	
	void Addition()
	{
		e = (a*d) + (b*c);
		f = b*d;
		cout << a << "/" << b << " + " << c << "/" << d << " = " << e << "/" << f << endl;
	}
	void Subtraction()
	{
		e = (a*d) - (b * c);
		f = b*d;
		cout << a << "/" << b << " - " << c << "/" << d << " = " << e << "/" << f << endl;
	}
	void Multiplication()
	{
		e = (a*d) / (b*c);
		f = b*d;
		cout << a << "/" << b << " * " << c << "/" << d << " = " << e << "/" << f << endl;

	}
	void Division()
	{
		e = (a*d) * (b*c);
		f = b*d;
		cout << a << "/" << b << " / " << c << "/" << d << " = " << e << "/" << f << endl;
	}
};

int main()
{
	Fraction fraction;
	fraction.Output();
	int a;
	do {
		cout << "\n1. Addition.";
		cout << "\n2. Substraction.";
		cout << "\n3. Multiplication.";
		cout << "\n4. Division." << endl;
		cout << "\nSelect the required operation - ";
		cin >> a;
		switch (a)
		{
		case 1: (a = 1);
			fraction.Addition();
			break;
		case 2: (a = 2);
			fraction.Subtraction();
			break;
		case 3: (a = 3);
			fraction.Multiplication();
			break;
		case 4: (a = 4);
			fraction.Division();
			break;
		case 5: (a = 5);
			break;
		}
	}
	while (a != 5);
	    cout << "Programm stopped.\n";
	return 0;
}
