# Structure and rules of writing in Golang

Let's go over the code we covered yesterday.

```golang
main package

import (
"fmt"
)

func main(){
fmt.Println("Hello World!")
}
```

Based on the code, there may still be a lot that you don't know. What are packages? What are imports? What is play? Let's discuss them one by one.

## Basic Structure of Golang

The structure of Golang is basically divided into 4, namely:
1. Package Declaration
2. Import Library
3. Main Method
4. Statement

```golang
package main -------------------------> package

import ( ------------------------> import
"fmt"
)

func main(){ ------------------------> main function
fmt.Println("Hello World!")
}
```

Discussion :

### Package Declaration

Package is a way to organize the existing files or can be said to be the name of the available folders. In Golang a file can be run when it has package main.

So what if the file is in the root of our project?

```golang
main package
```

Declaration of a package when in the main project by declaring a package with the name main

When our project has a lot of modules, of course, we create folders in order to make the program structure neater and easier to understand.

Then how about an example of implementing a package in a folder?

Assume that in our project we have a folder with the name “model”, now in the folder there is a file with the name “mahasiswa.go”, then you can write a package like the code below.

```golang
package model
```

If we incorrectly declare the name to be "packege" then the program will error / cannot be run.

### Import

Import is used to call the library that we will use in the program, in the code example above we call a library called fmt.

Before continuing, what is a library?

Library is a collection of functions that are processed in such a way for us to use their functions. By using our library it is easier to create a program. Example of calling library in Golang language.

```golang
import "fmt"
```

### Method Main

In the Golang language there must be one main method name, where the method is executed the first time the program is run, namely the main() method. Without the main() method, the program cannot be executed. An example of the main method we used earlier is as follows.

```golang
func main(){
  fmt.Println("Hello World!")
}
```

### Statement

Statements are the smallest pieces of code. A statement can be interpreted as an action or activity carried out. In our example, the example statement is:


```golang
  fmt.Println("Hello World!")
```

The code above will produce the words "Hello World!" on our monitor screen. In Golang we don't need to use semicolon(;) at the end of the line of code.

## Block Program Golang

A code block is a tag used to wrap other code. Just like any other starting with { then closing with }
For example :

```golang
  if i < n {
    
  }
```

## Writing comments section

Golang comments are the same as PHP and other languages. There are 2 writing comments, namely:
1. inline (//this comment)
2. multiline (/*this is a comment*/)


Next we will get to know variables and data types.

[Inodadx]

# Struktur dan Aturan penulisan dalam Golang

Mari kita bahas kode yang kemarin kita bahas.

```golang
package main

import (
	"fmt"
)

func main(){
	fmt.Println("Hello World!")
}
```

Berdasarkan kode tersebut mungkin masih banyak yang belum kalian ketahui. Apa itu package? Apa itu import? Apa itu main? Mari kita bahas satu persatu.

## Struktur Dasar Golang

Struktur Golang pada dasarnya dibagi menjadi 4, yaitu : 
1. Deklarasai Package
2. Import Library
3. Method Main
4. Statement

```golang
package main  -------------------------> package

import (      -------------------------> import
	"fmt"
)

func main(){  -------------------------> fungsi utama
	fmt.Println("Hello World!")
}
```

Pembahasan : 

### Deklarasi Package

Package adalah suatu cara untuk mengorganisasikan file yang ada atau bisa di bilang nama folder yang tersedia. Di Golang satu file dapat di jalankan ketika mempunya package main.

Nah bagaimana jika kasusnya file tersebut berada di root projek kita ?

```golang
package main
```

Deklarasi package ketika berada di main projek yaitu dengan mendeklarasikan package dengan nama main

Ketika projek kita mempunyai modul yang banyak tentunya kita membuat folder guna agar struktur program lebih rapi dan mudah di pahami.

Lalu bagaimana contoh implementasi package di dalam folder ?

Asumsikan di dalam projek kita punya folder dengan nama “model” nah di dalam folder terdapat file dengan nama “mahasiswa.go”, maka anda dapat menuliskan package seperti kode di bawah ini.

```golang
package model
```

Jika kita salah mendeklarasikan nama menjadi "packege" maka program akan error / tidak dapat dijalankan.

### Import

Import digunakan untuk memanggil library yang akan kita gunakan dalam program, pada contoh kode dia atas kita memanggil sebuah library yang bernama fmt.

Sebelum lanjut, apa itu Library ?

Library adalah Sekumpulan fungsi yang di proses sedemikian rupa untuk kita gunakan fungsi nya. Dengan menggunakan library kita lebih di mudahkan untuk membuat suatu program. Contoh pemanggilan library pada bahasa Golang.

```golang
import "fmt"
```

### Method Main

Di dalam bahasa Golang harus ada satu nama method utama, dimana method tersebut di eskteksusi pertama kali saat program tersebut di jalankan, yaitu method main(). Tanpa method main() maka program tidak dapat di jalankan. Contoh method main yang kita gunakan tadi seperti berikut.

```golang
func main(){
  fmt.Println("Hello World!")
}
```

### Statement

Statement merupakan bagian terkecil dalam sebuah kode. Statement bisa diartikan sebuah tindakan atau kegiatan yang dilakukan. Pada contoh kita tadi contoh statement nya adalah.


```golang
  fmt.Println("Hello World!")
```

Kode diatas akan menghasilkan tulisan "Hello World!" pada layar monitor kita. Pada bahasa Golang kita tidak perlu menggunakan semicolon(;) pada akhir baris kode.

## Blok Program Golang

Blok kode adalah sebuah tanda yang digunakan untuk membungkus kode lainnya. Sama seperti lainnya diawali dengan { lalu ditutup dengan }
Contohnya : 

```golang
  if i < n {
    
  }
```

## Penulisan bagian komentar

Pada golang komentar sama seperti bahasa PHP dan lainnya. Penulisan komentar ada 2 yaitu :
1. inline     (//ini komentar)
2. multiline  (/*ini komentar*/)


Selanjutnya kita akan mengenal variabel dan tipe data.
