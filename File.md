# View GO . Structure

## Variable Terms in Golang

1. GOROOT

GOROOT is the folder which contains the installation results of the Golang file. For example on Linux it is located in /usr/local. Golang can be used when there is GOROOT.

2. GOBIN

GOBIN is the Location to place the Binaries of the Golang Files project build.

3. GOOS

GOOS is a folder used to specify the operating system used

4. GOARCH

GOARCH is a folder that is used to specify / specify the architecture in the form of a processor. Parameters in this folder structure are not required to be provided.

5. GOPATH

GOPATH is the folder used to store our project files/folders. If you use XAMPP to run PHP files, it's like Golang's htdocs.

Golang recommends creating a folder with the name of a version control system followed by a free folder name, for example github.com even if you don't use a gitlab account. If you don't have version control, please create a folder with a free name in the version control system folder.

The folder structure by creating a folder name with the name version control is actually not mandatory but is recommended.

For example I created a folder with the name github.com and in the github.com folder I created a folder with the name student-GO.

Well, in this folder later as the project file that I use.

In this folder we can create a folder according to the name of the project we are working on.

Now let's take a look at our GOPATH folder structure.

```
|--- bin
|--- pkg
|--- src
      |--- github.com
                |---learning-GO
```

## How to see the environment on Golang

The way to see all environments in Golang just type this in your terminal.
```github
go env
```

[Indonesia]

# Melihat Struktur GO

## Variabel Istilah-istilah di Golang

1. GOROOT

GOROOT adalah folder dimana berisi hasil instalasi file Golang. Misalnya di Linux yang terletak di /usr/lokal. Golang dapat digunakan ketika terdapat GOROOT.

2. GOBIN

GOBIN adalah Lokasi untuk meletakkan file Binari dari build projek File Golang.

3. GOOS

GOOS adalah folder yang digunakan untuk mengkhususkan sistem operasi yang di gunakan

4. GOARCH

GOARCH adalah folder yang digunakan untuk mengkususkan / mensesifikasi arsitektur yang berupa proccessor. Parameter pada struktur folder ini tidak wajib di berikan.

5. GOPATH

GOPATH adalah folder yang digunakan untuk menaruh file / folder projek kita. Jika menggunakan XAMPP untuk menjalankan file PHP ibaratnya htdocs nya Golang.

Golang merekomendasikan untuk membuat folder dengan nama sebuah version control system di ikuti dengan nama folder bebas, misalnya github.com walaupun kalian tidak menggunakan akun gitlab. Jika tidak mempunyai version control silahkan bikin folder dengan nama bebas di dalam folder version control system.

Struktur folder dengan membuat nama folder dengan nama version controll ini sebearnya tidak wajib namun di rekomenasikan.

Sebagai contoh saya membuat folder dengan nama github.com dan di dalam folder github.com saya membuat folder dengan nama nelajar-GO.

Nah, di dalam folder ini nantinya sebagai file projek yang saya gunakan.

Di folder inilah kita dapat membuat folder sesaui nama projek yang sedang di kerjakan.

Sekarang kita lihat struktur folder GOPATH kita.

```
|--- bin
|--- pkg
|--- src
      |--- github.com
                |--- belajar-GO
```

## Cara melihat environment pada Golang

Cara untuk melihat semua environtment di Golang cukup ketikkan ini pada terminal kalian.
```github
go env
```
