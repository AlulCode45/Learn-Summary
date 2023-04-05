# Basic Pemrograman

Pemrograman adalah kegiatan menulis,menguji,memperbaiki dan mempelihara perintah atau kode program komputer

Perintah / Kode -> Bahasa Mesin ( Di compile ) -> Eksekusi mesin

Input device -> CPU ( Processor ) -> output device

## Bahasa tingkat rendah ( low-level lenguage )

  Bahasa pemrograman yang hanya dimengerti oleh mesin dan dapat dijalankan langsung oleh mesin
  atau dalam artian bahasa sulit dimengerti oleh manusia contoh : assembler
  
## Bahasa tingkat tinggi

  Bahasa pemrograman yang sudah mendekati bahasa manusia, mesin membutuhkan compiler / interpreter untuk dapat mengerjakan perintah yang dituliskan dengan bahasa ini. Contoh : C++ , PHP , Python

# 🚀 Mulai Belajar Kotlin

## Struktur Kotlin

```kotlin
fun main(args: Array<String>){
    println("Hello World")
}
```

## Variable Kotlin

##### Contoh variable  

```kotlin
  var nama: String  
  var alamat: String = "Bojonegoro"
```

keterangan : Variable kosong yang belum di kasih value wajib di set tipe datanya.  

## Variable Imutable dan Mutable

Variable konstan atau tidak bisa di rubah menggunakan (val)  

```kotlin
   val nama = "Alul"  
```

variable mutable atau bisa di rubah menggunakan (var)  

```kotlin
   var nama = "Alul"  
```

## Tipe data Kotlin

```text
Int = bilangan bulat - toInt()  
Float = pecahan - toFloat()  
Double = pecahan lebih besar dari Float - toDouble()  
Boolean = True / False   
Char = karakter tunggal - toChar()  
String = teks - toString()  
Unit = mirip dengan void  
```

## Operator Kotlin

### 1) Operator Aritmatika

```text
(+) Penjumlahan
(-) Pengurangan
(*) Perkalian
(/) Pembagian
(%) Modulus
```

### 2) Operator assignment

```kotlin
val g = 10
val g -= 1
val g += 1
val g /= 2
val g *= 2
val g %= 2
```

### 3) Operator Unary,Increment & Decrement

```text
+a
-a
!a
a++
a--
```

### 4) Operator Perbandingan dan Persamaan ( Comparison & Equality )

```text
(>) Lebih besar dari
(<) Lebih kecil dari
(>=) Lebih besar sama dengan
(<=) Lebih kecil sama dengan
(==) Sama dengan
(!=) tidak sama dengan
```

### 5) Operator Ligka ( Logical )

```text
( || ) Atau ( or )
( && ) Dan ( and )
```

### 6) Operator IN

Operator in digunakan untuk memerikasa apakah suatu objek termasuk dalam koleksi

```text
( in ) => ex: a in b
( !in ) => ex : a !in b
```

### 7) Operator bitwise

```text
(shl) = <<
(shr) = >>
(ushr) = >>>
(and) = &
(or) = or
(xor) = xor
(inv) = inv
```

## Array

### Contoh penggunaan Array

```kotlin
val mobil = arrayOf("toyota","honda","tesla")
```

### Cara pemanggilan Array

```kotlin
println(mobil[1])
```

### Cara Mengakses Semua Elemen Array

```kotlin
val mobil = arrayOf("toyota","honda","tesla")
for (m in mobil){
  println(m)
}
```

### Mengubah Elemen Array

```kotlin
val mobil = arrayOf("Toyota","Honda","Tesla")
mobil[1] = "Mazda"
```

### Mendapatkan Ukuran Array

```kotlin
val mobil = arrayOf("Toyota","Honda","Tesla")
println(mobil.size) //Hasil = 3
```

### Mengecek Elemen Array

```kotlin
val mobil = arrayOf("Toyota","Honda","Tesla")
if("Tesla" in mobil){
  //True
}else{
  //False
}
```

## Fungsi

Fungsi / Method / Function adalah blok kode program yang dirancang untuk mengerjakan tugas tertentu  

### Keuntungan Menggunakan Fungsi

- Mengurangi pengulangan kode
- Menghemat baris kode
- Membuat program lebih rapi
- Mudah dibaca
- Mempercepat coding

### Struktur kode fungsi

```kotlin
//Fungsi tanpa parameter  
fun namaFungsi(){
}

//Fungsi berparameter  
fun namaFungsi(namaParam: TipeData = defaultValue){
}
```

### Pemanggilan kode fungsi

```kotlin
// Memanggil fungsi tanpa param
namaFungsi()

// Memanggil fungsi dan parameter
namaFungsi(parameter)
```

# Percabangan

## Percabangan Menggunakan if

