// c++ program to to convert decimal number into binary number
using namespace std;
#include<iostream>
#include<math.h>
int main() {
int decimal_num, remainder, binary_num=0, i=0;
cout<<"enter the decimal number: ";
cin>>decimal_num;
while(decimal_num != 0) {
remainder= decimal_num%2;
binary_num= binary_num + remainder * pow(10, i);
decimal_num= decimal_num/2;
i++;
}
cout<<endl<<"the binary equivalent= "<<binary_num;
return 0;
}
