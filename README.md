# 5_practice_c-
Драбинка і кроки до одиниці
#include <iostream>
using namespace std;

int main() 
{
    int n;
    cin >> n;

    for (int i = 1; i <= n; i++) 
    {
        for (int j = 1; j <= i; j++) 
        {
            cout << "*";
        }
        cout << "\n";
    }

    int kroky = 0;

    while (n != 1) 
    {
        if (n % 2 == 0) 
        {
            n = n / 2;
            kroky=n;
            break;
        } else 
        
        {
            n = n * 3 + 1;
            kroky=n;
            break;
        }
    }

    cout << "kroky: " << kroky << "\n";

    return 0;
}
