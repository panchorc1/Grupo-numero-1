#include <iostream>
#include <fstream>

using namespace std;

struct equipo{
	char nombre_equipo[40];
	char numero_de_integrnates[20];
	int num;
};
struct integrante_equipo{
	char nombre_integrantes[30];
	int edad[15];
};
struct equipoo{
	equipo datos_equipo;
	integrante_equipo datos_integrnate_equipo;
};
int main (){

		int a,b,c,d,e,opcion;
	equipo equipo_1;
	cout << "\n DATOS DEL EQUIPO \n Introduce el nombre\n";
	cin >> equipo_1.nombre_equipo;
	cout << "numero de integrantes\n";
	cin >> equipo_1.numero_de_integrnates;
	cout << "año de fundacion \n";
	cin >> equipo_1.num;
	cout << "\n DATOS DEL INTEGRANTE EQUIPO \n Introduce el nombre\n";
	cin >> equipo_1.nombre_equipo;
	cout << "edad \n";
	cin >> equipo_1.num;

	cout << "INFORMACION DEL EQUIPO\n";
	cout << "Nombre:... "<<equipo_1.nombre_equipo;
	cout << "\nNumero integrantes:..." <<equipo_1.numero_de_integrnates;
	cout << "\nAño de fundacion:...." <<equipo_1.num;
	cout << "\nNombre integrante:..." <<equipo_1.nombre_equipo;
	cout << "\nEdad:...." <<equipo_1.num;

	
		//CREAR ARCHIVO DE TEXTO
	ofstream archivo("equipo.txt", ios::app);
	//INGRESO TEXTO AL ARCHIVO
	 archivo << "equipo_1";
	 archivo << "equipo completo";
	 
	 archivo.close();
	 
	
	return 0;
}
