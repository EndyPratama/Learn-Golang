# How to use Functions and Returns in Golang

What is Function??

A function is a line of code wrapped in a specific name. A function / function can be given a parameter, either single or multiple.

Actually, at the beginning we have made 1 function, whether someone is aware of it and knows it or not.

```golang
func main(){
   ...
}
```
This is the function we've been running so far, it must exist when the program is first run.

Functions also have many benefits. One that we often encounter is that functions can be called repeatedly according to the arguments we want. Examples like this:

```golang
func sum(a int, b int){
   x = a + b
   return x
}
func print(int result){
   fmt.Println("Result is",result)
}
func main(){
   c = sum(1,2) // 3
   print(c)
   c = sum(5,7) // 12
   c = sum(3,9) // 12
   fmt.Println("The result is",c)
}
```

[Indonesia]

# Cara menggunakan Fungsi dan Return di Golang

Apa itu Fungsi ??

Fungsi merupakan sebuah baris kode yang di bungkus dengan nama terntentu. Sebauh fungsi / function dapat di berikan sebuah parameter, baik tunggal maupun banyak.

Sebenarnya saat awal kita sudah membuat 1 fungsi, entah ada yang sadar dan tau atau tidak. 

```golang
func main(){
  ...
}
```
Ini merupakan fungsi yang kita jalankan selama ini, ini harus ada saat program pertama kali di run. 

Fungsi juga mempunyai banyak manfaat. Salah satu yang sering kita jumpai adalah fungsi dapat dipanggil berulang ulang sesuai dengan argumen yang kita inginkan. Contohnya seperti ini : 

```golang
func jumlah(a int, b int){
  x = a + b
  return x
}
func cetak(hasil int){
  fmt.Println("Hasilnya adalah",hasil)
}
func main(){
  c = jumlah(1,2)   // 3
  cetak(c)
  c = jumlah(5,7)   // 12
  c = jumlah(3,9)   // 12
  fmt.Println("Hasilnya adalah",c)
}
```

