# Matriz
en el comentario se encuentra el codigo.
#include<iostream>
#include<math.h>
#include<time.h>

using namespace std;


void matriz();


int main(){
	matriz();
	cout << endl;
	system("pause");
}

void matriz(){
	srand(time(NULL));
	int matriz[5][4], fil = 0, col = 0, aux = 0;
	int n;
	cout << "La matriz original" << "\n";
	for (int fil = 0; fil < 5; fil++){
		for (int col = 0; col < 4; col++){
			matriz[fil][col] = rand() % 100;

		}
	}
	for (int fil = 0; fil < 5; fil++){
		cout << endl;
		for (int col = 0; col < 4; col++){
			cout << matriz[fil][col] << "\t";
		}
	}
	if (matriz[fil][col] % 2 == 0){
		for (int fil = 0; fil < 5; fil++){
			cout << endl;
			for (int col = 0; col < 4; col++){
			}
			cout << endl;
			cout << matriz[fil][col];
			cout << endl;
			cout << "Numero par " << "\n";
		}
		if (matriz[fil][col] % 3 == 0){
			for (int fil = 0; fil < 5; fil++){
				cout << endl;
				for (int col = 0; col < 4; col++){
				}
				cout << endl;
				cout << matriz[fil][col];
				cout << endl;
				cout << "Numero impar " << "\n";
			}
		}
	}
}
