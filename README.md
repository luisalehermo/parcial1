/*1.- Elabore un programa que presente en pantalla los primeros veinte (20) números que:
a.- Que sean divisibles exactamente entre cuatro (4). (Sin parte decimal)
b.- Que sean divisibles exactamente entre seis (6). (Sin parte decimal)
c.- Que su raíz cuadrada de un numero entero (Sin parte decimal) y que ese número termine es cuatro (4).
El rango a revisar es desde 50000 hasta que consiga los veinte (20) números.
En la pantalla deberá presentarse el número, su división entre cuatro (4), su división entre seis (6)
 y la raíz cuadrada de ese resultado que termina en 4: 
Numero – División entre 4 – División entre 6 - Raíz Cuadrada terminada en 4
54756 – 13689 – 9126 - 234
El programa archivo .CPP deberá ser enviado al profesor al correo:
Cjferrer14@hotmail.com
En el cuerpo del correo debe aparecer el nombre del estudiante.
Programas idénticos serán evaluados con cero puntos.
El tiempo para ejecutar la actividad es de 1:45 minutos, por cada 5 minutos de retraso se le 
restara 4 puntos de la calificación al estudiante.

Éxito.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Programa elaborado por Luis Hernández C.I: 29.642.345
Universidad Santa María
Profesor: Carlos Ferrer
Programacion I 

Fecha de elaboracion: 12/04/2023
Revision #1 */

#include<iostream>
#include<math.h>
using namespace std;
main(){
	
	int i,cont; cont=0;
	//Cilo que va recorriendo los numeros que van desde 50.000 hasta encontrar los 20 primeros numeros que cumplan las 3 condiciones
	for(i=50000;cont<20;i++){
		if((i%4)==0){ //Numeros que sean exactamane divisbles entre 4
			if((i%6)==0){//Numeros que sean exactamente divisibles entre 6
				if(fmod(sqrt(i),10)==4){ //Numeros cuya raiz exacta termine en 4
					cont++;
					cout<<i<<"-"<<i/4<<"-"<<i/6<<"-"<<sqrt(i)<<endl;
				}
			}
		}
	}
	return 0;
}
