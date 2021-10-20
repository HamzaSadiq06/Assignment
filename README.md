# Assignment
#include<iostream>
#include<cstdlib>
#include<ctime>
using namespace std;

int main ()
{

char user, computer;
int randNum;
srand(5);
randNum = rand() % 3;

if (randNum == 0)
    computer = 'R';
else if (randNum == 1)
     computer = 'P';
else 
     computer = 's';
cout << "Enter R, P, S:";
cin >> user;

if (computer =='R'){
    if (user =='R')
       cout << "its a tie!";
    else if (user == 'p')
       cout << "you win!";
    else 
      cout << "you lose!";
}
     else if (computer =='P'){
     if (user == 'R')
         cout << "you lose!";
     else if(user == 'P')
        cout << "its a tie!";
     else
        cout << "you win!";
     }

     else {
     if (user == 'R')
         cout << "you win!";
     else if (user == 'P')
        cout << "you lose!";
    else
        cout << "its a tie!";
     }

    return 0;
    
}
