#include <iostream>

using namespace std;

void getNumbers(double num1, double num2, double num3, double num4, double &avg, double &max, double &min){
  
avg = (num1 + num2 + num3 + num4)/4;

max = num1;
if(max < num2)
max = num2;
if(max < num3)
max = num3;
if(max < num4)
max = num4;
  
  
min = num1;
if(min > num2)
min = num2;
if(min > num3)
min = num3;
if(min > num4)
min = num4;
}

int main()
{
double num1 = 4.6, num2=3.7, num3 = -1.7, num4 = -7.8, avg, min, max;
cout<<"\nPlease enter four numbers:";
cout << "\nNumber 1:" << endl;
cin>> num1;

cout << "\nNumber 2:" << endl;
cin>> num2;

cout << "\nNumber 3:" << endl;
cin>> num3;

cout << "\nNumber 4:" << endl;
cin>> num4;

getNumbers(num1, num2, num3, num4, avg, max, min);
cout<<"\nMinimum is "<< min;
cout<<"\nMaximum is "<<max;
cout<<"\nAverage is "<<avg;

return 0;
}
