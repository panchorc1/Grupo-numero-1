// # Grupo-numero-1
// Actividades del grupo numero 1 de ingeniería en sistemas 
//Codificado por: sAfOrAs
//Código Fuente: Calcula cuantos números pares hay entre dos ingresados
#include<iostream>
using namespace std;
int main()
{
    int a=0,b=0,c=0;
    cout<<"ingrese un numero: ";cin>>a;
    cout<<"ingrese otro numero: ";cin>>b;
    while(a<=b)
    {
        if(a%2!=0)
        c=c+1; a=a+1;       
    }
    cout<<c<<endl;
    cin.ignore(); return 0;
}
