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
