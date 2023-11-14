#include <iostream>
#include <string>
#include <math.h>
using namespace std;
void input_interger( string label, int &n);
bool is_prime(int n);
int main ()
{
   int n;
   input_interger("n= ",n);
   if ( is_prime(n))
   {
    cout <<n <<" la so nguyen to";
   } else {
    cout <<"khong phai la so nguyen to";
   }
} 

void input_interger( string label, int &n)
{
  cout <<label;
  cin >>n;
}
bool is_prime(int n)
{
  for ( int i = 2; i <=sqrt(n);i++)
  {
    if ( n % i == 0)
    {
      return false;
    }
  }
  return true;
}
