# -LT-19_Typeof

`typeof` adalah operator unary dalam JavaScript yang digunakan untuk menentukan tipe data dari sebuah variabel atau ekspresi. Operator ini akan mengembalikan string yang menggambarkan tipe data dari ekspresi yang ditentukan. Contoh:

    console.log(typeof "hello");   // "string"
    console.log(typeof 42);        // "number"
    console.log(typeof true);      // "boolean"
    console.log(typeof undefined); // "undefined"
    console.log(typeof {});        // "object"

Catatan: Beberapa tipe data JavaScript seperti Array dan Function juga akan diidentifikasi sebagai "object" oleh operator typeof.

Selain itu, operator typeof juga dapat digunakan untuk menentukan tipe data dari sebuah fungsi atau class. Contohnya:

    function myFunction() {}
    console.log(typeof myFunction); // "function"

    class MyClass {}
    console.log(typeof MyClass); // "function"

Operator typeof juga dapat digunakan untuk menentukan apakah sebuah variabel atau ekspresi bernilai "undefined" atau tidak. Contohnya:

    let myVar;
    console.log(typeof myVar === "undefined"); // true

    let myVar = null;
    console.log(typeof myVar === "undefined"); // false

Sebagai catatan, jika Anda ingin menentukan apakah sebuah variabel bernilai undefined atau tidak, sebaiknya menggunakan operator "===" atau "!==" daripada menggunakan operator typeof. Secara keseluruhan, operator typeof adalah alat yang berguna untuk menentukan tipe data dari sebuah variabel atau ekspresi dalam JavaScript.

Selain itu, operator typeof juga dapat digunakan untuk menentukan tipe data dari sebuah objek yang didefinisikan oleh pengguna. Contohnya:

    let myObject = {name: 'John', age: 42};
    console.log(typeof myObject); // "object"

Namun, jika Anda ingin menentukan tipe dari objek yang didefinisikan oleh pengguna, Anda dapat menggunakan properti khusus "constructor" pada objek tersebut. Contohnya:

    console.log(myObject.constructor.name); // "Object"

Sebagai catatan, operator typeof tidak akan bekerja dengan benar untuk objek yang dibuat menggunakan literal notasi seperti yang digunakan dalam contoh di atas, karena semua objek literal akan ditentukan sebagai "object" oleh operator typeof.

Secara keseluruhan, operator typeof adalah alat yang berguna untuk menentukan tipe data dari sebuah variabel atau ekspresi dalam JavaScript. Namun, untuk objek yang didefinisikan oleh pengguna, Anda dapat menggunakan properti "constructor" untuk mendapatkan tipe data yang lebih spesifik.
