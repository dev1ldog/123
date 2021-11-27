#include <iostream>
#include <windows.h>


using namespace std;


void square(int squaresize, char symbol) {
	system("cls");
	int squaresize1 = 0;
	char symbol1 = '*';
	sq1:
	cout << "[-----] Введите необходимый размер квадрата:[-----]  ";
	cin >> squaresize1;
	system("CLS");
	if (squaresize1 < 0) {
		
		cout << "\t[!!!]Вы ввели неверное значение[!!!]\t";
        Sleep(290);
		goto sq1;
		system("cls");
	}
	cout << "[][][]Результат : \n\n";
	for (int j = 1; j < squaresize1; j++) {
		for (int i = 1; i < squaresize1 - 2; i++) {
			cout << symbol1 << "  ";
		}
		cout << "\n";	
	}
	cout << endl;
	cout << endl;
	cout << "  Нажмите Enter:  ";
	cout << endl;
	cout << endl;
	system("pause");
	
}
void square2(int squaresize, char symbol) {
	system("cls");
	int squaresize2 = 0;
	char symbol2 = '#';
	sq2:
	cout << "[-----] Введите необходимый размер квадрата:[----]  ";
	cin >> squaresize2;
	system("CLS");
	if (squaresize2 < 0) {
		cout << "\t[!!!]Вы ввели неверное значение[!!!]\t";
		Sleep(290);
		goto sq2;
		system("cls");
	}
	cout << "[][][]Результат : \n\n";
	for (int j = 1; j < squaresize2; j++) {
		for (int i = 1; i < squaresize2 - 2; i++) {
			cout << symbol2 << "  ";
		}
		cout << "\n";
	}
	cout << endl;
	cout << endl;
	cout << " Введите и нажмите Enter:  ";
	
	cout << endl;
	cout << endl;
	system("pause");

}
void square3(int squaresize, char symbol) {
	system("cls");
	int squaresize3 = 0;
	char symbol3 = '@';
	sq3:
	cout << "[-----] Введите необходимый размер квадрата:[----]  ";
	cin >> squaresize3;
	system("CLS");
	if (squaresize3 < 0) {
		cout << "\t[!!!]Вы ввели неверное значение[!!!]\t";
		Sleep(290);
		goto sq3;
		system("cls");
	}
	cout << "[][][]Результат : \n\n";
	for (int j = 1; j < squaresize3; j++) {
		for (int i = 1; i < squaresize3 - 2; i++) {
			cout << symbol3 << "  ";
		}
		cout << "\n";
	}

	cout << endl;
	cout << endl;
	cout << " Введите и нажмите Enter:  ";
	
	cout << endl;
	cout << endl;

	system("pause");

}	
void triangle(char symbol, int high, int osnova) {
	cout << "[][][]Результат : \n\n";
	for (int i = 0; i < high; i++) {
		for (int j = 1; j < high - i; j++) cout << ' ';
		for (int j = high - 2 * i; j <= high; j++) cout << symbol;
		cout << endl;
	}
	

	system("pause");

}






