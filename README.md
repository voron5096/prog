**Логин** .\ivc6-10
<br>
**Пароль** 61

[https://lizochekk.jimdofree.com](https://lizochekk.jimdofree.com/%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5)

---

### Компиляторы
http://www.codeblocks.org/downloads/binaries
<br>
https://github.com/Embarcadero/Dev-Cpp

### Огромное спасибо
- https://github.com/Vedji/Procedural_Programming_HomeWork
- https://github.com/vbg911/procedural-programming
- https://github.com/MintyRoma/PP_MIREA
- https://github.com/zubai69
- https://github.com/karpelevi4?tab=repositories
- https://github.com/Bigljuse/UniversityHomeWorkCPP

Макаров Максим Алексеевич

---

12 практическая https://mirea.ninja/t/informatika-12-prakticheskaya-ctrl-c/2532

https://yaso.su/ibvo0503

## Домашнее задание 1
### 1.1 Имя
```c++
#include <iostream>
using namespace std;

int main() {
    setlocale(LC_ALL, "Russian"); // вывод русских букв
    cout << "Имя";
    return 0;
}
```
### 1.2 Арифметика
```c++
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    if (b == 0) {
        cout << "You cannot divide by 0";
    }
  
    cout << "a + b = " << a + b << endl;
    cout << "a - b = " << a - b << endl;
    cout << "a * b = " << a * b << endl;
    cout << "a / b = " << a / b << endl;
    return 0;
}
```

### 1.3 Уравнение
```c++
#include <iostream>
using namespace std;

int main() {
  int b, c;
  cin >> b >> c;
  if (b == 0) {
    cout << "division by zero" << endl;
    return 0;
  }
  
  int x = -c/b;
  cout << x;
  return 0;
}

```

### 1.3 Ещё одно уравнение

```c++
#include <iostream>
#include <math.h>
using namespace std;

int main() {
  int a, b, c;
  cout << "--------- \n";
  cout << "a = ";
  cin >> a;
  cout << "b = ";
  cin >> b;
  cout << "c = ";
  cin >> c;
  
  float d = (b*b)-4*a*c; // считаем d
  
  if (a == 0) { // если a = 0, то считаем линейное уравнение
    if (b == 0) {
    cout << "division by zero" << endl;
    main();
    }
  
  int x = -c/b;
  cout << "x = " << x << endl;
  main();
  }
  
  if (d < 0) { // если d < 0, то корней нет
    cout << "No solution" << endl;
    main();
  }
  else if (d == 0) { // если d = 0, то корень один
    cout << "x = " << (-b)/(2*a) << endl;
    main();
  }
  else {
    cout << "x1 = " << (-b + sqrt(d))/(2*a) << endl;
    cout << "x2 = " << (-b - sqrt(d))/(2*a) << endl;
    main();
  }

  return 0;
}
```

### 1.4 Лампа со шторой
Светло: день И раздвинуты шторы ИЛИ включена лампа
<br>
Светло ли в комнате?
```c++
#include <iostream>
using namespace std;

int main() {
  setlocale(LC_ALL, "Russian"); // вывод русских букв
  int time, curtains, lamp;
  cout << "Введите данные: \n";
  cout << "Про время суток (1 - день, 0 - ночь) \n";
  cout << "Про шторы (0 - раздвинуты, 1 - закрыты) \n";
  cout << "И лампу (1 - включена, 0 - выключена) \n";
  cin >> time >> curtains >> lamp;
  if (lamp == 1) {
    cout << "В комнате светло \n";
  }
  else if (time == 1 and curtains == 0) {
    cout << "В комнате светло \n";
  }
  else {
    cout << "В комнате темно \n";
  }

  return 0;
}

```
## Домашнее задание 2

### 2.1 Конус
```c++
#include <iostream>
#include <math.h>
using namespace std;

int main() {
    double R; // нижнее основание
    double r; // верхнее основание
    double h;
    
    cout << "R = ";
    cin >> R;
    cout << "r = ";
    cin >> r;
    cout << "h = ";
    cin >> h;
    cout << "---------\n";
    if (R <= 0 or r <= 0 or h <= 0) {
      cout << "No solution!\n";
      main();
    }
    float l = sqrt(pow(R, 2) + pow(h, 2));
    float S = M_PI * (pow(R, 2) + (R + r) * l + pow(r, 2));
    float V = 0.3333333333 * M_PI * h * (pow(R, 2) + R * r + pow(r, 2));
    cout << "l = " << l << endl;
    cout << "S = " << S << endl;
    cout << "V = " << V << endl;
    return 0;
}
// 3 2.5 8.016
```

### 2.2 Развлетвление
```c++
#include <iostream>
#include <cmath>
using namespace std;

int main() {
    double x;
    double a;
    double w;
    cin >> x >> a;
    if (x == 0) {
      cout << "x cannot be equal to 0" << endl;
    }
    else if (a - pow(x, 2) < 0) { 
      cout << "You cannot extract the root of a negative number" << endl;
    }
    else if (abs(x) < 1) {
      w = a * log(abs(x));
      cout << w << endl;
    }
    else {
      w = sqrt(a - pow(x, 2));
      cout << w << endl;
    }
}
```

### 2.3 Функция
```c++
#include <iostream>
#include <math.h>
using namespace std;

int main() {
    double x, y, b, z;
    
    cout << "x = ";
    cin >> x;
    cout << "y = ";
    cin >> y;
    cout << "b = ";
    cin >> b;
    
    if (b - y <= 0 or b - x < 0) {
        cout << "the coefficient of log() cannot be less than or equal to 0 OR the root cannot be extracted from a negative number";
    }
    else {
    	z = log(b - y) * sqrt(b - x);
    	cout << "z = " << z;
	}

    return 0;
}
```

### 2.4 Порядок
```c++
#include <iostream>
using namespace std;


int main() {
    int N;
    
    cout << "N = "; // ввод переменных
    cin >> N;
    
    if (N <= 0) { // проверка что N натуральное число
        cout << "N is not natural number";
        return 0;
    }
    
    for (int i = 0; i < 10; i++) { // вывод 10 натуральных чисел
        cout << N++ << endl;
    }
    
    return 0;
}
```

### 2.5 Табуляция
```c++
#include <iostream>
#include <math.h>
using namespace std;

int main() {
    float x, y;
	for (x = -4; x <= 4; x += 0.5) { // изменение X от -4 до 4 с шагом 0.5
		y = (x * x - 2 * x + 2) / (x - 1); // функция

		if (x - 1 == 0) { // проверка деления на нуль
			cout << "y(" << x << ") = " << "division by zero!" << endl;
		}
		else {
			cout << "y(" << x << ") = " << y << endl;
		}
	}
    return 0;
}
```
