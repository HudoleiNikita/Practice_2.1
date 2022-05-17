# Practice_2.1
TASK 1
#include <iostream>
using namespace std;
int main() {
    int da = 0; a
    int dada = 0; b
    char operation;
    cout << "Enter first number:";
    cin >> da;
    cout << "Enter second number:";
    cin >> dada;
    cout << "Enter operation:";
    cin >> operation;

    switch (operation) {
        case '-':
            cout << "da - dada = " << da - dada << '\n';
            break;
        case '+':
            cout << "da + dada = " << da + dada << '\n';
            break;
        case '*':
            cout << "da * dada = " << da * dada << '\n';
            break;
        case '/':
            cout << "da / dada = " << da / dada << '\n';
            break;
    }
}
TASK 2
#include <iostream>
#include "windows.h"
int main() {
    std::cout << "Write n:";
    int n = 0;
    std::cin >> n;
    while (n > 0) {
        std::cout << n << " ";
        Sleep(1000); // wait for 1 second
        n--;
    }
}
TASK 3
#include <iostream>
#include <string>
int main()
{
    system("chcp 65001");
    int n;
    std::string apple = "ÿáëîê";
    std::cout<<"Ââåäèòå êîë-âî ÿáëîê:";
    std::cin >> n;
    {
        if ((n==1) || (n % 10 == 1)) {
            apple = apple +"î";
        }
        if ((n > 1 && n < 5) || (n % 10 > 1 && n % 10 < 5)) {
            apple = apple + "à";
        }
        if ((n >= 5 && n < 10) || (n % 10 >= 5 && n % 10 < 10) || (n % 100 > 10 && n % 100 < 15 )) {
            apple = "ÿáëîê";
        }
        std::cout << n << ' ' << apple;
    }
}
