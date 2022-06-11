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
const lampuMerah = "hijau";
switch (lampuMerah){
    case "hijau":
        console.log("boleh lewat")
        break;
    case "kuning":
        console.log("hati-hati")
        break;
    case "merah":
        console.log("tidak boleh lewat")
        break;
    default:
        console.log("hati-hati melintas") //boleh lewat      
}
```

## **2.Scope**
bagaimana kita dapat memproses data di dalam ruang lingkup tertentu bisa diakses/tidak

sebagai contoh ada 2 orang berada di daerah berbeda, pasti akan memikili suasana dan pemandangan berbeda pula
yang tidak dimiliki daerah satu sama lain

kalo didalam sebuah kodingan, code yang berada di dalam sebuah block **Curly Braces { }**  jadi bila kodingan berada dalam sebuah block maka kodingan tidak dapat diakses dari luar block tersebut

### **Local Scope dan Global Scope**

***Local scope***, bila fungsi berada diluar scope maka tidak dapat mengakses variabel yang berada didalam scope 

***Global scope***, kita dapat mengakses variabel bila variabel dan fungsi tersebut berada diluar scope atau bisa juga mengakses variabel diluar scope dengan fungsi yang berada didalam scope 

 ### ***variabel luar dapat diakses dari dalam***
 Contoh;
 ![](./img/Scope.jpeg)

 ### ***variabel didalam tidak dapat diakses dari luar***
 tidak dapat Akses 

 ![](./img/Scope2.jpeg)

