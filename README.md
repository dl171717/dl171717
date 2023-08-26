#include <iostream>
#include <conio>

int funsumar(int x, int y)
{
    return(x+y);
}

int funrestar(int x, int y)
{
    return(x-y);
}

int funmultiplicar(int x, int y)
{
    return(x*y);
}

int fundividir(int x, int y)
{
    return(x/y);
}

int main()
{
    int opcion;
    int num1, num2;
    int resultado;
{
    do
    {
    	clrscr();
      gotoxy(30,45);cout<<"/-/-/-/RETIROS/-/-/-/";
      gotoxy(5,5);cout<<"----------------";
      gotoxy(5,6);cout<<"- 1. Suma -";
      gotoxy(5,7);cout<<"----------------";

      gotoxy(30,5);cout<<"----------------";
      gotoxy(30,6);cout<<"- 2. resta -";
      gotoxy(30,7);cout<<"----------------";

      gotoxy(30,12);cout<<"---------------";
      gotoxy(30,13);cout<<"- 3. multiplicar -";
      gotoxy(30,14);cout<<"---------------";

      gotoxy(5,12);cout<<"---------------";
      gotoxy(5,13);cout<<"- 4. dividir -";
      gotoxy(5,14);cout<<"---------------";

      gotoxy(20,18);cout<<"-------------";
      gotoxy(20,17);cout<<"- 5. salir -";
      gotoxy(20,16);cout<<"-------------";

      gotoxy(11,9);cout<<"Seleccione un opcion: ";
      cin>>opcion;
      switch(opcion)
      {
      	case 1:
      {
         cout << "Ingrese dos numeros: ";
         cin >> num1 >> num2;
         resultado = funsumar(num1, num2);
         cout << "La suma es: " << resultado ;
         getch();
         break;
         }
            case 2:
         {
         	cout << "Ingrese dos numeros: ";
            cin >> num1 >> num2;
            resultado = funrestar(num1, num2);
            cout << "La resta es: " << resultado;
            getch();
            break;
         }
         case 3:
         {
         	cout << "Ingrese dos numeros: ";
         	cin >> num1 >> num2;
            resultado = funmultiplicar(num1, num2);
            cout << "La multiplicacion es: " << resultado ;
            getch();
            break;
         }
         case 4:
         {
         	cout << "Ingrese dos numeros: ";
            cin >> num1 >> num2;
            resultado = fundividir(num1, num2);
            cout << "La division es: " << resultado ;
            getch();
            break;
         }
         case 5:
         {
         	exit(0);
         }
         default:
         {
         cout << "Opcion invalida." ;
         getch();
        	}
    	} while (opcion != 5);
		getch();
