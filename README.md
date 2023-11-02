#include <iostream>
using namespace std;
int main()

{
    char option;

      cout << "choose your option: \n a. Check prime number  \n b. find Prime Numbers in a range "  << endl;
      cin >> option;
    

   switch(option)
   {
    case 'a':
      int number;
      cout << " Enter a number: ";
      cin >> number;
      for  (int j = 2; j < number; j++)
   {
      if (number % j == 0)
   {
      cout << " not a prime number\n"<<endl;

      break;
   }
   else
   {
      cout << " prime Number\n"<<endl;
      break;
   }

   }
      break;
    case 'b':
     int minimumnumber;
     cout << " enter minimum number in the range:\n ";
     do
   {
     cin >> minimumnumber;
   }
     while (minimumnumber < 1);

     int maximumnumber;
     cout << "enter maximum number in the range:\n ";
     do
   {
     cin >> maximumnumber;
   }
     while (minimumnumber >= maximumnumber);

     for (int a = minimumnumber; a <= maximumnumber; a++)
   {

     for  (int b = 2; b < maximumnumber; b++)
   {
        
	if (a % b != 0)
   {
        
	cout << a <<endl;
   }

    break;
          
   }
   
   }
   
   }
}