int main() {
	setlocale(0, "");
	int GLOBALMENU = 0;
	int figure = 0;
	int Rombheight = 0;
	int width = 0;
	int rombmenu = 0;
	int menusquare = 0;
	int squaresize = 0;
	int kalk = 0;
globalmenu:
	system("CLS");

	cout << "--------------------------------------------\n";
	cout << "Введите [1] для печати квадрата            |  \n";
	cout << "--------------------------------------------\n";
	cout << "Введите [2] для печати треугольника        |  \n";	
	cout << "--------------------------------------------\n";
	cout << "Введите [3] для печати прямоугольника      |  \n";
	cout << "--------------------------------------------\n";
	cout << "Введите [4] чтобы запустить калькулятор    |\n";
	cout << "--------------------------------------------\n";
	cout << "Введите [5] Чтобы вывести 10 переменных    |\n";
	cout << "--------------------------------------------\n";
	cout << "Введите [6]  Календарь                     |\n";
	cout << "--------------------------------------------\n";
	cout << "Введите [7] для печати Решетки             |  \n";
	cout << "--------------------------------------------\n";
	cout << "Введите [8] для печати Крестика            |  \n";
	cout << "--------------------------------------------\n";
	cout << "Введите [9] для печати Плюсика            |  \n";
	cout << "--------------------------------------------\n";
	cout << "Введите [10] Чтобы вывести Лабиринт        |\n";
	cout << "--------------------------------------------\n";
	cout << "Введите [11] Чтобы играть в Крестики нолики|\n";
	cout << "--------------------------------------------\n";
	cout << "Введите [12] Открыть настройки меню        |\n";
	cout << "--------------------------------------------\n";
	cout << "Введите [13] чтобы закрыть приложение      |\n";
	cout << "--------------------------------------------\n";
	cout << "[################]Введите и нажмите Enter: ";


	cin >> GLOBALMENU;


	switch (GLOBALMENU) {

	case 1: 
	{
		system("CLS");
		if (GLOBALMENU == 1)
		{
		squaremenu:
			cout << "----------------------------------------------------------\n";
			cout << "\t\tВвыберите символ для печати квадрата     |\n";
			cout << "----------------------------------------------------------\n";
			cout << "\t\tВведите 1 для печати *                   |\n";
			cout << "----------------------------------------------------------\n";
			cout << "\t\tВведите 2 для печати #                   |\n";
			cout << "----------------------------------------------------------\n";
			cout << "\t\tВведите 3 для печати @                   |\n";
			cout << "----------------------------------------------------------\n";
			cout << "\t\tВведите 4 для возвращения в основное меню|\n";
			cout << "----------------------------------------------------------\n";
			cout << " Введите и нажмите Enter:  ";
			cin >> menusquare;
			if (menusquare == 4)
			{
				system("CLS");
				goto globalmenu;

			}


			switch (menusquare) {
			case 1: {
				if (menusquare == 1) {
					char symbol = '*';
					square(symbol, squaresize);
					goto globalmenu;
					break;
				}
			}
			case 2: {
				if (menusquare == 2) {
					char symbol2 = '#';
					square2(symbol2, squaresize);
					goto globalmenu;
					break;

				}
			}
			case 3: {
				if (menusquare == 3) {
					char symbol3 = '@';
					square(symbol3, squaresize);
					goto globalmenu;
					break;
				}
			}
			}

		}
	}

	
	
	case 2: {
		if (GLOBALMENU == 2) {
			system("CLS");
			int vidtri = 0;
			int trimenu = 0;
			int high = 0;
			int osnova = 0;


		triangle:
			cout << "------------------------------------------------------------\n";
			cout << "\t\tВвыберите символ для печати треугольника   |\n";
			cout << "------------------------------------------------------------\n";
			cout << "\t\tВведите [1] для печати - *                 |\n";
			cout << "------------------------------------------------------------\n";
			cout << "\t\tВведите [2] для печати - #                 |\n";
			cout << "------------------------------------------------------------\n";
			cout << "\t\tВведите [3] для печати - @                 |\n";
			cout << "------------------------------------------------------------\n";
			cout << "\t\tВведите [4] для возвращения в основное меню|\n";
			cout << "------------------------------------------------------------\n";
			cout << " Введите и нажмите Enter:  ";
			cin >> trimenu;
			if (trimenu == 4) {
				system("CLS");
				goto globalmenu;

			}
			if (trimenu == 1) {
				system("CLS");
				cout << "\t\t[-]ВВедите высоту треугольника: \n";
				cin >> high;
				if (high < 0) {
					cout << "\t\t[!!!]Вы ввели неверное значение высоты[!!!]";
					goto triangle;
				}
				cout << "\t\t[-]Введите длину основания треугольника \n";
				cin >> osnova;
				if (osnova < 0) {
					cout << "[!!!]Вы ввели неверное значение основания[!!!]";
					goto triangle;
				}

			}
			if (trimenu == 2) {
				system("CLS");
				cout << "\t\t[-]Введите высоту треугольника: \n";
				cin >> high;
				if (high < 0) {
					cout << "\t\t[!!!]Вы ввели неверное значение высоты[!!!]";
					goto triangle;
				}
				cout << "\t\t[-]Введите длину основания треугольника \n";
				cin >> osnova;
				if (osnova < 0) {
					cout << "[!!!]Вы ввели неверное значение основания[!!!]";
					goto triangle;
				}

			}
			if (trimenu == 3) {
				system("CLS");
				cout << "\t\t[-]Введите высоту треугольника: \n";
				cin >> high;
				if (high < 0) {
					cout << "\t\t[!!!]Вы ввели неверное значение высоты[!!!]";
					goto triangle;
				}
				cout << "\t\t[-]Введите длину основания треугольника \n";
				cin >> osnova;
				if (osnova < 0) {
					cout << "[!!!]Вы ввели неверное значение основания[!!!]";
					goto triangle;
				}

			}
			switch (trimenu) {
			case 1: {
				char symbol = '*';
				triangle(symbol, high, osnova);
				
				goto globalmenu;
				break;
			}
			case 2: {
				char symbol = '#';
				triangle(symbol, high, osnova);
				
				goto globalmenu;
				break;
			}
			case 3: {
				char symbol = '@';
				triangle(symbol, high, osnova);
				
				goto globalmenu;
				break;
			}
			}
		}
	}
	case 3: {
		system("cls");
		int x, y, i, j;
		cout << "Введите ширину: ";
		cin >> x;
		cout << "Введите  высоту: ";
		cin >> y;
		for (i = 1; i <= x; i++)
			cout << "*";
		cout << endl;
		for (j = 1; j <= y - 2; j++)
		{
			cout << "*";
			for (i = 1; i <= x - 2; i++)
				cout << " ";
			cout << "*" << endl;
		}
		for (i = 1; i <= x; i++)
			cout << "*";
		cout << endl;
	}
	case 4: {
		if (GLOBALMENU == 4) {
			system("CLS");
			int kalkmenu = 0;

		kalk:
			cout << "------------------------------------------------------------\n";
			cout << "\t\t[+][-]Вы запустили калькулятор![*][/]      |\n";
			cout << "------------------------------------------------------------\n";
			cout << "\t\t[][][]Список доступных действий:[][][]     |\n";
			cout << "------------------------------------------------------------\n";
			cout << "\t\t[1] Сложение двух или более чисел          |\n";
			cout << "------------------------------------------------------------\n";
			cout << "\t\t[2] Вычитание двух или более чисел         |\n";
			cout << "------------------------------------------------------------\n";
			cout << "\t\t[3] Умножение двух или более чисел         |\n";
			cout << "------------------------------------------------------------\n";
			cout << "\t\t[4] Деление двух или более чисел           |\n";       
			cout << "------------------------------------------------------------\n";
			cout << "\t\t[5] Деление c остатком двух или более чисел|\n";
			cout << "------------------------------------------------------------\n";
			cout << "\t\t[6] Вернуться назад в главное меню         |\n";
			cout << "------------------------------------------------------------\n";
			cin >> kalkmenu;
			switch (kalkmenu) {
			case 1: {
				if (kalkmenu == 1) {
					float a = 0;
					float b = 0;
					int prod = 0;

				kalksum:
					system("cls");
					cout << "\t\t[-]Введите первое число\n";
					cin >> a;
					cout << "\t\t[-]Введите второе число\n";
					cin >> b;
					float numd = a + b;
					cout << "\t\t[-]Результат: " << numd << endl;
					cout << "\t\t[-]Хотите продолжить действия?\n";
					cout << "\t\t[1] - Да || [2] - Нет\n";
					cout << " Введите и нажмите Enter:  ";
					cin >> prod;
					if (prod == 1) {
						system("cls");
						goto kalksum;


					}
					if (prod == 2) {
						system("cls");
						goto kalk;
					}

				}
			}
			case 2: {
				if (kalkmenu == 2) {
					float a = 0;
					float b = 0;
					int prod = 0;
				kalkmin:
					system("CLS");

					cout << "\t\t[-]Введите первое число\n";
					cin >> a;
					cout << "\t\t[-]Введите второе число\n";
					cin >> b;
					float numd = a - b;
					cout << "\t\t[-]Результат: " << numd << endl;
					cout << "\t\t[-]Хотите продолжить действия?\n";
					cout << "\t\t[1] - Да || [2] - Нет\n";
					cout << " Введите и нажмите Enter:  ";
					cin >> prod;
					if (prod == 1) {
						system("CLS");
						goto kalkmin;
					}
					if (prod == 2) {
						system("cls");
						goto kalk;
					}

				}
			}

			case 3: {
				if (kalkmenu == 3) {

					int a = 0;
					int b = 0;
					int prod = 0;
				kalkmulti:
					system("CLS");
					cout << "\t\t[-]Введите первое число\n";
					cin >> a;
					cout << "\t\t[-]Введите второе число\n";
					cin >> b;
					float numd = a * b;
					cout << "\t\t[-]Результат: " << numd << endl;
					cout << "\t\t[-]Хотите продолжить действия?\n";
					cout << "\t\t[1] - Да || [2] - Нет\n";
					cout << " Введите и нажмите Enter:  ";
					cin >> prod;
					if (prod == 1) {
						system("CLS");
						goto kalkmulti;

					}
					if (prod == 2) {
						system("cls");
						goto kalk;
					}

				}


			}
			case 4: {
				if (kalkmenu == 4) {
					int a = 0;
					int b = 0;
					int prod = 0;
				kalkdiv:
					system("cls");
					cout << "\t\t[-]Введите первое число\n";
					cin >> a;
					cout << "\t\t[-]Введите второе число\n";
					cin >> b;
					double numd = a / b;
					cout << "\t\t[-]Результат: " << numd << endl;
					cout << "\t\t[-]Хотите продолжить действия?\n";
					cout << "\t\t[1] - Да || [2] - Нет\n";
					cout << " Введите и нажмите Enter:  ";
					cin >> prod;
					if (prod == 1) {
						system("CLS");
						goto kalkdiv;
					}
					if (prod == 2) {
						system("cls");
						goto kalk;
					}
				}

			}
			case 5: {
				if (kalkmenu == 5) {
					int a = 0;
					int b = 0;
					int prod = 0;
				kalkdivpr:
					system("CLS");
					cout << "\t\t[-]Введите первое число\n";
					cin >> a;
					cout << "\t\t[-]Введите второе число\n";
					cin >> b;
					double numd = a % b;
					cout << "\t\t[-]Результат: " << numd << endl;
					cout << "\t\t[-]Хотите продолжить действия?\n";
					cout << "\t\t[1] - Да || [2] - Нет\n";
					cout << " Введите и нажмите Enter:  ";
					cin >> prod;
					if (prod == 1) {
						system("cls");
						goto kalk;
					}
					if (prod == 2) {
						system("cls");
						goto kalk;
					}


				}
			}
			case 6: {
				if (kalkmenu == 6) {
					goto globalmenu;
				}
			}
			}
		}

	}
	case 5: {
		if (GLOBALMENU == 5) {
			system("CLS");
			int a = 1;
			int b = 2;
			int c = 3;
			int d = 4;
			int e = 5;
			int f = 6;
			int g = 7;
			int h = 8;
			int k = 9;
			int l = 10;

			char b1 = '!';
			char b2 = '@';
			char b3 = '$';
			char b4 = '%';
			char b5 = '^';
			char b6 = '&';
			char b7 = '?';
			char b8 = '*';
			char b9 = '(';
			char b10 = ')';

			float c1 = 0.1;
			float c2 = 0.2;
			float c3 = 0.3;
			float c4 = 0.4;
			float c5 = 0.5;
			float c6 = 0.6;
			float c7 = 0.7;
			float c8 = 0.8;
			float c9 = 1.9;
			float c10 = 0.9;

			double d1 = 1.2651;
			double d2 = 1.2551;
			double d3 = 1.2551;
			double d4 = 1.2561;
			double d5 = 1.2571;
			double d6 = 1.5451;
			double d7 = 1.2657;
			double d8 = 1.2761;
			double d9 = 1.2475;
			double d10 = 1.2231;

			bool e1 = true;
			bool e2 = false;
			bool e3 = true;
			bool e4 = false;
			bool e5 = true;
			bool e6 = false;
			bool e7 = true;
			bool e8 = false;
			bool e9 = true;
			bool e10 = false;

			long f1 = 182;
			long f2 = 1382;
			long f3 = 124812;
			long f4 = 121842;
			long f5 = 1128842;
			long f6 = 1128412;
			long f7 = 112742;
			long f8 = 116242;
			long f9 = 112542;
			long f10 = 112452;

			short g1 = -1;
			short g2 = -2;
			short g3 = -3;
			short g4 = -4;
			short g5 = -5;
			short g6 = -6;
			short g7 = -7;
			short g8 = -8;
			short g9 = -9;
			short g10 = -10;
			

			string h1 = "aboba";
			string h2 = "waga";
			string h3 = "wag";
			string h4 = "awga";
			string h5 = "abhrdhoba";
			string h6 = "abdrhrdhoba";
			string h7 = "tfu";
			string h8 = "awgawg";
			string h9 = "abyeryoba";
			string h10 = "ahwah";
			cout << "--------------------------------------\n";
			cout << "---------------INT---------------------\n";
			cout << "a - " << a << " Тип int размер 16 бит| \n";
			cout << "b - " << b << " Тип int размер 16 бит| \n";
			cout << "c - " << c << " Тип int размер 16 бит| \n";
			cout << "d - " << d << " Тип int размер 16 бит| \n";
			cout << "e - " << e << " Тип int размер 16 бит| \n";
			cout << "f - " << f << " Тип int размер 16 бит| \n";
			cout << "g - " << g << " Тип int размер 16 бит| \n";
			cout << "h - " << h << " Тип int размер 16 бит| \n";
			cout << "k - " << k << " Тип int размер 16 бит| \n";
			cout << "l - " << l << " Тип int размер 16 бит| \n";
			cout << "--------------------------------------\n";
			cout << "---------------CHAR---------------------\n";
			cout << "b1 - " << b1  <<  "Тип char размер 8бит|\n";
			cout << "b2 - " << b2 <<   "Тип char размер 8бит|\n";
			cout << "b3 - " << b3 <<   "Тип char размер 8бит|\n";
			cout << "b4 - " << b4 <<   "Тип char размер 8бит|\n";
			cout << "b5 - " << b5 <<   "Тип char размер 8бит|\n";
			cout << "b6 - " << b6 <<   "Тип char размер 8бит|\n";
			cout << "b7 - " << b7 <<   "Тип char размер 8бит|\n";
			cout << "b8 - " << b8 <<   "Тип char размер 8бит|\n";
			cout << "b9 - " << b9 <<   "Тип char размер 8бит|\n";	
			cout << "b10 - " << b10 << "Тип char размер 8бит|\n";
			cout << "--------------------------------------\n";
			cout << "---------------FLOAT------------------\n";
			cout << "c1 - " << c1 << "   Тип float размер 32 бита|\n";
			cout << "c2 - " << c2 << "   Тип float размер 32 бита|\n";
			cout << "c3 - " << c3 << "   Тип float размер 32 бита|\n";
			cout << "c4 - " << c4 << "   Тип float размер 32 бита|\n";
			cout << "c5 - " << c5 << "   Тип float размер 32 бита|\n";
			cout << "c6 - " << c6 << "   Тип float размер 32 бита|\n";
			cout << "c7 - " << c7 << "   Тип float размер 32 бита|\n";
			cout << "c8 - " << c8 << "   Тип float размер 32 бита|\n";
			cout << "c9 - " << c9 << "   Тип float размер 32 бита|\n";
			cout << "c10 - " << c10 << " Тип float размер 32 бита|\n";
			cout << "--------------------------------------\n";
			cout << "---------------DOUBLE-----------------\n";
			cout << "d1 - " << d1 << "   Тип double размер 64 бита|\n";
			cout << "d2 - " << d2 << "   Тип double размер 64 бита|\n";
			cout << "d3 - " << d3 << "   Тип double размер 64 бита|\n";
			cout << "d4 - " << d4 << "   Тип double размер 64 бита|\n";
			cout << "d5 - " << d5 << "   Тип double размер 64 бита|\n";
			cout << "d6 - " << d6 << "   Тип double размер 64 бита|\n";
			cout << "d7 - " << d7 << "   Тип double размер 64 бита|\n";
			cout << "d8 - " << d8 << "   Тип double размер 64 бита|\n";
			cout << "d9 -  " << d9 << "   Тип double размер 64 бита|\n";
			cout << "d10 - " << d10 << " Тип double размер 64 бита|\n";
			cout << "--------------------------------------\n";
			cout << "---------------BOOL-----------------\n";
			cout << "e1 - " << e1 << "(true)" <<   "Тип Bool Размер ???|\n" ;
			cout << "e2 - " << e2 << "(false)"  "Тип Bool Размер ???|\n";
			cout << "e3 - " << e3 << "(true)"  "Тип Bool Размер ???|\n";
			cout << "e4 - " << e4 << "(false)"  "Тип Bool Размер ???|\n";
			cout << "e5 - " << e5 <<   "(true)" "Тип Bool Размер ???|\n";
			cout << "e6 - " << e6 << "(false)"  "Тип Bool Размер ???|\n";
			cout << "e7 - " << e7 <<  "(true)" "Тип Bool Размер ???|\n";
			cout << "e8 - " << e8 << "(false)"  "Тип Bool Размер ???|\n";
			cout << "e9 - " << e9 <<  "(true)" "Тип Bool Размер ???|\n";
			cout << "e10 - " << e10 << "(false)" "Тип Bool Размер ???|\n";
			cout << "--------------------------------------\n";
			cout << "---------------LONG-----------------\n";
			cout << "f1 -" << f1 << "Тип Long размер 32 бита|\n";
			cout << "f2 -" << f2 << "Тип Long размер 32 бита|\n";
			cout << "f3 -" << f3 << "Тип Long размер 32 бита|\n";
			cout << "f4 -" << f4 << "Тип Long размер 32 бита|\n";
			cout << "f5 -" << f5 << "Тип Long размер 32 бита|\n";
			cout << "f6 -" << f6 << "Тип Long размер 32 бита|\n";
			cout << "f7 -" << f7 << "Тип Long размер 32 бита|\n";
			cout << "f8 -" << f8 << "Тип Long размер 32 бита|\n";
			cout << "f9 -" << f9 << "Тип Long размер 32 бита|\n";
			cout << "f10 -" << f10 << "Тип Long размер 32 бита|\n";
			cout << "--------------------------------------\n";
			cout << "---------------SHORT-----------------\n";
			cout << "g1 - " << g1 << "Тип short размер 16 бит|\n";
			cout << "g2 - " << g2 << "Тип short размер 16 бит|\n";
			cout << "g3 - " << g3 << "Тип short размер 16 бит|\n";
			cout << "g4 - " << g4 << "Тип short размер 16 бит|\n";
			cout << "g5 - " << g5 << "Тип short размер 16 бит|\n";
			cout << "g6 - " << g6 << "Тип short размер 16 бит|\n";
			cout << "g7 - " << g7 << "Тип short размер 16 бит|\n";
			cout << "g8 - " << g8 << "Тип short размер 16 бит|\n";
			cout << "g9 - " << g9 << "Тип short размер 16 бит|\n";
			cout << "g10 - " << g10 << "Тип short размер 16 бит|\n";
			cout << "--------------------------------------\n";
			cout << "---------------STRING-----------------\n";
			cout << 

			system("pause");
			goto globalmenu;
		}
	}
	case 6: {
	mnthday:
		system("cls");
		
		cout << "Календарь\n";
		cout << "Выберите сегодняшний месяц.\n";
		cout << "[1] - Январь\n [2] Февраль\n [3] Март\n [4] Апрель\n [5] Май\n [6] Июнь\n [7] Июль\n [8] Август\n [9] Сентябрь\n [10] Октябрь\n [11] Ноябрь\n [12] Декабрь\n ";
		cout << "Выберите месяц введя число: \n";
		cout << "Примечание не вводите название месяца или символы! это может вызвать некорректную работы приложения!\n";
		int mounth;
		int day;
		
		cin >> mounth;
		if (mounth > 12) {
			cout << "Вы ввели некоректное число: \n";
			system("pause");
			goto mnthday;
		}
		if (mounth == 1) {
			cout << "[1] Январь\n ";
			cout << "Сегодняшнее число: ";
			cin >> day; 
			if (day > 31) {
				cout << "Вы ввели некорректное число!";
				system("pause");
				goto mnthday;
			}
		    cout << "Месяц -" <<  mounth << " Число -" << day << endl;
		   
		}
		if (mounth == 2) {
			cout << "[2] Февраль\n ";
			cout << "Сегодняшнее число: ";
			cin >> day;
			if (day > 31) {
				cout << "Вы ввели некорректное число!";
				system("pause");
				goto mnthday;
			}
			
			cout << "Месяц -" << mounth << " Число -" << day << endl;
		}
		if (mounth == 3) {
			cout << "[3] Март\n ";
			cout << "Сегодняшнее число: ";
			cin >> day;
			if (day > 31) {
				cout << "Вы ввели некорректное число!";
				system("pause");
				goto mnthday;
			}
				
			cout << "Месяц -" << mounth << " Число -" << day << endl;
		}
		if (mounth == 4) {
			cout << "[4] Апрель\n ";
			cout << "Сегодняшнее число: ";
			cin >> day;
			if (day > 31) {
				cout << "Вы ввели некорректное число!";
				system("pause");
				goto mnthday;
			}
				
			cout << "Месяц -" << mounth << " Число -" << day << endl;
		}
		if (mounth == 5) {
			cout << "[5] Май\n ";
			cout << "Сегодняшнее число: ";
			cin >> day;
			if (day > 31) {
				cout << "Вы ввели некорректное число!";
				system("pause");
				goto mnthday;
			}
				
			cout << "Месяц -" << mounth << " Число -" << day << endl;
		}
		if (mounth == 6) {
			cout << "[6] Июнь\n ";
			cout << "Сегодняшнее число: ";
			cin >> day;
			if (day > 31) {
				cout << "Вы ввели некорректное число!";
				system("pause");
				goto mnthday;
			}
				
			cout << "Месяц -" << mounth << " Число -" << day << endl;
		}
		if (mounth == 7) {
			cout << "[7] Июль\n ";
			cout << "Сегодняшнее число: ";
			cin >> day;
			if (day > 31) {
				cout << "Вы ввели некорректное число!";
				system("pause");
				goto mnthday;
			}
				
			cout << "Месяц -" << mounth << " Число -" << day << endl;
		}
		if (mounth == 8) {
			cout << "[8] Август\n ";
			cout << "Сегодняшнее число: ";
			cin >> day;
			if (day > 31) {
				cout << "Вы ввели некорректное число!";
				system("pause");
				goto mnthday;
			}
				
			cout << "Месяц -" << mounth << " Число -" << day << endl;
		}
		if (mounth == 9) {
			cout << "[9] Сентябрь\n ";
			cout << "Сегодняшнее число: ";
			cin >> day;
			if (day > 31) {
				cout << "Вы ввели некорректное число!";
				system("pause");
				goto mnthday;
			}
				
			cout << "Месяц -" << mounth << " Число -" << day << endl;
		}
		if (mounth == 10) {
			cout << "[10] Октябрь\n ";
			cout << "Сегодняшнее число: ";
			cin >> day;
			if (day > 31) {
				cout << "Вы ввели некорректное число!";
				system("pause");
				goto mnthday;
			}
				
			cout << "Месяц -" << mounth << " Число -" << day << endl;
		}
		if (mounth == 11) {
			cout << "[11] Ноябрь\n ";
			cout << "Сегодняшнее число: ";
			cin >> day;
			if (day > 31) {
				cout << "Вы ввели некорректное число!";
				system("pause");
				goto mnthday;
			}
				
			cout << "Месяц -" << mounth << " Число -" << day << endl;
		}
		if (mounth == 12) {
			cout << "[12] Декабрь\n ";
			cout << "Сегодняшнее число: ";
			cin >> day;
			if (day > 31) {
				cout << "Вы ввели некорректное число!";
				system("pause");
				goto mnthday;
			}
				
			cout << "Месяц -" << mounth << " Число -" << day << endl;
		}
		system("pause");
		goto globalmenu;
	}
	case 7: {
		system("cls");
		int size;
		cout << "[ ] Размер решетки: ";
		cin >> size;

		char texture = '#';
		

		for (int y = 0; y < size; y++) {
			for (int x = 0; x < size; x++) {
				if (x % 2 == 0 || y % 2 == 0) {
					cout << texture  << " ";
				}
				else {
					cout << " ";
				}
			}
			cout << endl;
		}
		system("pause");
	}
	
	case 8: {

		system("cls");
		cout << "[ ] Размер крестика: ";
		int size;
		cin >> size;
		char texture = '-';
		
		for (int y = 0; y < size; y++) {
			for (int x = 0; x < size; x++) {
				if (x == y || size - x == y + 1) {
					cout << texture << " ";
				}
				else {
					cout << " ";
				}
			}
			cout << endl;
		}
		system("pause");
		goto globalmenu;
	}

	case 9: {
		system("CLS");
		int x = 0;
		int y = 0;
		cout << "Введите кол-во жжелаемых символом по оси X\n";
		cin >> x;
		cout << "Введите кол-во жжелаемых символом по оси Y\n";
		cin >> y;
		for (int i = 0;i < x;++i)
		{
			for (int j =0;j < y;++j)
			{
				if (i == x/2 || j == y/2)
					cout << '*';
				else cout << ' ';
			}
			
			cout << endl;
		}
		system("pause");
	}


	case 10: {
		system("cls");
		int a;
	Maze:
		system("cls");
		cout << "Вы зашли в игру THE MAZE\n";
		cout << "Выберите сложность\n";
		cout << "[1] Easy - \n";
		cout << "[2] Medium - \n";
		cout << "[3] Hard - \n";
		cout << "[4]Выход - \n";
		cout << "Введите число: ";

		cin >> a;
		if (a == 1) {
			system("cls");
			int labirint1[15][15] = {
			{0, 0, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,},
			{0, 0, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,},
			{0, 0, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,},
			{0, 0, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,},
			{0, 0, 0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,},
			{0, 0, 0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,},
			{0, 0, 1, 1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1,},
			{0, 0, 1, 1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1,},
			{0, 0, 1, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0,},
			{0, 0, 1, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0,},
			{0, 0, 1, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0,},
			{0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0,},
			{0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0,},
			{0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,},
			{0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,}
			};

			for (int i = 0; i < 15; i++) {
				for (int j = 0; j < 15; j++) {
					if (labirint1[i][j] == 1)
						cout << " ";
					else if (labirint1[i][j] == 0) {
						cout << "#";
					}
				}
				cout << endl;
			}
			system("Pause");
			goto Maze;
		}
		else if (a == 2) {
			system("cls");
			int labirint1[20][20] = {
			{0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0},
            {0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 1, 1, 1, 0, 1, 0, 1, 1, 1, 0},
            {0, 0, 0, 0, 0, 1, 0, 1, 0, 0, 0, 0, 1, 0, 1, 0, 1, 0, 1, 0},
            {0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0, 1, 0, 1, 0, 0, 0, 1, 0},
            {0, 0, 0, 0, 0, 1, 0, 1, 0, 0, 0, 0, 1, 0, 1, 1, 0, 0, 1, 0},
            {0, 0, 0, 0, 0, 1, 0, 1, 0, 0, 1, 0, 1, 0, 0, 1, 1, 1, 1, 0},
            {0, 0, 1, 1, 1, 1, 0, 1, 1, 1, 1, 0, 1, 0, 0, 1, 0, 1, 0, 0},
            {0, 0, 1, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 1, 0, 1, 0, 0},
            {0, 0, 1, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 1, 0, 0},
            {0, 0, 1, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0},
            {0, 0, 1, 0, 1, 0, 1, 0, 1, 1, 1, 1, 0, 0, 0, 1, 0, 1, 1, 0},
            {0, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 0, 1, 1, 1, 0, 1, 0, 0},
            {0, 1, 0, 0, 0, 1, 0, 1, 0, 0, 0, 1, 0, 0, 0, 1, 0, 1, 0, 0},
            {0, 1, 0, 1, 0, 1, 0, 1, 1, 1, 0, 1, 0, 0, 0, 1, 0, 1, 0, 0},
            {0, 1, 0, 1, 0, 0, 0, 1, 0, 1, 0, 1, 0, 1, 0, 1, 1, 1, 0, 0},
            {0, 1, 0, 1, 0, 1, 0, 1, 0, 0, 0, 1, 0, 1, 0, 0, 0, 1, 0, 0},
            {0, 1, 1, 1, 0, 1, 0, 1, 1, 1, 1, 1, 0, 1, 0, 1, 0, 1, 0, 0},
            {0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 1, 0, 1, 0, 1, 0, 1, 0, 0},
            {0, 0, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 0, 1, 1, 1, 1, 1, 0, 0},
			{0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0},
			};

			for (int i = 0; i < 20; i++) {
				for (int j = 0; j < 20; j++) {
					if (labirint1[i][j] == 1)
						cout << " ";
					else if (labirint1[i][j] == 0) {
						cout << "#";
					}
				}
				cout  << endl;
			}
			goto Maze;
		}
		else if (a == 3) {
			system("cls");
			int labirint1[30][30] = {
			
			{0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0,},
			{0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 1, 0,},
			{0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 1, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 0,},
			{0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0,},
			{0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 1, 0, 0, 0, 0, 1, 0,},
			{0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 1, 0, 0, 1, 1, 1, 1, 0, 1, 0, 0, 0, 0, 1, 0,},
			{0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 1, 0, 0, 0, 0, 1, 0,},
			{0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 1, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 1, 0, 0, 0, 0, 1, 0,},
			{0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 1, 0, 0, 0, 0, 0, 1, 0, 1, 0, 0, 1, 1, 1, 0,},
			{0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 0, 1, 1, 0, 1, 0, 0, 0,},
			{0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 1, 0, 0, 0,},
			{0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 0, 1, 0, 1, 0, 0, 0,},
			{0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 1, 0, 1, 0, 0, 0,},
			{0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 0, 1, 0, 1, 0, 0, 0,},
			{0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 1, 0, 1, 0, 1, 0, 0, 0,},
			{0, 0, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 1, 0, 1, 0, 1, 0, 0, 0,},
			{0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 0, 0, 1, 0, 1, 0, 1, 0, 0, 0,},
			{0, 0, 1, 0, 1, 0, 0, 1, 0, 0, 1, 0, 0, 0, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 1, 0, 1, 0, 0, 0,},
			{0, 0, 1, 0, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 0, 1, 0, 0, 1, 0, 0, 1, 0, 1, 0, 1, 0, 0, 0,},
			{0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 1, 0, 1, 0, 0, 1, 0, 0, 1, 0, 1, 0, 1, 0, 0, 0,},
			{0, 0, 1, 1, 1, 1, 1, 1, 1, 0, 1, 0, 0, 0, 1, 0, 1, 0, 0, 1, 0, 0, 1, 0, 1, 0, 1, 0, 0, 0,},
			{0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 1, 0, 0, 0, 1, 0, 1, 1, 0, 1, 0, 0, 1, 0, 1, 0, 1, 1, 1, 0,},
			{0, 0, 1, 1, 1, 1, 0, 0, 1, 0, 1, 0, 0, 0, 1, 0, 0, 1, 0, 1, 0, 0, 1, 0, 1, 0, 0, 0, 1, 0,},
			{0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 1, 0, 0, 0, 1, 0, 0, 1, 0, 1, 0, 0, 1, 0, 1, 0, 0, 0, 1, 0,},
			{0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 1, 0, 0, 0, 1, 1, 1, 1, 0, 1, 0, 0, 1, 0, 1, 0, 0, 0, 1, 0,},
			{0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 1, 0, 0, 0, 1, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0,},
			{0, 0, 1, 0, 0, 1, 1, 1, 1, 0, 1, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0,},
			{0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 1, 1, 1, 1, 1, 1, 0, 0, 0, 1, 0, 0, 1, 0, 0, 0,},
			{1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 0,},
			{0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,},
			};

			for (int i = 0; i < 30; i++) {
				for (int j = 0; j < 30; j++) {
					if (labirint1[i][j] == 1)
						cout << " ";
					else if (labirint1[i][j] == 0) {
						cout << "#";
					}
				}
				cout << endl;
			}
			goto Maze;
		}
		else if (a == 4) {
		system("cls");
		goto globalmenu;

     }
	 if (a > 4) {
		 cout << "вы ввели некорректное значение\n";
		 system("pause");
		 goto Maze;
		 
	 }
	}
	case 11: {
		cout << "Work in progress";
	}
	case 12: {
		int color = 0;
		cout << " Здесь вы можете выбрать только цвет ФОНА и ТЕКСТА";
		cout << "[1]";
		cout << "[2]";
		cout << "[3]";
		cout << "[4]";
		cout << "[5]";
		cout << "[6]";
		cin >> color;
		if (color == 1) {
			system("color 20");
		}
		
	}
	case 13: {
		if (GLOBALMENU == 13) {
           exit (0);
		}
		exit(0);
	 }
	}
	return 0;
}
