# Understanding the Map in Golang

Map is a key… value… data array. This folder must exist in a programming language, it's just a different name. An example of key value implementation is JSON data, where the key is an identification while the value is defined data.

Map is more flexible than slice, where we can define the key data type and value. For example, there is a key with a string data type and a value with an integer data type. However, in one map arrangement, each element must be consistent.

## Define Map

```golang
map[KeyTypeData]ValueTypeData
var student = map[string]string{}
var student map[string]string
student = make(map[string]string)
```

## Declaration of Value in Map

```golang
var student = map[string]string{"name": "Endy", "address": "Kediri"}
```

## Fill in Map Data

```golang
variableMap[Keyname]=Value
student["Name"] = "Endy"
student["address"] = "Kediri"
```

## Print Key and Value

```golang

main package

import (
"fmt"
)

func main() {
var student = map[string]string{"name": "Endy", "address": "Kediri"}
  
  fmt.Println(student)
  // output : map[Name:Endy address:Kediri]
  
  // Print with a range . loop
for i, v := range of students {
fmt.Println(i, "=", v)
}

}
```

## Delete Map Value

```golang
delete(variableMap, key)
delete(student, "address")
```

## Merge Map with Slice

In general, to handle a need, you must use slices to manage large amounts of data. Slices are used to manage large amounts of data, while slice data elements are in the form of maps.

An example of its use is when you have 10 student data and each data has a different key value.

Usually a combination of map and slice to handle data that comes from a database, for example a MySQL database.

To make it clearer, let's make the code, the following is a combination of map code with slices:
```golang
package main

import "fmt"

func main() {
  var student = []map[string]string{
    map[string]string{"name": "Endy", "address": "Kediri"},
    map[string]string{"name": "Oliv", "address": "Sidoarjo"},
  }

  for i, v := range of students {
    fmt.Println(i, "= name :", v["name"], "address:", v["address"])
  }
}
outputs:
0 = name : Endy address : Kediri
1 = name : Oliv address : Sidoarjo
```

[Indonesia]

# Memahami Map di Golang

Map merupakan sebuah key… value… data array. Map ini wajib ada dalam sebuah bahasa program, hanya saja namanya yang berbeda. Contoh implementasi key value yaitu data JSON, dimana key nya merupakan sebauh identifikasi sedangkan value nya merupakan data yang di definisikan.

Map lebih bersifat fleksibel dari pada slice, dimana kita dapat menentukan tipe data key nya dan value nya. Sebagai contoh ada sebuah key dengan tipe data string dan value dengan tipe data integer. Namun dalam satu susunan map harus konsisten pada setiap elemen.

## Mendefinisikan Map

```golang
map[KeyTypeData]ValueTypeData
var mahasiswa = map[string]string{}
var mahasiswa map[string]string
mahasiswa = make(map[string]string)
```

## Deklarasi Nilai di Map

```golang
var mahasiswa = map[string]string{"nama": "Endy", "alamat": "Kediri"}
```

## Mengisi Data Map

```golang
variableMap[namaKey]=Value
mahasiswa["Nama"] = "Endy"
mahasiswa["alamat"] = "Kediri"
```

## Mencetak Key dan Value

```golang

package main

import (
	"fmt"
)

func main() {
	var mahasiswa = map[string]string{"nama": "Endy", "alamat": "Kediri"}
  
  fmt.Println(mahasiswa)
  // output : map[Nama:Endy alamat:Kediri]
  
  // Mencetak dengan perulangan range
	for i, v := range mahasiswa {
		fmt.Println(i, "=", v)
	}

}
```

## Delete Nilai Map

```golang
delete(variableMap, key)
delete(mahasiswa, "alamat")
```

## Menggabungkan Map dengan Slice

Pada umumnya untuk menangani suatu kebutuhan harus menggunakan slice guna mengelola data yang banyak. Slice untuk mengelola data yang banyak, sedangkan element data slice berupa map.

Contoh penggunaannya yaitu ketika mempunyai data mahasiswa dengan jumlah 10 dan setiap data mempunyai key value yang berbeda-beda.

Biasanya Kombinasi map dan slice untuk menangani data yang berasal dari database, misanya database MySQL.

Biar lebih jelas mari kita bikin kodenya, berikut ini gabungan kode map dengan slice :
```golang
package main

import (
	"fmt"
)

func main() {
	var mahasiswa = []map[string]string{
		map[string]string{"nama": "Endy", "alamat": "Kediri"},
		map[string]string{"nama": "Oliv", "alamat": "Sidoarjo"},
	}

	for i, v := range mahasiswa {
		fmt.Println(i, "= nama :", v["nama"], "alamat:", v["alamat"])
	}
}
output : 
0 = nama : Endy alamat : Kediri
1 = nama : Oliv alamat : Sidoarjo
```
