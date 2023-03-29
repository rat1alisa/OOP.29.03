# OOP.29.03
#include <iostream>
#include <iomanip>
using namespace std;

class Fraction
{
public:    
   int numerator;
   int denominator;
   int newnum;
   int newdeno;
   void input()
   {
       cin >> numerator >> denominator;
   }
   void print()
   {
       cout << endl;
       cout << numerator << "/" << denominator;
   }
   void addition(int a, int b)
   {
       newnum = (numerator * y) + (denominator * x);
       newdeno = denominator * y;
       cout << "Sum = " << newnum << "/" << newdeno;
   }
   void subtraction()
   {
       
   }
   void multiplication()
   {
       
   }
   void division()
   {
       
   }
};

int main()
{
    Fraction first;
    Fraction second;
    cout << "First fraction: ";
    first.input();
    cout << "Second fraction: ";
    second.input();
    //-------------------
    cout << "Enter the required operation - " << endl;
        cout << "1. Addition" << endl;
        cout << "2. Subtraction" << endl;
        cout << "3. Multiplication" << endl;
        cout << "4. Division" << '\n';
        cin >> m;
        switch (m)
        {
        case 1:
            first.addition(a);
            break;
        case 2:
            first.sbtraction(a);
            break;
        case 3: 
            first.multiplication(a);
            break;
        case 4:  
            first.division(a);
            break;
        default: 
            cout << "Error" << endl;
        }
    //-------------------
    first.print();
    second.print();
    int x = second.numerator;
    int y = second.denominator;
    first.addition(x, y);
}
