# JavaScript - 100 Day

## belajar day #1 mod (1)

# Lingkungan Javascript :

### console (browser)

    - menampilkan error
    - debug

### alert (script)

    - menampilkan notifikasi/pop up
        contoh : alert("hello world");

# Nilai dan Tipe Data :

## Materi

### Biner

    - "bit/binary digit, adalah satuan terkecil dari data yang ada di dalam komputer kita"

    - bit yaitu 0/1

    - contoh biner : "biner -> decimal"
            1  0 1 1 1 --> contoh kasus
            16 8 4 2 1 --> rumus biner
            16 0 4 2 1 --> total nya 23

### Values/nilai atau tipe data

    # Jenis Tipe data
        - number --> 10, -1500, 3.14
        - string --> "", "hello world"
        - boolean
        - object
        - function
        - undefined

    # Angka
        - "didalam javascript tidak ada integer atau bilangan bulat, yang ada hanya floating point"

        - ukuran nya hanya 63 bit / 2^64 / 18x10^18

        - # Angka tanpa desimal
            * 10, 1500, 123456 (menggunakan tanda koma)
            * akurat sampai 15 digit
        - # Angka dengan desimal
            * 3.14, 0.5, 100.00 (menggunakan tanda titik)
        - # Eksponen
            * 123e5 // 12300000
            * 123e-5 // 0.00123
        - # Bilangan negatif
            "jangan pernah mengawali angka dengan 0(okta) atau sama seperti 0x(hexadesimal)"
        - # Angka Spesial
            * Infinity : 2/0
            * -Infinity : -2/0
            * NaN (not a number) : 0/0 atau 100/"apel"

### Operator pada javascript

    Note : "operator dalam javascript adalah sebuah syntax yang digunakan untuk melakukan operasi"

    # Operator
        - aritmatika -
        - penugasan     -
        - perbandingan      - {binary}
        - logika        -
        - string     -

        - kondisional - ternary

        - typeof - unary

        * binary
            note :
                "membutuhkan 2 operand"
            contoh :
                operand1 operator operand2

        * unary
            note :
                "membutuhkan 1 operand"
            contoh :
                operator operand atau operand operator

        * ternary
            note :
                "membutuhkan 3 operand"


            ## - operator aritmatika
                syntax :
                            + penjumlahan
                            - pengurangan
                            * perkalian
                            / pembagian
                            % mod

                note : operator precedence atau urutan operasi matematika

                urutan nya : () -> * -> / -> + -> -

            ## - operator penugasan/assignment
                syntax :
                        =
                        += sama seperti : x=x+y
                        -= sama seperti : x=x-y
                        *= sama seperti : x=x*y
                        /= sama seperti : x=x/y
                        %= sama seperti : x=x%y
                contoh :
                x = 10 arti nya x memiliki nilai 10


            ## - operator perbadingan/comparison
                syntax :
                    == sama dengan
                    != tidak sama dengan
                    === strict sama dengan
                    !=== strict tidak sama dengan
                    > lebih besar dari
                    < lebih kecil dari
                    >= lebih besar sama dengan
                    <= lebih kecil sama dengan


                menghasilkan boolean :
                    - true : benar
                    - false : salah

            ## - operator logika / logical
                syntax :
                    &&  : and
                    ||  : or
                    !   : not

                note :
                    "asal salah satu nya benar, pasti hasil nya true"
                contoh :
                    (x % 2 == 0) && (x < 10)

## belajar day #2 mod (1)

            ## - operator string
                syntax : +

                note :
                * memiliki 2 fungsi yaitu
                - jika operand nya adalah angka maka dia akan menjadi operator artimatika,
                - jika operand nya adalah string maka dia akan menjadi operator penggabung string/tulisan

                contoh :
                jika 10 + "10" hasil nya "1010"
                sedangkan 10 + 10 hasil nya 20

                10+10"10" -> "2010"
                tapi
                "10"+10+10 -> "101010"

            ## - operator typeof
                syntax : typeof(operand)

                contoh :
                    > typeof(10)    --> input
                    < "number"      --> mengembalikan

                note :
                    digunakan untuk mengetahui tipe data apa dari suatu nilai

            ## - operator kondisional
                syntax : (kondisi) ? benar : salah

                contoh:
                    (x % 2 == 0) ? "genap" : "ganjil"
                    jika kondisi nya bernilai true maka yang akan di kembalikan adalah tulisan genap dan jika bernilai false maka akan sebalik nya.

        # Tipe data pada javascript
            ## Tipe data (String)

                note : "tipe data string dalam javascript digunakan untuk merepresentasikan data tekstual/plaintext"

                syntax : "" atau ''

                contoh :
                "candra" atau 'kirana'

                    * escape character
                        note : jika ingin menulis
                        jum'at maka gunakan jum\'at
                        atau
                        "\"gerakan pungut sampah\" pada hari jum'at"

                        escape charcater    |     hasil
                        ------------------------------------------
                        \0                  |     karakter NULL
                        \'                  |     '
                        \"                  |     "
                        \\                  |     \
                        \n                  |     new line/baris baru
                        \t                  |     tab
                        \b                  |     backspace
                        \uXXXX              |     unicode


                    * unicode
                        unicode                 |     hasil
                        ------------------------------------------
                        \u00A9                  |     C
                        \u00AE                  |     R
                        \u00B1                  |     +
                        \u00B5                  |     u
                        \u2122                  |     TM
                        ...                     |     ...


                    * Concatenation konkatenasi
                        note : bisa membandingkan 2 buah string

                        contoh : "Candra Kirana"  == "candra kirana"
                        ->                    false


                    * .length (menghitung panjang string)

                        contoh : "Candra Kirana".length   //13

## belajar day #3 mod (1)

     # Tipe data pada javascript
            ## Tipe data (Boolean)

            note : "boolean adalah sebuah tipe data yang digunakan untuk merepresentasikan logika true atau false"

            contoh :
                var x = 10;
                arti nya variable x menyimpan nilai 10 maka hasil nya true

                jika

                "Candra" == "candra"
                maka akan menghasilkan false

                Boolean(10 < 20)
                Boolean(0)
                Boolean(-1)
                maka ketiga tersebut akan menghasilkan true, karna perbandingan nya benar


                truthy/true     |       falsy/false
                ---------------------------------
                true            |       false
                non-zero number |       0
                "string"        |       ""
                object          |       undefined
                arrays          |       null
                functions       |       NaN

                note :
                    "undefined adalah sebuah tipe yang dihasilkan ketika kita mendeklarasikan sebuah variable tapi kita blum mengisikan nilai nya"
                    "sedangkan null adalah nilai kosong yang bisa kita berikan pada suatu variable, dan bisa menulis var x=null"


            ## Variable

                note : "variable adalah sebuah tempat/wadah yang memiliki nama, yang digunakan untuk menyimpna nilai"
                "harus paham dulu [DEKLARASI, INISIALISASI, ASSIGNMENT]"

                    * Deklarasi yaitu mendaftarkan variable ke dalam lingkup yang sesuai
                    * Inisialisasi yaitu menyediakan memori untuk variable
                    * Assignment yaitu menetapkan nilai yang spesifik ke dalam variable

                    contoh :
                        var x; //deklarasi & inisialisasi
                        x = 20; // assignment

                    syntax deklarasi:
                    - var
                    - let
                    - const

                    format :
                     var 1gaboleh; X
                     var boleh1; ✔
                     atau
                     var ini_juga_boleh; ✔

                    jenis penulisan :
                    internal    : di satu file yang sama
                    eksternal   : di file yang berbeda
