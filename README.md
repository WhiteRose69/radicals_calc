# radicals_calc
This tool will help you to calculate what number on what power is your number.
For example you choose 256 -> The result will be 16 power of 2 wich is 256 ,4 power of 4 which is also 256 and 2 power of 8.
I am a lazy person so i don't want to think and calculate because it takes time but with this program you need a few seconds.
Good luck .
P.s It's a simple code and my first on github so don't be cruel.
#################
HERE IS THE CODE I WROTE ON C++
#################
```
#include <iostream>
#include <cmath>
#include <unistd.h>
#include <string>
using namespace std;

int main()
{
    string go;
    void ordinul();
    while (true)
    {
        cout<<"What is the number?\n:";
        ordinul();
        cout << "           Type exit to exit..\n           Continue to continue...\n";
        cin >> go;
        if( go == "exit")
        {
            cout<<"The program will end in ";
            for (int e=1;e<=3;e++)
            {
                cout<<e<<".";
                sleep(1);
            }
            break;
        }else
        {
                continue;
        }
    }
    return 0;
}
void ordinul()
{
    int numarul,radicalul,sum,i,x;
    string go;
    cin>>numarul;
    for(i=1;i<=100;i++)
    {
        for (x=1;x<=100;x=x)
        {
            if(pow(x,i)==numarul)
            {
                cout<<x<<"^"<<i<<endl;
                sleep(2);
                break;
            }
            else
            {
                x=x+1;
            }
        }
    }
}
```
