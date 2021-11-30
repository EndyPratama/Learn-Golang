# Know the Types of Operators on Golang

What are Operators?
Operator is a symbol / sign to perform the operation of calculating a number.

One example of an operator that we often do is addition. Even basic operators have been taught starting from elementary school. However... In the programming language the operator is not just a sum. There are several types of operators in the golang programming language.

## Types of operators in Golang
- Arithmetic
- Relationship / Comparison
- Logic
- Assignment

### Arithmetic Operators

Arithmetic operators consist of:
- + Addition
- -   Subtraction
- *   Multiplication
- /   Distribution
- % Modulus

For example :
```golang
package main

import (
"fmt"
)

func main() {

//Set Initial Value
number1 := 10
number2 := 5

//Sum Operator
resultsum := number1 + number2
fmt.Println(resultsum)

//Reduction Operator
result less := number1 - number2
fmt.Println(less result)

//Multiplication Operator
product := number1 * number2
fmt.Println(product)

//Sharing Operator
quotient := number1 / number2
fmt.Println(quote)

//Operator Modulus
remainder := number1 % numeral2
fmt.Println(modulus result)
}
```
For the results, you can run it yourself.

### Relational / Comparison Operators

The result of the comparison operator is True and False.
- ==
- !=
- <
- <=
- >
- >=

I assume you already understand what the signs are all for. Let's make an example of a comparison operation on golang:

```golang
package main

import (
"fmt"
)

func main() {

//Set Initial Value
number1 := 10
number2 := 5

number3 := number1 > number2
fmt.Println(number3) //output : True
}
```
This will return the output value True because the value 10 is greater than 5.

### Logical Operators

Logical operators are used to perform logical operations. The actual logical operators in mathematics have been used, such as AND, OR and NOT.

The result of a logical operator True or False

- &&    And
- || Or
- ! negation

For more details, let's look at the following code:
```golang
package main

import "fmt"

func main() {

a := false
b := true

c := a && b
fmt.Println(c) Output false
}
```
Logical operators are usually used to select conditions using if.. else… which we will discuss in future tutorials.

## Assignment Operators

The assignment operator is used to assign an assignment to a specified variable.

- = Charging
- += Addition
- -+ Reduction
- *= Multiplication
- %= Remaining quotient

```golang
package main

import "fmt"

func main() {

a := 5 // a = 5
a += 4 // a = a + 4

fmt.Println(a) // 5 + 4 = 9
}
```

[Indonesia]

# Mengenal Jenis Operator pada Golang

Apa Itu Operator ?
Operator adalah suatu simbol / tanda untuk melakukan operasi perhitungan sebuah angka.

Salah satu contoh operator yang sering kita lakukan yaitu penjumlahan. Bahkan operator dasar sudah di ajarkan mulai dari bangku sekolah dasar. Namun... Di dalam bahasa program operator bukan hanya sekedar penjumlahan saja. Ada beberapa Jenis Operator dalam bahasa program golang.

## Jenis operator dala Golang
- Aritmatika
- Relasi / Perbandingan
- Logika
- Penugasan

### Operator Aritmatika

Operator aritmatika terdiri :
- +   Penjumlahan
- -   Pengurangan
- *   Perkalian
- /   Pembagian
- %   Modulus

Contohnya : 
```golang
package main

import (
	"fmt"
)

func main() {

	//Set Nilai Awal
	angka1 := 10
	angka2 := 5

	//Operator Penjumlahan
	hasiljumlah := angka1 + angka2
	fmt.Println(hasiljumlah)

	//Operator Pengurangan
	hasilkurang := angka1 - angka2
	fmt.Println(hasilkurang)

	//Operator Perkalian
	hasilkali := angka1 * angka2
	fmt.Println(hasilkali)

	//Operator Pembagian
	hasilbagi := angka1 / angka2
	fmt.Println(hasilbagi)

	//Operator Modulus
	hasilsisa := angka1 % angka2
	fmt.Println(hasilmodulus)
}
```
Untuk hasilnya kalian bisa run sendiri.

### Operator Relasi / Pembanding

Hasil dari operator perbandingan yati True dan False.
- ==
- !=
- <
- <=
- >
- >=

Saya anggap kalian sudah paham untuk apa tanda itu semua. Mari kita buat contoh operasi perbandingan pada golang :

```golang
package main

import (
	"fmt"
)

func main() {

	//Set Nilai Awal
	angka1 := 10
	angka2 := 5

	angka3 := angka1 > angka2
	fmt.Println(angka3)         //output : True
}
```
Ini akan menghasilkan nilai output True karena nilai 10 lebih besar dari 5.

### Operator Logika

Operator logika digunakan untuk melakuakn operasi logika. Operator logika sebenarnya dalam mata pelajaran mateamtika sudah di gunakan, seperti AND, OR dan NOT.

Hasil dari operator logika True atau False

- &&    Dan
- ||    Atau
- !     Negasi

Untuk lebih jelas mari kita lihat di kodingan berikut
```golang
package main

import "fmt"

func main() {

	a := false
	b := true

	c := a && b
	fmt.Println(c)    Outpur false
}
```
Operator logika biasanya di gunakan untuk mneyeleksi kondisi menggunakan if.. else… yang akan kita bahas pada tutorial kedepannya. 

## Operator Penugasan

Operator penugasan digunakan untuk memberikan tugas pada variable yang telah ditentukan.

- =   Pengisian
- +=  Penjumlahan
- -+  Pengurangan
- *=  Perkalian
- %=  Sisa hasil bagi

```golang
package main

import "fmt"

func main() {

	a := 5      // a = 5
	a += 4      // a = a + 4

	fmt.Println(a)  // 5 + 4 = 9
}
```






















