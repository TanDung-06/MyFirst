"Hello,Github!"
#include <iostream>
 using namespace std;
 // Recursive function to solve Tower of Hanoi
 void towerOfHanoi(int n, char from_rod, char to_rod, char aux_rod) {
 if (n == 1) {
 6
7 cout<<"Movedisk1from"<<from_rod<<"to"<<to_rod<<endl;
 8 return;
 9 }
 10 towerOfHanoi(n-1,from_rod,aux_rod,to_rod);
 11 cout<<"Movedisk"<<n<< "from"<<from_rod<<"to"<<to_rod<<endl;
 12 towerOfHanoi(n-1,aux_rod, to_rod,from_rod);
 13 }
 14
 15 intmain() {
 16 intn=3;//Numberofdisks
 17 towerOfHanoi(n,'A','C','B');
 18 return 0;
 19 }