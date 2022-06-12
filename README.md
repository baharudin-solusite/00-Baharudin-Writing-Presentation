# **JavaScript**

## **1.Condisional**

Condisional Statment bertugas mengecek kondisi spesifik untuk menjalankan sebuah perintah berdasarkan kondisi yang dinilai terbaik akan dipilih (true) maka kode dijalankan, (false) maka kode tidak berjalan
//sebagai contoh alur kita saat sedang mengabil makan maka kodisi yang akan kita lakukan bagaimana?

### ***(Condisional if else)***
***contoh sederhana***
```js
if(true){
    console.log("saya masuk kerja");
    } else {
        console.log("saya tidak masuk");
    }
    //input keluar = saya masuk kerja

    // (true) melambangkan sebuah kondisi
```
***contoh dengan nilai***
```js
const nilai = 70;
if (nilai >= 80){
    console.log("nilainya A");
} else if (nilai >= 60) {
   console.log("nilainya B");
} else if (nlai >= 40){
    console.log("nilainya C");
} else {
    console.log('remidi');
}
//"nilainya B"
```
### ***(Switch Case)***
digunakan saat kondisi percabangan terlalu banyak hampir sama dengan (if else) tetapi lebih detail cara penggunaan data di setiap Swich-Case wajib memiliki nilai default
```js
const lampu = "hijau";
switch (lampu){
    case "hijau":
        console.log("Jalan")
        break;
    case "kuning":
        console.log("hati-hati")
        break;
    case "merah":
        console.log("Berhenti")
        break;
    default:
        console.log("hati-hati melintas") //boleh lewat      
}
```

## **2.Scope**
bagaimana kita dapat memproses data di dalam ruang lingkup tertentu bisa diakses/tidak

sebagai contoh ada 2 orang berada di daerah berbeda, pasti akan memikili suasana dan pemandangan berbeda pula
yang tidak dimiliki daerah satu sama lain

 ![](./img/dua%20tempat.jpeg)

kalo didalam sebuah kodingan, code yang berada di dalam sebuah block **Curly Braces { }**  jadi bila kodingan berada dalam sebuah block maka kodingan tidak dapat diakses dari luar block tersebut.

***1.*** bila fungsi berada diluar scope maka tidak dapat mengakses variabel yang berada didalam scope 

***2.*** kita dapat mengakses variabel bila variabel dan fungsi tersebut berada diluar scope atau bisa juga mengakses variabel diluar scope dengan fungsi yang berada didalam scope 

 ### ***variabel luar dapat diakses dari dalam***
 Contoh;
 ![](./img/Scope.jpeg)

 ### ***variabel didalam tidak dapat diakses dari luar***
 tidak dapat Akses 

 ![](./img/Scope2.jpeg)

 
## **3.Function**

adalah sebuah blok kode yang digunakan untuk membungkus suatu proses dengan tujuan agar mempermudah penulisan kode.

blok kode yang digunakan untuk membuangkus suatu proses agar proses tersebut tidak ditulis secara berulang kali.

***BEFORE***

***Menghitung luas persegi***
```js
let panjang = 10;
let lebar = 20;
let luas = panjang * lebar;
console.log(luas);//200

let panjang1 = 9;
let lebar1 = 20;
let luas1 = panjang1 * lebar1;
console.log(luas1);//180
```
***A) Argumen dan parameter***
Argumen dan Parameter berguna untuk mengetahui suatu nilai/angka sebuah Function 
```js
function luasArea(widht, height) {
    return widht * height
}
console.log(luasArea(10,10));//100
console.log(luasArea(15,17));//255
console.log(luasArea(17,10));//170
console.log(luasArea(100,10));//1000
```
***B.Default Parameters***

Default paramaters digunakan untuk memberikan nilai awal/default pada parameter function.

Default parameters bisa digunakan jika kita ingin menjaga function agar tidak error saat dipanggil tanpa argumen

***C)Function Helper***

Kita bisa menggunakan function yang sudah dibuat pada function lain

***D.Arrow Function***

Arrow function adalah cara lain menuliskan function. Ini adalah fitur terbaru yang ada pada ES6 (Javascript Version)

## **4.Looping**
mengulang sebuah instruksi hingga kondisi terpenuhi atau jika kondisi telah terpenuhi.

sebagai contoh; orang yang ingin pergi keluar dia akan menata barang apa saja yang akan dibawa bila masih ada akan mencari kmbali barang tersebut

***A)Manual Looping***
kita menulis secara manual sebuah pengulangan
```js
console.log(1)//1
console.log(2)//2
console.log(3)//3
console.log(4)//4
console.log(5)//5
```
 ## **5.Prototype**

 yaitu sebuah fitur bawaan javascript yang bisa ditambahkan pada sebuah properti

 A) Constructor bila kita memiliki banyak objeck dari pola data yang sama kita bisa meggunakan fitur constractor

 kita tidak bisa mengunakan fitur constractor secara langsung

 ***Memanggil Objeck yang berada pada Prototype***
```js
console.log(Object);//tidak terpanggil
console.log(Object.prototype);//terpangil
```
B) *Menthod/Function Prototyping* 

kita juga bisa menambahkan method untuk constructor yang telah kita buat Method bisa digunakan untuk semua instance object. jadi buat satu kali untuk digunakan semua instrance object

kita juga dapat menambahkan sebuah properti menggunakan Custom prototype

kita dapat menambah properti menggunakan custem properti
```js
String.prototype.repeatString = function (n) {
    return this.repeat(n);
};
console.log("Public".repeatString(2));//11111
```
 ## **6 Array**
 Sebuah variabel yang dapat menampilkan banyak data dan Jenis tipe data

