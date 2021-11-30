# Slice on Golang

What is Slice?
Slice is one of the functions in golang whose function is similar to arrays, but the difference is that by using slices we don't need to define the number / length of the array.

It can be said that slice is a more dynamic array.

Then what is the better array of slices?

It all depends on our data needs, when our data is static, we can use arrays, while if the data is mutable, we recommend using slices.

In arrays, you can also not define the number of arrays and replace them with a three dot (...) but directly give the data value while in the slice it is not necessary.

## Making Slices

```golang
var student[]string
var student []string{"Endy","Olivia"}
```

## Filling Slice
```golang
student = []string{"Endy", "Olivia"}
```

## Display Data
```golang
package main

import "fmt"

func main() {
  var student[]string
  student = []string{"Endy", "Olivia"}
  
  <!-- Method 1 -->
  fmt.Println("Student Data => ", student)
  
  <!-- Method 2 -->
  fmt.Println("Student Data 0 to 1 => ", student[0:1])
  fmt.Println("Student Data 0 to 2 => ", student[0:2])
  <!-- Then the result will display the array 0 to 1 and 0 to 2. -->
  
  <!-- Displays the amount of data -->
  
  <!-- Copy values -->
  fmt.Println("The number of students is => ", len((student)))
  
  human := make([]string, len(student))

  copy(human, student)
  fmt.Println(human)
  <!-- The contents of the human and student arrays are the same -->
  
  <!-- Adding Elements -->
  new student := "Daffa"
  student := append(student, new student)
  fmt.Println(student)
}
```

[Indonesia]

# Slice pada Golang

Apa itu Slice ?
Slice salah satu fungsi di golang yang fungsinya mirip dengan array, namun yang membedakan dengan menggunakan slice kita tidak perlu mendefinisikan jumlah / panjang array.

Bisa di katakan bahwa slice adalah array yang lebih dinamis / dinamic array.

Lalu lebih baik array apa slice ?

Semua tergantung pada kebutuhan data kita, ketika data kita bersifat tetap / static dapat menggunakan array sedangkan jika datanya bisa berubah maka sebaiknya menggunakan slice.

Pada array juga bisa tidak medefinisikan jumlah array dan mengganti dengan tanda titik tiga (…) namun langsung di berikan nilai data sedangkan di slice tidak perlu.

## Membuat Slice

```golang
var mahasiswa []string
var mahasiswa []string{"Endy","Olivia"}
```

## Mengisi Slice
```golang
mahasiswa = []string{"Endy", "Olivia"}
```

## Menampilkan Data
```golang
package main

import (
	"fmt"
)

func main() {
	var mahasiswa []string
	mahasiswa = []string{"Endy", "Olivia"}
  
  <!--  Cara 1  -->
	fmt.Println("Data Mahasiswa => ", mahasiswa)
  
  <!--  Cara 2  -->
  fmt.Println("Data Mahasiswa ke 0 sampai 1 => ", mahasiswa[0:1])
	fmt.Println("Data Mahasiswa ke 0 sampai 2 => ", mahasiswa[0:2])
  <!--  Maka hasilnya akan menampilkan array ke 0 sampai 1 dan 0 sampai ke 2.  -->
  
  <!--  Menampilkan jumlah data  -->
  
  <!--  Menyalin nilai  -->
  fmt.Println("Jumlah Mahasiswanya adalah => ", len((mahasiswa)))
  
	manusia := make([]string, len(mahasiswa))

	copy(manusia, mahasiswa)
	fmt.Println(manusia)
  <!--  Isi dari array manusia dan mahasiswa sama  -->
  
  <!--  Menambah Element  -->
  mahasiswabaru := "Daffa"
  mahasiswa := append(mahasiswa,mahasiswabaru)
  fmt.Println(mahasiswa)
}
```
