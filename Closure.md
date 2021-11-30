# Closure function in Golang

A golang closure function is a function that returns another function. Can be stored in a variable or directly returned a value in the function.

An example of implementing the closure function in another language is PHP with the Laravel Framework. In Laravel you can perform a closure function as a query.

If you already know that the closure is a function inside a function, then the function inside the function will only be executed on the function that wraps it.

The closure function is an anonymous function, because it is a block of function code that does not have a function name. But can do a process.

Yul, let's just make an example program for the closure function in golang.

```golang
package main

import "fmt"

func main() {

  go1 := func() {
    fmt.Println("Learn Golang!")
  }
  go2 := func() {
    fmt.Println("Learn PHP!")
  }

  go1()
  go2()
}
outputs:
Learn Golang!
Learn PHP!
```
Creating a Closure Function with Return
In Golang, you can return a value in the form of a function and a data type value.

Here's an example:

```golang
package main

import "fmt"

func todo() func() int {
  i := 2
  return func() int {
    i++
    j := 1
    return j
  }
}

func main() {
  dataTodo := todo()
  fmt.Println("The value of toDo is", dataTodo())
}
outputs:
The value of toDo is 1. Why is that?? because even though the value of i goes to the next function, what is returned last is var j which has a value of 1.
```

[Indonesia]

# Fungsi Closure di Golang

Fungsi closure golang adalah fungsi yang mengembalikan fungsi lainnya. Dapat di simpan dalam variable maupun secara langsung di kembalikan nilai di dalam fungsi tersebut.

Contoh penerapan fungsi closure di bahasa lain yaitu PHP dengan Framework Laravel. Di dala Laravel dapat melakukan fungsi closure sebagai query.

Jika sudah tahu bahwa closure merupakan fungsi di dalam fungsi maka fungsi di dalam fungsi hanya akan di jalankan pada fungsi yang membungkusnya.

Fungsi closure merupakan anonymous function , karena sebuah blok kode fungsi yang tidak mempunyai nama fungsi. Namun bisa melakukan suatu proses.

Yul langsung saja kita buat contoh program fungsi closure di golang.

```golang
package main

import "fmt"

func main() {

	go1 := func() {
		fmt.Println("Belajar Golang!")
	}
	go2 := func() {
		fmt.Println("Belajar PHP!")
	}

	go1()
	go2()
}
output : 
Belajar Golang!
Belajar PHP!
```
Membuat Fungsi Closure dengan Nilai Balik
Di Golang dapat di lakukan nilai balik berupa sebauh fungsi dan nilai tipe data.

Berikut ini contohnya :

```golang
package main

import (
	"fmt"
)

func todo() func() int {
	i := 2
	return func() int {
		i++
    j := 1
		return j
	}
}

func main() {
	dataTodo := todo()
	fmt.Println("Nilai toDo adalah", dataTodo())
}
output : 
Nilai toDo adalah 1. Kenapa demikian?? karena walaupun nilai i masuk ke function selanjutnya tapi yang di return terakhir adalah var j yang bernilai 1.  
```
