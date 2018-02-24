# Solving-Quadratics
Please enter the general formula of the quadratic equation
//Solution of binary first order equation
#include <iostream>
#include<math.h>
using namespace std;

int main()
{
    int xh = 0,cs = 0;
    cout << "How many times do you want to run?\nPlease enter the number.\n";//你想运行几次？请输入数值。
    cin >> cs;
    while (xh <= cs-1 )
    {
        int a = 0, b = 0, c = 0;
        int f = 0;
        cout << "\nPlease enter the value of a, b and c:" << endl;//请输入a b c 的值：
        cin >> a >> b >> c;
        if (b * b - 4 * a * c >= f)
        {
            if (b * b - 4 * a * c == f)
            {
                cout << "X1=X2= " << b / -2 * a << endl;
            }
            else
            {
                cout << "△= " << b * b - 4 * a * c << endl;
                cout << "X1= " << -1 * b - sqrt(b * b - 4 * a * c) / 2 * a << endl;
                cout << "X2= " << -1 * b - sqrt(b * b + 4 * a * c) / 2 * a << endl;
            }
        }
        else
        {
            cout << "This equation has no real roots!" << endl;//此方程无实数根！
        }
        xh ++;
    }
    cout << "\n\nThank you for using";
    return 0;
}
