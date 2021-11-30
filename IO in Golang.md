# Input Output in Golang

# Take input and display output on Golang

In this discussion, it will be brief, because it is almost similar to C language. For those who have studied it, it will be easy to follow today's lesson.

A program code in dealing with certain needs sometimes there are 3 sequential processes, namely Input, Process and Output.

1. Input is a value that we will enter later.
2. Process is Processing the results that are entered.
3. Output is a value of the result of the process.

## How to take input value

Golang already provides a function to retrieve an input value typed using the keyboard. There are 3 forms of input in Golang, namely:

1. Scan(), used for numeric values.
2. Scanf(), used for string values.
3. Scanln(), used for numeric values ​​at the end of the line.

Let's make a short program

```golang
package main

import "fmt"

func main() {
var name string
var a, b int
fmt.Println("Enter Your Name: ")
fmt.Scanf("%s", &name)
fmt.Println("Enter First Number: ")
fmt.Scanln(&a)
fmt.Println("Enter Second Number: ")
fmt.Scanln(&b)
}
```

## Display input result

```golang
package main

import "fmt"

func main() {
var name string
var a, b, result int
fmt.Println("Enter Your Name: ")
fmt.Scanf("%s", &name)
fmt.Println("Enter First Number: ")
fmt.Scan(&a)
fmt.Println("Enter Second Number: ")
fmt.Scan(&b)
  
result = a + b
  
fmt.Printf("Name => %s \n", name)
fmt.Printf("The sum (a + b) => %d + %d = %d \n", a, b, result)l)
}
```

Pay attention to the code above, there is a symbol for example "%s", So what is it for?

Symbol string format
- %v, for all data types with a string return value.
- %t, for data type boolean, TRUE or FALSE.
- %b, to display binary data, namely 0 and 1. For example, if you input an integer value, it will print the binary value of the integer.
- %c, , to display unicode data.
- %d, to display integer data with a maximum length of 10.
- %f, to display decimal data with float data type input.
- %s, to display string data.
- %t, to display the type of variable used.
- %%, to display the character %.

[Indonesia]

# Mengambil masukan dan menampilkan keluaran pada Golang

Pada pembahasan kali ini akan singkat saja, karena ini hampir mirip - mirip dengan bahasa C. Bagi yang sudah pernah memperlajari nya pasti mudah untuk mengikuti pelajaran hari ini.

Sebuah kode program dalam menangani kebutuhan tertentu ada kalanya terdapat 3 proses yang berurutan yaitu Input, Proses dan Output.

1. Input adalah sebuah nilai yang nantinya kita masukkan. 
2. Proses adalah Memproses hasil yang di masukkan.
3. Output adalah sebuah nilai hasil dari proses.

## Cara mengambil nilai input

Golang sudah menyediakan fungsi untuk mengambil sebuah nilai input yang diketikkan menggunakan keyboard. Ada 3 Bentuk Input pada Golang yaitu :

1. Scan(), digunakan untuk nilai angka.
2. Scanf(), digunakan untuk nilai string.
3. Scanln(), digunakan untuk nilai angka pada baris akhir.

Mari kita buat program singkatnya

```golang
package main

import "fmt"

func main() {
	var nama string
	var a, b int
	fmt.Println("Masukkan Nama Anda: ")
	fmt.Scanf("%s", &nama)
	fmt.Println("Masukkan Angka Pertama: ")
	fmt.Scanln(&a)
	fmt.Println("Masukkan Angka Kedua: ")
	fmt.Scanln(&b)
}
```

## Menampilkan hasil input

```golang
package main

import "fmt"

func main() {
	var nama string
	var a, b, hasil int
	fmt.Println("Masukkan Nama Anda: ")
	fmt.Scanf("%s", &nama)
	fmt.Println("Masukkan Angka Pertama: ")
	fmt.Scan(&a)
	fmt.Println("Masukkan Angka Kedua: ")
	fmt.Scan(&b)
  
  hasil = a + b
  
  fmt.Printf("Nama => %s \n", nama)
	fmt.Printf("Hasil penjumlahan (a + b) => %d + %d = %d \n", a, b, hasil)l)
}
```

Perrhatikan kode di atas, terdapat simbol contohnya “%s”, Nah itu buat apa ?

Format string Simbol
- %v, untuk semua tipe data dengan nilai kembalian string.
- %t, untuk tipe data boolean, TRUE atau FALSE.
- %b, untuk menampilkan data biner yaitu 0 dan 1. Misalnya input nilai integer maka akan di cetak nilai biner dari integer tersebut.
- %c, ,untuk menampilkan data unicode.
- %d, untuk menampilkan data integer dengan panjang maksimal 10.
- %f, untuk menampilkan data desimal dengan input tipe data float.
- %s, untuk menampilkan data string.
- %t, untuk menampilkan jenis variable yang digunakan.
- %%, untuk menampilkan karakter %.

