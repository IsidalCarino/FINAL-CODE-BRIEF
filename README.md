# FINAL-CODE-BRIEF
```
#include <iostream>
#include <array>
using namespace std;
int main()
{
    cout << "Welcome! Would you like to buy some Coffee or Tea?\nHere is our MENU:\n\n";
    {
        string menu[4][6] = {
        {"Drink Number  ","Coffee        ","Price(AED) | ","Drink Number  ","Tea        ","Price(AED) "},
        {"     1        ","Ice Coffee    ","    3      | ","     4        ","Ice Tea    ","    3 "},
        {"     2        ","Milk Coffee   ","    2      | ","     5        ","Milk Tea   ","    2 "},
        {"     3        ","Black Coffee  ","    1      | ","     6        ","Black Tea  ","    1 "},
        };
        for (int x = 0; x < 4; x++) {
            for (int y = 0; y < 6; y++)
            {
                cout << menu[x][y] << "";
            }
            cout << endl;
        }
    }
    {}
    cout << "\nPlease enter the number of the drink you want to order: ";
    int order;
    cin >> order;
    while (cin.fail() || order >=7 || order <=0)
    {
        cout << "Invalid drink. Please choose another drink from MENU above and enter it's NUMBER: ";
        cin.clear();
        cin.ignore(1000, '\n');
        cin >> order;
    }
    if (order == 1) {
        cout << "Ice Coffee." << endl;
    }
    else if (order == 2) {
        cout << "Milk Coffee." << endl;
    }
    else if (order == 3) {
        cout << "Black Coffee." << endl;
    }
    else if (order == 4) {
        cout << "Ice Tea." << endl;
    }
    else if (order == 5) {
        cout << "Milk Tea." << endl;
    }
    else if (order == 6) {
        cout << "Black Tea." << endl;
    }
    {
        cout << "\nWould you like to add sugar? (Y/N): ";
        char sugar;
        cin >> sugar;
        switch (sugar)
        {
        case'Y':
        case'y':
        {
            cout << "Sugar will be added." << endl;
            break;
        }
        case'N':
        case'n':
        {
            cout << "Sugar will NOT be added." << endl;
            break;
        }
        default:
        {
            cout << "Input is not recognized. But we will be providing sachet of sugar for you; just incase you need it." << endl;
            break;
        }
        }
    }
    {
        double a = 1, b = 2, c = 3;
        double money;   
        cout << "\nPlease enter your money(AED):";
        cin >> money;
        double z = money - a;
        double x = money - b;
        double y = money - c;
        while (cin.fail())
        {
            cin.clear();
            cin.ignore();
            cout << "\nInvalid Input. Please input your amount of money: ";
            cin >> money;
        }
        if (z < 0 && x < 0 && y < 0) {
            cout << "\nSorry. you do not have enough money to buy this drink." << endl;
        }
        if (order == 1) 
        {
            cout << "Ice Coffee costs 3 AED." << endl << "You paid: " << money << endl << "Your change is: " << y << endl;
            if (y >= 0)
                cout << "Thanks you come again.\nEnjoy your Ice Coffee!" << endl;
            if (y < 0)
                cout << "Your money is not enough. Please take your money back and come again next time." << endl << "Returning: " << money;
        }
        if (order == 2)
        {
            cout << "Milk Coffee costs 2 AED." << endl << "You paid: " << money << endl << "Your change is : " << x << endl;
            if (x >= 0)
                cout << "Thanks you come again.\nEnjoy your Milk Coffee!" << endl;
            if (x < 0)
                cout << "Your money is not enough. Please take your money back and come again next time." << endl << "Returning: " << money;
        }
        if (order == 3) 
        {
            cout << "Black Coffee costs 1 AED." << endl << "You paid: " << money << endl << "Your change is: " << z << endl;
            if (z >= 0)
                cout << "Thank you come again.\nEnjoy your Black Coffee!" << endl;
            if (z < 0)
                cout << "Your money is not enough. Please take your money back and come again next time." << endl << "Returning: " << money;
        }
        if (order == 4) 
        {
            cout << "Ice Tea costs 3 AED." << endl << "You paid: " << money << endl << "Your change is: " << y << endl;
            if (y >= 0)
                cout << "Thank you come again.\nEnjoy your Ice Tea!" << endl;
            if (y < 0)
                cout << "Your money is not enough. Please take your money back and come again next time." << endl << "Returning: " << money;
        }
        if (order == 5) 
        {
            cout << "Milk Tea costs 2 AED." << endl << "You paid: " << money << endl << "Your change is: " << x << endl;
            if (x >= 0)
                cout << "Thank you come again.\nEnjoy your Milk Tea!" << endl;
            if (x < 0)
                cout << "Your money is not enough. Please take your money back and come again next time." << endl << "Returning: " << money;
        }
        if (order == 6) 
        {
            cout << "Black Tea costs 1 AED." << endl << "You paid: " << money << endl << "Your change is: " << z << endl;
            if (z >= 0)
                cout << "Thank you come again.\nEnjoy your Black Tea!" << endl;
            if (z < 0)
                cout << "Your money is not enough. Please take your money back and come again next time." << endl << "Returning: " << money;
        }
    }
} 
```
