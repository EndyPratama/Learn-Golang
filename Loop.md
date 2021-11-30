# Loop on Golang

In the Golang program there are 3 types of iterations, namely:

- For
- While
- Range

3 The type of loop in golang uses the "for" function command and is followed by the type of loop used.

## For
The For loop is marked with a maximum value that is useful for defining how many times it will be repeated.
```golang
package main

import "fmt"

func main() {
  for i := 0; i < 10; i++ {
    fmt.Println("Loop to", i)
  }
}
```
## While
The while loop can also determine when the loop will stop. In fact, the while loop uses a condition operator, such as less than (<).
```golang
package main

import "fmt"

func main() {
  true := true
  i := 0

  for true {
    if i == 3 {
      true = false
    }
    fmt.Println("Number to", i)
    i++
  }
  <!-- When condition is true = false then exit the loop -->
  <!--  Contoh lainnya  -->
  var index = 0

  for index < 4 {
    fmt.Println("Number to", index)
    index++
  }
  <!-- when the index value is more than 4 exits the loop -->
  <!--   Contoh lainnya   -->
  var index = 0

  for index < 4 {
    fmt.Println("Number to", index)
    index++
    if index == 2 {
      break
    }
  }
  <!-- If index == 2 it will exit -->
}
```
## Range
The range loop is the same as the foreach loop in the PHP programming language. Looping this range must use data in the form of an array.
```golang
package main

import "fmt"

func main() {

  color := []string{"red", "blue","green", "yellow"}

  for index, v := color range {
    fmt.Println("Loop to", index, v)
  }
}
```
Because the array contains 4 data, only 4 loops will occur.

[Indonesia]

# Perulangan pada Golang

Di dalam program Golang terdapat 3 jenis perulangan yaitu :

- For 
- While
- Range

3 Jenis perulangan di golang menggunakan perintah fungsi “for” dan di ikuti oleh jenis perulangan yang digunakan.

## For
Perulangan For di tandai dengan sebauh nilai maksimal yang berguna untuk mendefinisikan berapa kali akan di ulang.
```golang
package main

import "fmt"

func main() {
	for i := 0; i < 10; i++ {
		fmt.Println("Perulangan ke", i)
	}
}
```
## While
Perulangan while juga dapat menentukan kapan perulangan akan berhenti.Sebenarnya perulangan dengan while menggunakan sebuah kondisi operator, seperti kurang dari (<).
```golang
package main

import "fmt"

func main() {
	benar := true
	i := 0

	for benar {
		if i == 3 {
			benar = false
		}
		fmt.Println("Angka ke", i)
		i++
	}
<!--  Saat kondisi benar = false maka keluar dari loop  -->
  var index = 0

	for index < 4 {
		fmt.Println("Angka ke", index)
		index++
	}
<!--  saat nilai index lebih dari 4 keluar loop  -->
var index = 0

	for index < 4 {

		fmt.Println("Angka ke", index)
		index++

		if index == 2 {
			break
		}
	}
<!--  Jika index == 2 maka akan keluar  -->
}
```
## Range
Perulangan range ini sama aja dengan perulangan foreach pada bahasa program PHP. Perulangan range ini harus menggunakan data yang berupa array.
```golang
package main

import "fmt"

func main() {

	warna := []string{"merah", "biru","hijau", "kuning"}

	for index, v := range warna {
		fmt.Println("Perulangan ke", index, v)
	}
}
```
Karena dalam array tersebut terdapat 4 data maka akan terjadi 4x looping saja.
