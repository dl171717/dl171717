#include <iostream>
#include <conio>
#include <math>
//Inician las funciones sin parametros
void acercade()
{
	clrscr();
	gotoxy(10,6);cout<<" Menu de operaciones aritmeticas haciendo uso de funciones sin parametros";
   gotoxy(10,7);cout<< " Creado por: Diego Alejandro Lemus";
}

void suma()
{
	clrscr();
   int num1, num2, Resultado;
   gotoxy(15,7);cout<<"Suma de dos numeros";
   gotoxy(15,8);cout<<"Formula: Numero1+9numero2 ";
   gotoxy(15,9);cout<<"Ingrese el primero numero: ";
   cin>>num1;
   gotoxy(15,10);cout<<"Ingrese el segundo numero: ";
   cin>>num2;
   Resultado=num1+num2;
   gotoxy(15,12);cout<<"El resultado de la operacion es: "<<Resultado;
   getch();
}

void resta()
{
	clrscr();
	int num1, num2, Resultado;
   gotoxy(15,7);cout<<"Resta de dos numeros";
   gotoxy(15,8);cout<<"Formula: Numero1-numero2 ";
   gotoxy(15,9);cout<<"Ingrese el primero numero: ";
   cin>>num1;
   gotoxy(15,10);cout<<"Ingrese el segundo numero: ";
   cin>>num2;
   Resultado=num1-num2;
   gotoxy(15,12);cout<<"El resultado de la operacion es: "<<Resultado;
   getch();
}

void multi()
{
	clrscr();
   int num1, num2, Resultado;
	gotoxy(15,7);cout<<"Multiplicacion de dos numeros";
   gotoxy(15,8);cout<<"Formula: Numero1*numero2 ";
   gotoxy(15,9);cout<<"Ingrese el primero numero: ";
   cin>>num1;
   gotoxy(15,10);cout<<"Ingrese el segundo numero: ";
   cin>>num2;
   Resultado=num1*num2;
   gotoxy(15,12);cout<<"El resultado de la operacion es: "<<Resultado;
   getch();
}

void divicion()
{
	clrscr();
	int num1, num2, Resultado;
  	gotoxy(15,7);cout<<"Divicion de dos numeros";
   gotoxy(15,8);cout<<"Formula: Numero1/numero2 ";
   gotoxy(15,9);cout<<"Ingrese el primero numero: ";
   cin>>num1;
   gotoxy(15,10);cout<<"Ingrese el segundo numero: ";
   cin>>num2;
   Resultado=num1/num2;
   gotoxy(15,12);cout<<"El resultado de la operacion es: "<<Resultado;
   getch();
}

void pote()
{
	clrscr();
	int num1, num2, Resultado;
   gotoxy(15,7);cout<<"Potencia de un numero";
   gotoxy(15,8);cout<<"Formula: Numero1^numero2 ";
   gotoxy(15,9);cout<<"Ingrese el primero numero: ";
   cin>>num1;
   gotoxy(15,10);cout<<"Ingrese el segundo numero: ";
   cin>>num2;
   Resultado=pow(num1,num2);
   gotoxy(15,12);cout<<"El resultado de la operacion es: "<<Resultado;
   getch();
   //inicia el menu
}
void main();
{
	int opcion;
	do
   {
		clrscr();
		gotoxy(10,5);cout << "Menú de opciones";
		gotoxy(10,6);cout << "1. Acerca De";
		gotoxy(10,7);cout << "2. Suma ";
		gotoxy(10,8);cout << "3. Resta ";
		gotoxy(10,9);cout << "4. Multiplicacion";
		gotoxy(10,10);cout <<"5. Divicion";
		gotoxy(10,11);cout << "6. Potenca";
		gotoxy(10,12);cout << "7. Salir";
		gotoxy(10,13);cout << "Ingrese su opción: ";
		cin >> opcion;
		switch (opcion)
		{
			case 1:
			{
         	clrscr();
				acercade();
				break;
			}
			case 2:
			{
         	clrscr();
				suma();
				break;
			}
			case 3:
			{
         	clrscr();
				resta();
				break;
			}
			case 4:
			{
            clrscr();
				multi();
				break;
			}
			case 5:
			{
            clrscr();
				divicion();
				break;
			}
			case 6:
			{
            clrscr();
				pote();
				break;
			}
			case 7:
			{
            clrscr();
				cout << "Gracias.";
				break;
			}
			default:
			{
				cout << "Opción inválida";
				break;
			}
		}
	} while (opcion != 7);
	return 0;
}
