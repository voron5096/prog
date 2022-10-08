**Логин** .\ivc6-10
<br>
**Пароль** 61

[https://lizochekk.jimdofree.com](https://lizochekk.jimdofree.com/%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5)

https://drive.google.com/drive/folders/1T8KGQzLWOGvZWzi3enRzfc3__xW3sQtq?usp=sharing
<br>
https://drive.google.com/drive/folders/1Rh50529LxhNPl_TIQUIOIWV7k5EShAM3


---

### Компиляторы
http://www.codeblocks.org/downloads/binaries
<br>
https://github.com/Embarcadero/Dev-Cpp

### Огромное спасибо
- https://github.com/Vedji/Procedural_Programming_HomeWork
- https://github.com/vbg911/procedural-programming
- https://github.com/Nick648/C-plus-_Codes
- https://github.com/MintyRoma/PP_MIREA
- https://github.com/zubai69
- https://github.com/micr0chip/CompilerLAB7
- https://github.com/Kyinex/Homework
- https://github.com/ledhcg/Mos19_si2pls
- https://github.com/ViktorVlasov/Homework-Mirea
- https://github.com/NEK-RA/university-homeworks
- https://github.com/Alunchik
- https://github.com/soumirel/RTU_ProceduralProgramming_1stSemester_Task4
- https://github.com/Haze272/University-programming
- https://github.com/karpelevi4?tab=repositories
- https://github.com/Kreckeroff/1sem_PP
- https://github.com/Bigljuse/UniversityHomeWorkCPP

---

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

## Домашнее задание 3
### 3.1 «Заем»
Месячная выплата m по займу в S рублей на n лет под процент p вычисляется по формуле

![изображение](https://user-images.githubusercontent.com/70198995/193253807-93376b73-5d95-4ee6-8386-9a82694b2de6.png)

```c++
#include <iostream>
#include <math.h>
using namespace std;

int main() {
double S; 
double p;
double n;
double r;
double m;
cout << "----------------------- \n";
cout << "S = ";
cin >> S;
cout << "p = ";
cin >> p;
cout << "n = ";
cin >> n;
  
if (S <= 0) {
  cout << "Numbers cannot be less than zero! \n";
  main();
  }

else if (p == 0) {
  m = S / (12 * n);
}

else {
  r = p / 100;
  m = S * r * pow(1 + r, n) / (12 * (pow(1 + r, n) - 1));
}

if (12 * (pow(1 + r, n) - 1) < 0) {
  cout << "You can't divide by 0! \n";
  main();
  }

cout << "m = " << m << endl;
main();
}
```

### 3.2 «Ссуда»
Под какой процент p выдана ссуда величиной S рублей, которая гасится месячными выплатами величиной m в течение n лет. Формула приведена в предыдущей задаче.

```c++
#include <iostream>
#include <math.h>
using namespace std;

int main() {
double S; // начальная ссуда S рублей
double n; // в течении n лет
double mTest; // месячная выплата mTest
double m; // заданная под условие с выплатами r
double r;
double rTemp = 0.0001; // временное r для вычисления
cout << "----------------------- \n";
cout << "S = ";
cin >> S;
cout << "n = ";
cin >> n;
cout << "mTest = ";
cin >> mTest;
  

if (n == 0 or S <= 0) { // на 0 делить нельзя!
  cout << "Incorrect years or amount of credit! \n";
  main();
  }

while (m < mTest) { ////// находим когда выплаты будут больше заданного, и выводим нужный %
  r = rTemp;
  m = S * r * pow(1 + r, n) / (12 * (pow(1 + r, n) - 1)); // подсчёт m с течением времени
  rTemp = rTemp + 0.0001;
  }

cout << "p = " << r * 100 << "%" << endl;  
main();
}
```

### 3.3 «Копирование файла»
Создать на диске текстовый файл и скопировать его на экран.

```c++
#include <iostream>
#include <fstream>
#include <string.h>
using namespace std;

int main() {
setlocale(LC_ALL, "rus"); // корректное отображение Кириллицы
char readline[30]; // буфер промежуточного хранения считываемого из файла текста
ifstream fin("33.txt"); // открыли файл для чтения
while (fin.getline(readline, 30)) {
  for (int i = 0; i < strlen(readline); i++) { // пробегание по кол-ву символов строки
    cout << readline[i];
  }
  cout << "\n"; // перенос на другую строку
}
fin.close();
return 0;
}
```
### Другое решение
```c++
    fstream fileStream;
    fileStream.open("33.txt");

    char readline[30];
    if (fileStream.fail()) {
        cout << "file not exist";
        ofstream fout("33.txt");
    }
    else {
        cout << "nice";
        ifstream fin("33.txt");
        while (fin.getline(readline, 30)) {
          for (int i = 0; i < strlen(readline); i++) {
            cout << readline[i];
          }
          cout << "\n";
        }
        fin.close();
    }
```

### 3.4 «Фильтр»
Вывести на экран только числа из созданного Вами на диске текстового файла, содержащего буквы и числа.

```c++
#include <iostream>
#include <fstream>
#include <string.h>
using namespace std;

int main() {
  setlocale(LC_ALL, "rus"); // корректное отображение Кириллицы
  char readline[30]; // буфер промежуточного хранения считываемого из файла текста
  ifstream fin("33.txt"); // открыли файл для чтения
  while (fin.getline(readline, 30)) {
    
    for(int i = 0; i < strlen(readline); i++) {
      if (isdigit(readline[i]) or readline[i] == '-' or readline[i] == ',' or readline[i] == '.') { // проверка на число
        cout << readline[i];
      }
    }
    
    cout << "\n"; // перенос на другую строку
    
  }
  fin.close();
}
```

### 3.5 «Сортировка букв»
Задать строку из 30 букв и расставить их в алфавитном порядке.

```c++
#include <iostream>
#include <fstream>
#include <string.h>
#include <algorithm>
using namespace std;

int main() {
  setlocale(0, "");
  string x;
  int i = 0;
  cout << "----------------------- \n";    
  getline(cin, x); // функция скушает строки с пробелами
  
  
  for (int i = 0; i < x.length() - 1; i++) {
    for (int j = i; j < x.length() - 1; j++) { 
      if (x[i] > x[j + 1]) {
        swap(x[i], x[j + 1]);
        }
      }
  }
  cout << x.substr(count(x.begin(), x.end(), ' '), x.length()) << endl; // конструкция чистит пробелы " "
  main();
```
### 4.1 «Файл»
Создать файл, записать в него 10 чисел, закрыть, потом вновь открыть файл и найти сумму чисел.

Ввод в консоли!

```c++
#include <iostream>
#include <fstream>
using namespace std;

int main() {
  int i = 0; // кол-во цифр
  double sum = 0; // сумма
  double digital = 0;
  
  ofstream file("41.txt");
  while (i != 10) { // ввод чисел
  	i += 1;
  	cout << i << ") ";
  	if (cin >> digital) { // проверка на число
  		file << digital << "\n"; // запись в файл
	  }
	else {
		cout << "Incorrect input!" << endl;
		return 0;
	}
  }
  file.close();
  
  ifstream ifile("41.txt");
  while (i != 20) { // сумма чисел
  	ifile >> digital; // чтение из файла
    sum += digital; 
    i += 1;
  }
  ifile.close();
  
  cout << "SUM = " << sum << endl;
  return 0;
}
```
