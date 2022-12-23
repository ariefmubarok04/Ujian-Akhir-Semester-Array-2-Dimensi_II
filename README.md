# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Arief Rahman Mubarok
<br>NIM		:	1227050026
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

Tema dari source code ini yaitu array 2 dimensi menggunakan bahasa c++.
Tujuan dari source code ini yaitu mengubah letak nilai yang pada awalnya sebuah baris angka menjadi sebuah kolom dan sebaliknya.
<br> Algoritma dari source code ini yaitu :
<br> 1. input berapa baris yang dinginkan pada array.
<br> 2. input berapa kolom yang diinginkan pada array.
<br> 3. input satu persatu nilai array pada masing masing baris dan kolom.
<br> 4. akan di tampilkan nilai yang sudah diinput sesuai aturan matriks.
<br> 5. ditampilkan juga nilai dalam array yang sudah diubah letaknya dari baris menjadi kolom dan sebaliknya.

## Source Code

```C++
  #include <iostream>
  using namespace std;

  int main() {
	int b,k;
	cout<<"masukan jumlah baris : ";
	cin>>b;
	cout<<"masukan jumlah kolom : ";
	cin>>k;
	cout<<endl;

	int array[b][k];
	for(int i=0; i<b; i++){
		for(int j=0; j<k; j++) {
			cout<<"baris ke "<<i+1<<" kolom ke "<<j+1<<" : ";
			cin>>array[i][j];
		}
	}
	cout<<"bentuk awal : "<<endl;
	for(int i=0; i<b; i++){
		for(int j=0; j<k; j++) {
			cout<<array[i][j]<<" ";
		}
		cout<<endl;
	}
	cout<<endl;
	cout<<"bentuk akhir : "<<endl;
	for(int i=0; i<k; i++){
		for(int j=0; j<b; j++) {
			cout<<array[j][i]<<" ";	
		}
		cout<<endl;
	}
  }
 ```

## Output
<img width="671" alt="buat uas 2" src="https://user-images.githubusercontent.com/118902896/209353702-96367761-d3c6-4517-b560-dde19b91635b.png">