![If Flowchart](https://www.programtopia.net/wp-content/uploads/2021/01/if_0.png)

#### Code if

```kotlin
if(condition){
    //statement
}

//Contoh
fun main(args: Array<String>) {
    var a = 20
    var b = 18
    
    if(a>b){
        println("$a lebih besar dari $b")
    }
}
```

## Percabangan Menggunakan if - else

![If Else Flowchart](https://www.programtopia.net/wp-content/uploads/2021/01/ifelse_0.png)

#### Code if - else

```kotlin
if(condition){
    // statement jika true
}else{
    // statement jika false
}

//Contoh
fun main(args: Array<String>) {
    var a = 20
    var b = 18
    
    if(a>b){
        println("$a lebih besar dari $b")
    }else{
        println("$a lebih kecil dari $b")
    }
}
```

## Percabangan Menggunakan if - else if - else

![If Else If Flowchart](https://www.tutlane.com/images/swift/swift-if-else-if-statement-algorithm-diagram.png)

#### Code if - else if - else

```kotlin
if (kondisi1) {

  // blok kode program yang dieksekusi jika kondisi1 bernilai true

} else if (kondisi2) {

  // blok kode program yang dieksekusi jika kondisi1 bernilai false and kondisi2 bernilai true

} else {

  // blok kode program yang dieksekusi jika kondisi1 bernilai false dan kondisi2 juga bernilai false

}

//Contoh
fun main(args: Array<String>) {
    val jam = 22
    if (time < 10) {
        println("Selamat pagi")
    } else if (jam < 14) {
        println("Selamat siang")
    } else if (jam < 18) {
        println("Selamat sore")
    } else {
        println("Selamat malam")
    }
}
```

## Percabangan When / Switch Case

![When FLowchart](https://uploads-ssl.webflow.com/6184b461a39ff1011f8c0582/624bffae64d6b60b5e49105e_Switch%20Case%20Flowchart.png)

#### Code When

```kotlin
// Code dasar when
val varName = when (varSelected) {
  valueCompare1 -> "Results1"
  valueCompare2 -> "Results2"
  else -> "Else Results"
}

// Contoh penggunaan
val hari = 4
val hasil = when (hari) {
  1 -> "Senin"
  2 -> "Selasa"
  3 -> "Rabu"
  4 -> "Kamis"
  5 -> "Jumat"
  6 -> "Sabtu"
  7 -> "Minggu"
  else -> "Tidak valid"
}
println(hasil)

// Blok Perintah pada When
when (variable) {
    state1 -> {
        // blok yang dieksekusi jika variabel == state1
    }
    state2 -> { 
        // blok yang dieksekusi jika variabel == state2
    } 
    else -> {
        // blok yang dieksekusi jika semua kondisi false
    }
}
//Contoh Penggunaan Blok Perintah
val hari = 4
when (hari) {
    1 -> {
        println("Nilai hari = 1")
        println("Maka, hari = Senin")
    }
    2 -> { 
        println("Nilai hari = 2")
        println("Maka, hari = Selasa")
    } 
    3 -> { 
        println("Nilai hari = 3")
        println("Maka, hari = Rabu")
    } 
    4 -> { 
        println("Nilai hari = 4")
        println("Maka, hari = Kamis")
    } 
    5 -> { 
        println("Nilai hari = 5")
        println("Maka, hari = Jumat")
    } 
    6 -> { 
        println("Nilai hari = 6")
        println("Maka, hari = Sabtu")
    } 
    7 -> { 
        println("Nilai hari = 7")
        println("Maka, hari = Minggu")
    } 
    else -> {
        println("Nilai hari = $hari")
        println("Maka, hari = tidak valid")
    }
}

```

# Perulangan

Perintah perulangan merupakan sebuah perintah, yang tujuannya akan mengulang blok baris perintah tertentu jika kondisi pengecekan bernilai benar (true). Di dalam bahasa pemrograman, biasanya terdapat 2 macam perulangan, yaitu: for dan while.  

## For Loop

![For concept looping](https://problemsolvingwithpython.com/09-Loops/images/flow_chart_of_program_that_contains_a_for_loop.png)

#### Code program

```kotlin
for (item in collection) {
    // blok perintah yang diulang
}

//contoh penggunaan
fun main(args: Array<String>) {
    for (i in 1..3) {
      prinln(i)
    }
}

//Rumus Perintah for DownTo
for (item in starting downTo ending step stepping) {
    // blok yang dipanggil ketika berulang
}
//contoh penggunaan
for (i in 6 downTo 0 step 2) {
    println(i)
}
```

## While Loop

![while Flowchart](https://uploads-ssl.webflow.com/6184b461a39ff1011f8c0582/623c0c66fad507a80764a3f5_while-loop-flowchart.png)

#### Code Program

```kotlin
while (condition) {
    // blok kode yang dieksekusi jika condition bernilai true
}

//Contoh penggunaan

// buat variabel baru dengan nama g
// isi variabel g dengan nilai 0
var g = 0

// mulai perintah perulangan while
// cek, apakah nilai g < 5? 
while (g < 5) {

  // blok ini dijalankan, selama nilai g < 5 = true
  println(g)

  // perubahan nilai g di setiap perulangan
  g++
}
```

## Do While Loop

![Do while flowchart](https://2.bp.blogspot.com/-Ejqpw2aVATE/XGYHCwNy83I/AAAAAAAACH8/0ax3VKgaj6IrSNogkBd5WFLOrRT5TLQigCLcBGAs/s640/ilearning_logo.png)

#### Perbedaan While dan Do-While

Perintah perulangan do-while sebenarnya tidak berbeda jauh dengan perintah perulangan while. Satu-satunya perbedaan adalah, di perulangan do-while setidaknya blok kode program di dalam perulangan selalu dilakukan minimal 1x.  

Perhatikan rumus berikut ini:

```kotlin
do { 
    
    // blok yang dieksekusi, minimal 1x
    
} while (conditional)
```

#### Contoh penggunaan do While

```kotlin
fun cekKoneksiJaringan() { 
    // kode program lengkap tidak ditampilkan

    return kondisiJaringan;
}

fun main(args: Array<String>) {
    do { 
         var koneksi = cekKoneksiJaringan()
         if (koneksi) {
             // lakukan sesuai jika koneksi aktif
         } else {
             // lakukan sesuai jika koneksi tidak aktif
         }
    } while (!cekKoneksiJaringan())
}
```
