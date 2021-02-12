# Lab-7.30-
#include <iostream>
using namespace std;

int main() {
  const int INSTATETUITION = 3000;
  const int OUTSTATETUITION = 4500;
  const int INSTATEROOM = 2500;
  const int OUTSTATEROOM = 3500;
  int status;
  int room;
  
  cout << "Enter 1 for in-state residency or 2 for out-of-state:\n";
  cin >> status;

  cout << "Enter 1 for if you need room and board or 2 for no room and board:\n";
  cin >> room; 
  
  if (status == 1 && room == 2)
  {
    cout << "Your total bill for this semester is $" << INSTATETUITION + OUTSTATEROOM << endl;
  }
  
  if (status == 2 && room == 1)
  {
    cout << "Your total bill for this semester is $" << OUTSTATETUITION + INSTATEROOM << endl;
  }
}
