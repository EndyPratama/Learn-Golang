# Make Hello World!

Well as usual here we will create the first page or the first program, which displays Hello World.

Before we start, let's understand the 3 concepts in Golang when creating a project.

The Golang program is fairly simple, it doesn't write too much code.

1. Write the code in the text editor.
2. Run Golang Files.
3. Build the Golang Project into Binary form.

It should be noted that point 3 is carried out when the project is finished or has been completed. so we focus on points 1 and 2.

Let's start making the first program in Golang.

1. You guys just finished creating folders. We use the folder
2. We create a file in the folder. Here I named it with main.go
3. Oh yes, if you have already installed the extension, please restart your VSC first.
4. If you have entered this code into main.go
```golang
main package

import (
"fmt"
)

func main(){
fmt.Println("Hello World!")
}
```
5. The code above is used to display the text "Hello World!" Please note that golang has a main method / function that is called when the program is run, namely func main(). This is the same if the PHP language is named index.php.
6. To run the go file, you can open your respective terminal code editor". For VSC you can use the ``` CTRL + ` ```` key. Then to run it type this. the name of the file you created).
```github
go run play.go
```
8. Done

[Indonesia]

# Membuat Hello World!

Baiklah seperti biasa disini kita akan membuat halaman pertama atau program pertama, yaitu menampilkan Hello World. 

Sebelum Memulai Kita Pahami dulu 3 Konsep di Golang ketika membuat suatu projek.

Program Golang terbilang cukup sderhana, tidak terlalu banyak menuliskan kode.

1. Menuliskan kode di text Editor.
2. Menjalankan File Golang.
3. Build Projek Golang ke dalam bentuk Binary.

Perlu di ketahui pada poin 3 di lakukan ketika projek sudah selesai ataupun sudah selesai. jadi kita fokus ke point 1 dan 2.

Yuk Kita mulai membuat program pertama di Golang.

1. Kalian kan tadi sudah selesai membuat folder. Kita gunakan folder tersebut
2. Kita buat sebuah file dalam folder tersebut. Disini saya menamainya dengan main.go
3. Oh ya jika kalian tadi sudah install extension harap restart dahulu VSC kalian. 
4. Jika sudah masukkan kode ini kedalam main.go
```golang
package main

import (
	"fmt"
)

func main(){
	fmt.Println("Hello World!")
}
```
5. Kode diatas digunakan untuk menampilkan Tulisan "Hello World!" Perlu diketahui golang mempunyai method / fungsi utama yang di panggil ketika program tersebut di jalalnkan yaitu func main(). Ini sama aja jika di bahasa PHP bernama index.php.
6. Untuk menjalankan file go kalian bisa buka terminal code editor kalian masing". Untuk VSC dapat dengan tombol ``` CTRL + ` ```. Lalu untuk menjalankanya ketik ini. (main.go itu merupakan file yang kalian buat, sesuaikan dengan nama file yang kalian buat).
```github
go run main.go
```
8. Selesai
