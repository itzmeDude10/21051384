# 21051384
#include <iostream>
using namespace std; 
void add(int a, int b)
{
  cout << "sum = " << (a + b);
} 
void add(double a, double b)
{
    cout << endl << "sum = " << (a + b);
}
int main()
{
    add(10, 2);
    add(5.3, 6.2);
    return 0;
}


include<iostream>
using namespace std;
class Complex {
private:
    int real, imag;
public:
    Complex(int r = 0, int i = 0) {real = r;   imag = i;}
    Complex operator + (Complex const &obj) {
         Complex res;
         res.real = real + obj.real;
         res.imag = imag + obj.imag;
         return res;
    }
    void print() { cout << real << " + i" << imag << '\n'; }
};
int main()
{
    Complex c1(10, 5), c2(2, 4);
    Complex c3 = c1 + c2;
    c3.print();
}


#include <iostream>
#include <string>

using namespace std;

template <typename T>
inline T const& Max (T const& a, T const& b){ 
   return a < b ? b:a; 
}
int main () {
   int i = 39;
   int j = 20;
   cout << "Max(i, j): " << Max(i, j) << endl; 
   double f1 = 13.5; 
   double f2 = 20.7; 
   cout << "Max(f1, f2): " << Max(f1, f2) << endl; 
   string s1 = "Hello"; 
   string s2 = "World"; 
   cout << "Max(s1, s2): " << Max(s1, s2) << endl; 
   return 0;
}
