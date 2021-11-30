# Understanding Condition Selection

For this condition, it is the same as other discussions, namely using if else and switch cases. The Golang language does not support the <b>ternary</b> language like PHP.

```golang
condition ?: result
```

## Condition If.. Else
```golang
package main

import "fmt"

func main() {
  value := 10

  if value > 7 {
    fmt.Println("You passed with a grade", grade)
  } else {
    fmt.Println("You Did Not Pass with Grade", grade)
  }
}
```
The above conditions are used to select a value, when the value is more than 7 it will result in a true selection condition, while false will result in a false condition. Another example with a true or false condition.
```golang
package main

import "fmt"

func main() {
  var s = "Indonesian"
  x := false
  if x {
    fmt.Println("You are in", s)
  } else {
    fmt.Println("You are not in", s)
  }
}
```
The output will go to else, why is that?? Because x evaluates to false, so we're going to enter else.

## Switch Case Condition

Condition Format:
```golang
switch expressions {
  case conditions:
    
}
```

An example of using a Switch Case is as follows:
```golang
package main

import "fmt"

func main() {
  value := 70

  switch value {
    case 50:
      fmt.Println("Your grade is C")
    case 70:
      fmt.Println("Your score is B")
    case 100:
      fmt.Println("Your grade is A")
    defaults:
      fmt.Println("No category")
  }
}
```
Because the value var is 70, it will go into case 70, if the var value is not in the case condition, it will go straight to default.

[Indonesia]

# Memahami Seleksi Kondisi

Untuk Kondisi ini sama seperti bahas lainnya yaitu menggunakan if else dan switch case. Pada bahasa Golang tidak mendukung dengan bahasa <b>ternary</b> seperti di PHP.

```golang
kondisi ?: hasil
```

## Kondisi If.. Else
```golang
package main

import "fmt"

func main() {
	nilai := 10

	if nilai > 7 {
		fmt.Println("Anda Lulus dengan Nilai", nilai)
	} else {
		fmt.Println("Anda Tidak Lulus dengan Nilai", nilai)
	}
}
```
Kondisi di atas digunakan untuk menyeleksi sebuah nilai, ketika nilai lebih dari 7 maka akan menghasilkan seleksi kondisi benar, sedangkan salah maka akan mengasilkan kondisi salah. Contoh lainnya dengan kondisi benar atau salah. 
```golang
package main

import (
	"fmt"
)

func main() {
	var s = "Indonesias"
	x := false
	if x {
		fmt.Println("Anda berada di", s)
	} else {
		fmt.Println("Anda tidak berada di", s)
	}
}
```
Outputnya akan ke else, kenapa demikian?? Karena x bernilai false, jadi kita akan masuk ke else.

## Kondisi Switch Case

Format kondisi : 
```golang
switch expression {
  case condition:
    
}
```

Contoh menggunakan Switch Case sebagai berikut : 
```golang
package main

import "fmt"

func main() {
	nilai := 70

	switch nilai {
	case 50:
		fmt.Println("Nilai Anda C")
	case 70:
		fmt.Println("Nilai Anda B")
	case 100:
		fmt.Println("Nilai Anda A")
	default:
		fmt.Println("Tidak ada kategori")
	}
}
```
Karena var nilai bernilai 70, maka akan masuk kedalam case 70, jika var nilai tidak ada dalam condisi case, maka akan langsung masuk ke default. 







