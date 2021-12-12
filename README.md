# TUGAS-PRAKTEK-FUNGSI


// NO 2

#include <iostream>

  // itu abis include diatas dikasih iostream ya, sebenernya udh ditulis tapi gak tampil, gak tau lh tulis aja :) #SALAMDARIYGBUAT
  
#include<conio.h>
  
#include<math.h>

using namespace std;


int main()
{
  
  // MENCARI SIMPAN BAKU
	
	float S,Xi,X,N,hasil_N,hasil_XiX;
	float XiX1,XiX2,XiX3,XiX4,a,b;
	
	
	cout << "Simpan baku yang akan dihitung \t\t--> "; cin >> S;
	cout << "Data ke I dari N buah data \t\t--> "; cin >> X;
	cout << "Nilai rata-rata dari keseluruhan data \t--> "; cin >> Xi;
	cout << "Cacah data \t\t\t\t--> "; cin >> N;
	

	
	// MENCARI RATA2
	
	hasil_N = S + X + Xi + N;
	hasil_N /= 4;
	
	cout << "~~~~~~~~~~~~~~~~~~~~~~~~~~~~~" << endl;
	cout << "Rata - rata --> " << hasil_N << endl;
	
	// Xi - X
	a = S - hasil_N;
	XiX1 =  pow(a, 2);
	cout << "(" << S <<  " - " << hasil_N << ") = " << XiX1 << endl;
	
	a = X - hasil_N;
	XiX2 =  pow(a, 2);
	cout << "(" << X << " - " << hasil_N << ") = " << XiX2 << endl;
	
	a = Xi - hasil_N;
	XiX3 =  pow(a, 2);
	cout << "(" << Xi << " - " << hasil_N << ") = " << XiX3 << endl;
	
	a = N - hasil_N;
	XiX4 =  pow(a, 2);
	cout << "(" << N << " - " << hasil_N << ") = " << XiX4 << endl;
	
	hasil_XiX = XiX1 + XiX2 + XiX3 + XiX4;
	cout << "Hasil dari Xi-X --> " << hasil_XiX << endl;
	
	// MENCARI S
	b = sqrt(hasil_XiX);
	cout << "Hasil akar dari " << hasil_XiX << " --> " << b;
	
		
}
