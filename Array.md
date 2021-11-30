# Arrays on Golang

What are Arrays?
An array is a collection of data stored in a variable with a predefined value.

In the programming language, golang arrays must use the same data type, if the data in the array contains a string, then the other data array elements also use the string data type.

Arrays use an indexing label. And it should be noted that the array starts from data to 0.

## How to create an array in Golang

```golang
var color [3]string
var color = make([]string,3)
var color[...]string{}
```
The colon (…) means that it can accommodate any number of elements in the array. It should be noted that if we use […] then the elements in it must also be filled in.

```golang
package main

import "fmt"

func main() {
  var color[3]string

  <!-- Filling Array -->
  var color[0] = "red"
  var color[1] = "blue"
  var color[2] = "green",
  var color[3] = "yellow"

  <!-- Displaying Arrays -->
  fmt.Println(color[0], color[1], color[2], color[3])

  <!-- Using For Range -->
  for i, v := color range {
    fmt.Println("Color to ", i, "=>", v)
  }
  <!-- Using Normal For -->
  for index := 0; index < len(color); index++ {
    fmt.Println("Color to ", index, "=>", color[index])
  }
  <!-- Deleting Arrays -->
  color[len(color)-1] = "" // remove the last element

  <!-- Using Multi-dimensional Arrays -->
  fmt.Println("Multi-Dimensional Array")
  var number = [5][2]int{{0, 0}, {2, 2}, {3, 4}, {5, 6}, {7, 8}}

  for i := 0; i < 5; i++ {
    for j := 0; j < 2; j++ {
      fmt.Printf("Data to [%d][%d] = %d\n", i, j, number[i][j])
    }
  }
}
```

[Indonesia]

# Array pada Golang

Apa itu Array ?
Array adalah kumpulan data yang di simpan dalam suatu variable dengan nilai yang sudah di tetapkan.

Dalam bahasa program golang array harus menggunakan tipe data yang sama, apabila data yang ada di dalam array terdapat string maka data element array lainnya juga menggunakan tipe data string.

Array menggunakan sebuah label pengindekan. Dan perlu di perhatikan array di mulai dari data ke 0.

## Cara membuat array pada Golang

```golang
var warna [3]string
var warna = make([]string,3)
var warna[...]string{}
```
Tanda titik tiga(…) artinya dapat menampung berapapun jumlah element yang ada di array. Perlu di ketahu jika kita menggunakan […] maka element di dalam nya harus juga di isi.

```golang
package main

import "fmt"

func main() {
	var warna[3]string
  
  <!--  Mengisi Array  -->
	var warna[0] = "merah"
	var warna[1] = "biru"
	var warna[2] = "hijau",
	var warna[3] = "kuning"
  
  <!--  Menampilkan Array  -->
  fmt.Println(warna[0], warna[1], warna[2], warna[3])
  
  <!--  Menggunakan For Range  -->
  for i, v := range warna {
		fmt.Println("Warna ke ", i, "=>", v)
	}
  <!--  Menggunakan For Biasa  -->
  for index := 0; index < len(warna); index++ {
		fmt.Println("Warna ke ", index, "=>", warna[index])
	}
  <!--  Menghapus Array  -->
  warna[len(warna)-1] = ""    // menghapus element paling belakang
  
  <!--  Menggunakan Array Multi dimensi  -->
  fmt.Println("Array Multi Dimensi")
	var angka = [5][2]int{{0, 0}, {2, 2}, {3, 4}, {5, 6}, {7, 8}}

	for i := 0; i < 5; i++ {
		for j := 0; j < 2; j++ {
			fmt.Printf("Data ke [%d][%d] = %d\n", i, j, angka[i][j])
		}
	}

}
```
