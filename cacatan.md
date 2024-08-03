# JavaScript - 100 Day

## Day 1

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

    Note : "operator dalam javascript adalah sebuah simbol yang digunakan untuk melakukan operasi"

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
                simbol :
                            + penjumlahan
                            - pengurangan
                            * perkalian
                            / pembagian
                            % mod

                note : operator precedence atau urutan operasi matematika

                urutan nya : () -> * -> / -> + -> -

            ## - operator penugasan/assignment
                simbol :
                        =
                        += sama seperti : x=x+y
                        -= sama seperti : x=x-y
                        *= sama seperti : x=x*y
                        /= sama seperti : x=x/y
                        %= sama seperti : x=x%y
                contoh :
                x = 10 arti nya x memiliki nilai 10


            ## - operator perbadingan/comparison
                simbol :
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
                simbol :
                    &&  : and
                    ||  : or
                    !   : not

                note :
                    "asal salah satu nya benar, pasti hasil nya true"
                contoh :
                    (x % 2 == 0) && (x < 10)
