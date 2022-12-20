# Ujian Akhir Semester

<br> Mata Kuliah : Dasar Pemrograman
<br> Nama        : Amanda Zulfa Salsabila
<br> NIM         : 1227050019
<br> Jurusan     : Teknik Informatika UIN Sunan Gunung Djati Bandung



# Deskripsi Umum

Tema utama dari source code yang satu ini adalah untuk membuat array 2 dimensi menggunakan bahasa C++.
Tujuan utama dari source code ini adalah mengubah letak nilai yang tadinya sebuah baris menjadi sebuah kolom, begitupun sebaliknya.
<br> Algoritma dari source code ini yaitu :
<br> 1. User menginputkan beberapa banyak baris pada array.
<br> 2. User menginputkan beberapa banayak kolom dari baris pada array.
<br> 3. User menginputkan satu persatu nilai array, dimulai dari baris 1 dan kolom 1
<br> 4. Jika sudah, nilai dalam array tersebut ditampilkan sesuai aturan matriks.
<br> 5. Lalu ditampilkan juga nilai dalam array yang sudah dibalik, dari baris menjadi kolom dan sebaliknya



# Source Code
#include <iostream>
using namespace std;

int main()
{
	int input [100][100];
	int baris, kolom, i, j;
	
	cout << "Imput jumlah baris : ";
	cin >> baris;
	cout << "Input jumlah kolom : ";
	cin >> kolom;
	cout << endl;
	
	for (i = 0; i < baris; i++){
		for (j = 0; j < kolom; j++){
			cout << "baris" << i+1 << ",kolom" << j+1 << " = ";
			cin >> input[i][j];
		}
		cout << endl;
	}
	
	cout << "Hasil : "<<endl;
	
	for (i = 0; i < baris; i++){
		for (j = 0; j < kolom; j++){
			cout << " " << input [i][j];
		}
		cout << endl;
	}
	
	cout << "=======================" << endl;
	
	for (i = 0; i < kolom; i++){
		for (j = 0; j < baris; j++){
			cout << " " << input[j][i];
		}
		cout << endl;
	}
	
}

	
# Output
