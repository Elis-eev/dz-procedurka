# dz-procedurka
#include <cmath>
 
using namespace std;
 
int main()
{
  double a,b,c,d,x,x1;
 
  cout << "Введите a\n";
  cin >> a;
  cout << "Введите b\n";
  cin >> b;
  cout << "Введите c\n";
  cin >> c;
 
  d = b * b - 4 * a * c;
  if (d > 0)
  {
    x1 = ((-b) + sqrt(d)) / (2 * a);
    x = ((-b) - sqrt(d)) / (2 * a);
    cout << "x1 = " << x1 << "\n";
    cout << "x = " << x << "\n";
  }
  if (d == 0)
  {
    x1 = -(b / (2 * a));
    cout << "x1 = x = " << x1 << "\n";
  }
  if (d < 0)
    cout << "дискриминант меньше нуля";
}


#include <iostream> не робит!!!!!

int main()
{
    setlocale(LC_ALL, "rus");
    std::cout << " ax^2 + bx + c = 0 , ";
    int a, b, c, x1, l, x2;
    std::cout << "введите значение a\n";
    std::cin >> a;
    std::cout << "введите значение b\n";
    std::cin >> b;
    std::cout << "введите значение c\n";
    std::cin >> c;
    l = b ^ 2 - 4 * a * c;
    if (l > 0);
    {
        x1 = (-b + sqrt(l)) / 2 * a;
        std::cout << "x1 = " << x1 << "\n";
        x2 = (-b - sqrt(l)) / 2 * a;
        std::cout << "x2 = " << x2 << "\n";
    }
    if (l < 0);
    {
        std::cout << "решение уравнения с данными значениями невозможно ";
    }
    if (l == 0);
    {
        x1 = -b / (2 * a);
        std::cout << "x1 = x2 = " << x2 << "\n";
    }
    system("break");
}


#include <iostream>                                         //2.1
#include <cmath>

using namespace std;

int main()
{
	setlocale(0, "");
	float p = 3.14;
	float h, R, r, l;
	cout << "h= ";
	cin >> h;
	cout << "R = ";
	cin >> R;
	cout << "r = ";
	cin >> r;
	cout << "l = ";
	cin >> l;
	float R1, r1;
	R1 = pow(R, 2);
	r1 = pow(r, 2);
	cout << "V = " << (p * h * (R1 + R * r + r1)) / 3 << "\n";
	cout << "S = " << p * (R1 + (R + r) * l + r1);

}



#include <iostream>                                  //2.2
#include <cmath>

using namespace std;

int main() {
	setlocale(LC_ALL, "Russian");
	float x, a;
	cout << "x = ";
	cin >> x;
	cout << "a= ";
	cin >> a;
	float w, l, s, x1;
	if (x == 0)
	{
		cout << "неподходящее значение";
	}
	else
	{
		if (abs(x) < 1)
		{
			l = log(abs(x));
			cout << a * l;
		}
		else
		{
			x1 = pow(x, 2);
			if (a < x1)
			{
				cout << "Решений нет";
			}
			else
			{
				cout << sqrt((a - x1));
			}

		}
	}
}
