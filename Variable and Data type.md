# Learn to recognize variables and data types

A variable is a symbol used to store a value either temporarily or permanently. While the data type is a type of data stored in a variable.

What is the relationship between variables and data types?
A variable is an entity that has a certain data type. A data type is something that defines the variable.

## Creating Variables

To create a variable that needs to be considered is the writing format. It is necessary to know that in the Golang language, to declare a <strong> variable, you can use the <strong> data type <strong> or not</strong>. Examples like this

```golang
  //var <variable name> <data type>
  var string name = "Endy"
  var name, address, school string
  var height = 180
  height := 180
```

## Type Golang data type
1. Number(Number data type)
    1. integers
        ```golang
        var integer height = 180
        ```
    2. Floats
        ```golang
        var float width = 3.5
        ```
2. Text(String data type)
    ```golang
    var string name = "Endy"
    ```
3. Booleans data type
    ```golang
    var login boolean = True
    ```
    
The following is an example of using a variable in golang.

```golang
package main

import "fmt"

func main() {
var name, address, school string
var age int

name = "Endy"
address = "Kediri"
school = "UPN"
age = 21
height := 180
weight := 68
  
fmt.Println("==== Biodata ==")
fmt.Println("Name : " + name)
fmt.Println("Address : " + address)
fmt.Println("School : " + school)
fmt.Println("Age : ", age)
fmt.Println("Height", height)
fmt.Println("Weight", weight)
}
```
If so, it's time for us to run.

```github
go run main.go
```

## Rules for writing data types in Golang

The following are the rules for writing the Golang programming language:

- Cannot give variable names with numbers (0-9).
- Can't add prefix / cloud $ in variable.
- The value of the variable must match the data type.
- It is not allowed to give variable names with golang keywords, for example if, map and others.

## Conversion of data types on Golang

Why should it be converted?

Golang is very strict, cannot combine or perform operators with different data types. For example Integer + String.

Although there are ways to declare variables by directly assigning a value or not specifying a data type, there are times when we are required to convert to another data type.

### Conversion Example

The following is an example of a data type conversion:

```golang
strconv.Itoa(variable)
```

The code above is the code that serves to change the data type from int to string. The other functions are also like:
- Atoi() to convert from string to integer data type.
- Itoa() to convert from integer to string.
- ParseBool() to convert string data type to integer data type.
- FomatBool() to convert bolean data type into string.

Let's try the implementation..

```golang
package main

import (
"fmt"
"strconv"
)

func main() {
    vara = "10"
    var b = 2
    var toInteger, err = strconv.Atoi(a)

    if err == nil {
        var result = a + b
        fmt.Println(result) // Output : 12
    }
}
```

Note: Here we need to import a new library, namely strconv to do the conversion.

[Indonesia]

# Belajar mengenal variabel dan tipe data

Variabel adalah simbol yang digunakan untuk menyimpan sebuah nilai baik sementara maupun tetap. Sedangkan Tipe data adalah suatu tipe data yang tersimpan dalam suatu variable.

Apa hubungan variabel dan tipe data?
Variabel merupakan entitas yang memiliki tipe data tertentu. Tipe data adalah sesuatu yang mendefinisikan variabel tersebut.

## Membuat Variabel

Untuk membuat variable yang perlu di perhatikan yaitu format penulisannya. Perlu di ketahui di bahasa golang untuk mendeklrasaikan variable <strong>dapat menggunakan</strong> tipe data <strong>maupun tidak</strong>. Contohnya seperti ini 

```golang 
  //var <nama variable> <titpe data>
  var nama string = "Endy"
  var nama,alamat,sekolah string
  var tinggi = 180
  tinggi := 180
```

## Jenis tipe data Golang
1. Number(Tipe data angka)
    1. integers
        ```golang
        var tinggi integer = 180
        ```
    2. Floats
        ```golang
        var lebar float = 3.5
        ```
2. Text(Tipe data string)
    ```golang
    var nama string = "Endy"
    ```
3. Tipe data booleans
    ```golang
    var login boolean = True
    ```
    
Berikut ini contoh menggunakan variable di golang.

```golang
package main

import "fmt"

func main() {
	var nama, alamat, sekolah string
	var umur int

	nama = "Endy"
	alamat = "Kediri"
	sekolah = "UPN"
	umur = 21
	tinggibadan := 180
	beratbadan := 68
  
	fmt.Println("=== Biodata ===")
	fmt.Println("Nama : " + nama)
	fmt.Println("Alamat : " + alamat)
	fmt.Println("Sekolah : " + sekolah)
	fmt.Println("Umur : ", umur)
	fmt.Println("Tinggi Badan", tinggibadan)
	fmt.Println("Berat Badan", beratbadan)
}
```
Jika sudah maka waktunya kita run. 

```github
go run main.go
```

## Aturan penulisan Tipe data pada Golang

Berikut ini aturan penulisan pada bahasa program golang:

- Tidak boleh memberikan nama variable dengan angka (0-9).
- Tidak boleh menambahkan prefix / awan $ dalam variable.
- Nilai dari varible harus sesuai dengan tipe data.
- Tidak boleh memberikan nama variable dengan keyword golang, misalnya if, map dan lainnya.

## Konversi Tipe data pada Golang

Kenapa harus di konversi ?

Di golang sangat ketat sekali, tidak dapat menggabungkan atau melakukan operator dengan tipe data yang berbeda. Contohnya Integer + String.

Meskipun terdapat cara untuk mendeklarasikan variable dengan langsung memberi nilai / tidak menentukan tipe data, namun ada kalanya kita di haruskan mengkoversi ke bentuk tipe data lainnya.

### Contoh Konversi 

Berikut contoh konversi tipe data : 

```golang
strconv.Itoa(variable)
```

Kode diatas adalah code yang berfungsi untuk mengubah tipe data dari int ke string. Adapun fungsi - fungsi lainnya juga seperti : 
- Atoi() untuk mengubah dari string ke dalam tipe data integer.
- Itoa() untuk mengubah dari integer ke dalam string.
- ParseBool() untuk mengubah tipe data string ke tipe data integer.
- FomatBool() untuk mengubah tipe data bolean ke dalam string.

Yuk mari kita coba implementasinya..

```golang
package main

import (
"fmt"
"strconv"
)

func main() {
    var a = "10"
    var b = 2
    var toInteger, err = strconv.Atoi(a)

    if err == nil {
        var hasil = a + b
        fmt.Println(hasil) // Output : 12
    }
}
```

Catatan : Disini kita perlu import library baru yaitu strconv untuk melakukan konversi.
