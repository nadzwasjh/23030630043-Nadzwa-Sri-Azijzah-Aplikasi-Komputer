# 23030630043_Nadzwa Sri Azijzah_MatE23_LaTex Mardown_Pertemuan 15&16
## NAMA  : NADZWA SRI AZIJZAH

## NIM   :        23030630043

## KELAS :  MATEMATIKA E 2023

# TUGAS &amp; Materi EMT ALJABAR - STATISTIKA 

# EMT untuk Perhitungan Aljabar

Pada notebook ini Anda belajar menggunakan EMT untuk melakukan
berbagai perhitungan terkait dengan materi atau topik dalam Aljabar.
Kegiatan yang harus Anda lakukan adalah sebagai berikut:


* 
Membaca secara cermat dan teliti notebook ini;

* 
Menerjemahkan teks bahasa Inggris ke Indonesia;

* 
Mencoba contoh-contoh peritungan (perintah EMT) dengan cara
* meng-ENTER setiap perintah EMT yang ada (pindahkan kursor ke baris
* perintah)

* 
Jika perlu Anda dapat memodifiksi perintah yang ada dan memberikan
* keterangan/penjelasan tambahan terkait hasilnya.

* 
Menyisipkan baris-baris perintah baru untuk mengerjakan soal-soal
* Aljabar dari file PDF yang saya berikan;

* 
Memberi catatan hasilnya.

* 
Jika perlu tuliskan soalnya pada teks notebook (menggunakan format
* LaTeX).

* 
Gunakan tampilan hasil semua perhitungan yang eksk atau simbolik
* dengan format LaTeX. (Seperti contoh-contoh pada notebook ini.)


## Contoh pertama

Menyederhanakan bentuk aljabar:


  6x^{-3}y^5\times -7x^2y^{-9}  

\>$&6\*x^(-3)\*y^5\*-7\*x^2\*y^(-9)


$$-\frac{42}{x\,y^4}$$Menjabarkan:


  (6x^{-3}+y^5) (-7x^2-y^{-9})  

\>$&showev('expand((6\*x^(-3)+y^5)\*(-7\*x^2-y^(-9))))


$${\it expand}\left(\left(-\frac{1}{y^9}-7\,x^2\right)\,\left(y^5+
 \frac{6}{x^3}\right)\right)=-7\,x^2\,y^5-\frac{1}{y^4}-\frac{6}{x^3
 \,y^9}-\frac{42}{x}$$## Baris Perintah

Baris perintah Euler terdiri dari satu atau beberapa perintah Euler
yang diakhiri dengan tanda titik koma ";" atau koma ",". Tanda titik
koma akan menghentikan hasil yang akan ditampilkan. Sehingga koma
setelah perintah terakhir bisa dihilangkan.


Baris perintah berikut hanya akan menampilkan hasil dari ekspresi,
melainkan bukan penugasan atau pun peritah format.


\>r:=2; h:=4; pi\*r^2\*h/3


    16.7551608191

Perintah harus dipisahkan dengan spasi. Baris perintah berikut akan
mencetak dua hasilnya.


\>pi\*2r\*h, %+2\*pi\*r\*h // Ingat tanda % menyatakan hasil perhitungan terakhir sebelumnya


    50.2654824574
    100.530964915

Baris perintah dieksekusi sesuai uruan saat pengguna menekan tombol
enter. Jadi, setiap kali Anda akan mendapatkan nilai baru.


\>x := 1;

\>x:= cos(x) // nilai cosinus (x dalam radian)


    0.540302305868

\>x:= cos (x)


    0.857553215846

Jika dua baris kode dihubungkan dengan "..." maka kedua baris tersebut
akan selalu dijalankan secara bersamaan.


\>x := 1.5; ...  
\>   x := (x+2/x)/2, x := (x+2/x)/2, x := (x+2/x)/2,


    1.41666666667
    1.41421568627
    1.41421356237

Tidak masalah menggunakan beberapa baris. Pastikan baris tersebut
diakhiri dengan "...".


\>x := 1.5; // komentar ditulis di sini sebelum ...  
\>   repeat xnew:=(x+2/x)/2; until xnew~=x; ...  
\>     x := xnew; ...  
\>   end; ...  
\>   x,


    1.41421356237

Struktur kondisional juga berfungsi.


\>if E^pi\>pi^E; then "Good Job, Nadzwa!", endif;


    Good Job, Nadzwa!

Ini juga merupakan cara yang baik untuk membagi perintah panjang
menjadi dua atau lebih baris. Anda bisa teksn Ctrl+Return untuk
membagi baris menjadi dua di posisi kursor saat ii=ni, atau Ctrl+Back
untuk menghubungkan baris-baris tersebut.


Untuk melipat semua baris multi-lines, tekanlah Ctrl+L. Kemudian
baris-baris berikutnya hanya akan terlihat jika salah satunya
mendapatkan fokus. Untuk melipat satu baris multi-line, mulailah
dengan "%+ ".


\>%+ x=4+5; ...  
\>  
Baris yang dimulai dengan %% akan sepenuhnya tidak terlihat.


81


Euler mendukung penggunaan loop dalam baris perintah, selama semuanya
muat dalam satu baris atau beberapa baris. Dalam program, batasan ini
tidak berlaku, tentu saja. Untuk informasi lebih lanjut, lihat
pengantar berikut.


\>x=1; for i=1 to 5; x := (x+2/x)/2, end; // menghitung akar 2


    Cannot assign to a value of type string.
    Error in:
    %+ x=4+5; %+ x=4+5; %+ x=4+5; %+ x=4+5; %+ x=4+5; %+ x=4+5; %+ ...
                  ^

Tidak masalah menggunakan beberapa baris. Pastikan baris tersebut
diakhiri dengan " ...".


\>x := 1.5; // comments go here before the ...  
\>   repeat xnew:=(x+2/x)/2; until xnew~=x; ...  
\>      x := xnew; ...  
\>   end; ...  
\>   x,


    1.41421356237

Struktur kondisional juga berfungsi.


\>if E^pi\>pi^E; then "Good Job, Nadzwa!", endif;


    Good Job, Nadzwa!

Ketika Anda menjalankan sebuah perintah, kursor bisa berada di posisi
mana saja dalam baris perintah. Anda bisa kembali ke perintah
sebelumnya atau melompat ke perintah berikutnya dengan tombol panah.
Atau Anda bisa mengklik bagian komentar di atas perintah untuk menuju
ke perintah tersebut. 


Saat Anda memindahkan kursor sepanjang baris, pasangan tanda kurung
atau tanda kurung bulat akan disorot. Selain itu, perhatikan baris
status. Setelah tanda kurung pembuka dari fungsi sqrt(), baris status
akan menampilkan teks bantuan untuk fungsi tersebut. Jalankan perintah
dengan tombol enter.


\>sqrt(sin(10°)/cos(20°))


    0.429875017772

Untuk melihat bantuan untuk perintah terbaru, buka jendela bantuan
dengan menekan F1. Di sana, Anda bisa memasukkan teks untuk mencari.
Pada baris kosong, bantuan untuk jendela bantuan akan ditampilkan.
Anda bisa menekan tombol escape untuk membersihkan baris tersebut atau
menutup jendela bantuan. 


Anda bisa mengklik dua kali pada perintah apa pun untuk membuka
bantuan untuk perintah tersebut. Cobalah mengklik dua kali pada
perintah exp di bawah ini di baris perintah.


\>exp(log(5.5))


    5.5

Anda juga bisa menyalin dan menempel di Euler. Gunakan Ctrl-C dan
Ctrl-V untuk ini. Untuk menandai teks, seret mouse atau gunakan shift
bersama dengan tombol panah. Selain itu, Anda bisa menyalin tanda
kurung yang disorot.


## Basic Syntax atau Sintaks Dasar

Euler mengenal fungsi matematika yang umum. Seperti yang telah Anda
lihat di atas, fungsi trigonometri bekerja dalam radian atau derajat.
Untuk mengonversi ke derajat, tambahkan simbol derajat (dengan tombol
F7) ke nilai, atau gunakan fungsi rad(x). Fungsi akar kuadrat disebut
sqrt di Euler. Tentu saja, x^(1/2) juga bisa digunakan. 


Untuk mengatur variabel, gunakan "=" atau ":=". Untuk kejelasan,
pengantar ini menggunakan bentuk yang terakhir. Spasi tidak
mempengaruhi. Namun, spasi antara perintah diharapkan ada. 


Beberapa perintah dalam satu baris dipisahkan dengan "," atau ";".
Titik koma menekan output perintah. Di akhir baris perintah, sebuah
"," diasumsikan jika ";" hilang.


\>g:=10; t:=3; 1/2\*g\*t^2


    45

EMT menggunakan sintaks pemrograman untuk ekspresi. Untuk memasukkan


  e^2 \cdot \left( \frac{1} {3+4 \log(0.6)}+\frac{1}{7} \right)  

Anda harus menyetel tanda kurung yang benar dan menggunakan / untuk
pecahan. Perhatikan tanda kurung yang disorot untuk bantuan. Perlu
dicatat bahwa konstanta Euler e disebut E dalam EMT.


\>E^2\*(1/(3+4\*log(0.6))+1/7)


    8.77908249441

Untuk menghitung ekspresi yang rumit seperti


Anda perlu memasukkannya dalam bentuk baris.


\>((1/7 + 1/8 + 2) / (1/3 + 1/2))^2 \* pi


    23.2671801626

Letakkan tanda kurung dengan hati-hati di sekitar sub-ekspresi yang
perlu dihitung terlebih dahulu. EMT membantu Anda dengan menyorot
ekspresi yang diakhiri oleh tanda kurung penutup. Anda juga harus
memasukkan nama "pi" untuk huruf Yunani pi. 


Hasil dari perhitungan ini adalah angka floating point. Secara
default, hasil tersebut dicetak dengan akurasi sekitar 12 digit. Pada
baris perintah berikutnya, kita juga akan belajar bagaimana kita bisa
merujuk ke hasil sebelumnya dalam baris yang sama.


\>1/3+1/7, fraction %


    0.47619047619
    10/21

Sebuah perintah Euler bisa berupa ekspresi atau perintah primitif.
Ekspresi terdiri dari operator dan fungsi. Jika perlu, harus
mengandung tanda kurung untuk memaksa urutan eksekusi yang benar. Jika
ragu, menambahkan tanda kurung adalah ide yang baik. Perlu dicatat
bahwa EMT menunjukkan tanda kurung pembuka dan penutup saat mengedit
baris perintah.


\>(cos(pi/6)+1)^3\*(sin(pi/2)+1)^2


    25.9903810568

Operator numerik di Euler meliputi


+ penjumlahan atau operator plus


- pengurangan atau operator minus


*, /


. produk matriks


a^b pangkat untuk a positif atau b bilangan bulat (a**b juga
berfungsi) n! operator faktorial


dan masih banyak lagi.


Berikut beberapa fungsi yang mungkin Anda butuhkan. Masih banyak lagi.


   sin,cos,tan,atan,asin,acos,rad,deg  
   log,exp,log10,sqrt,logbase  
   bin,logbin,logfac,mod,floor,ceil,round,abs,sign  
   conj,re,im,arg,conj,real,complex  
   beta,betai,gamma,complexgamma,ellrf,ellf,ellrd,elle  
   bitand,bitor,bitxor,bitnot  

Beberapa perintah memiliki alias, misalnya ln untuk log.


\>ln(E^2), arctan(tan(1))


    2
    1

\>sin(90°)


    1

Pastikan untuk menggunakan tanda kurung (kurung bulat) setiap kali ada
keraguan tentang urutan eksekusi! Yang berikut ini tidak sama dengan
(2^3)^4, yang merupakan default untuk 2^3^4 dalam EMT (beberapa sistem
numerik melakukannya dengan cara sebaliknya).


\>2^4^2, (2^4)^2, 2^(4^2)


    65536
    256
    65536

## Bilangan Rill

Tipe data utama di Euler adalah bilangan riil. Bilangan riil
direpresentasikan dalam format IEEE dengan akurasi sekitar 16 digit
desimal.


\>longest 7/3


          2.333333333333333 

Representasi internal ganda memerlukan 8 byte.


\>printdual(7/3)


    1.0010101010101010101010101010101010101010101010101011*2^1

\>printhex(7/3)


    2.5555555555556*16^0

## String

Sebuah string di Euler didefinisikan dengan "...".


\>"Nadzwa Sri Azijzah."


    Nadzwa Sri Azijzah.

String dapat digabungkan dengan | atau dengan +. Ini juga berlaku
untuk angka, yang dikonversi menjadi string dalam kasus tersebut.


\>"Luas suatu daerah dengan radius " + 3 + " adalah " + pi\*2 + " cm^2."


    Luas suatu daerah dengan radius 3 adalah 6.28318530718 cm^2.

Fungsi print juga mengonversi angka menjadi string. Fungsi ini dapat
menerima jumlah digit dan jumlah tempat (0 untuk output padat), serta
idealnya sebuah unit.


\>"Tinggi badanku : " + print((1+sqrt(100000))/2,6,0)


    Tinggi badanku : 158.613883

Ada string khusus bernama none, yang tidak dicetak. String ini
dikembalikan oleh beberapa fungsi ketika hasilnya tidak penting. (Ini
dikembalikan secara otomatis jika fungsi tersebut tidak memiliki
pernyataan return.)


\>none


Untuk mengonversi string menjadi angka, cukup evaluasi string
tersebut. Ini juga berlaku untuk ekspresi (lihat di bawah).


\>"1234.5"()


    1234.5

Untuk mendefinisikan vektor string, gunakan notasi vektor [...].


\>v:=["Nadzwa","suka","melukis"]


    Nadzwa
    suka
    melukis

Vektor string kosong dilambangkan dengan [none]. Vektor string dapat
digabungkan.


\>w:=[none]; w|v|v


    Nadzwa
    suka
    melukis
    Nadzwa
    suka
    melukis

String dapat berisi karakter Unicode. Secara internal, string ini
menggunakan kode UTF-8. Untuk menghasilkan string seperti itu, gunakan
u"..." dan salah satu entitas HTML. 


String Unicode dapat digabungkan seperti string lainnya.


\>u"&alpha; = " + 45 + u"&deg;" // pdfLaTeX mungkin gagal menampilkan secara benar


    α = 45°

I


Dalam komentar, entitas yang sama seperti a, ß, dll. dapat digunakan.
Ini bisa menjadi alternatif cepat untuk LaTeX. (Detail lebih lanjut
tentang komentar di bawah).


Ada beberapa fungsi untuk membuat atau menganalisis string Unicode.
Fungsi strtochar() akan mengenali string Unicode dan menerjemahkannya
dengan benar.


\>v=strtochar(u"&Auml; is a German letter")


    [196,  32,  105,  115,  32,  97,  32,  71,  101,  114,  109,  97,  110,
    32,  108,  101,  116,  116,  101,  114]

Hasilnya adalah vektor angka Unicode. Fungsi kebalikannya adalah
chartoutf().


\>v[1]=strtochar(u"&Uuml;")[1]; chartoutf(v)


    Ü is a German letter

Fungsi utf() dapat menerjemahkan string dengan entitas dalam sebuah
variabel menjadi string Unicode.


\>s="We have &alpha;=&beta;."; utf(s) // pdfLaTeX mungkin gagal menampilkan secara benar


    We have α=β.

Juga memungkinkan untuk menggunakan entitas numerik.


\>u"&#196;hnliches"


    Ähnliches

## Nilai Boolean

Nilai Boolean direpresentasikan dengan 1=true atau 0=false di Euler. %
String dapat dibandingkan, sama seperti angka.


\>5<9, "jeruk"<"mangga"


    1
    1

 "and" adalah operator "&amp;&amp;" dan "or" adalah operator "||", seperti  

dalam bahasa C. (Kata "and" dan "or" hanya dapat digunakan dalam
kondisi untuk "if".)


\>2<E && E<3


    1

Operator Boolean mengikuti aturan bahasa matriks.


\>(1:10)\>5, nonzeros(%)


    [0,  0,  0,  0,  0,  1,  1,  1,  1,  1]
    [6,  7,  8,  9,  10]

Anda bisa menggunakan fungsi nonzeros() untuk mengekstrak elemen
tertentu dari sebuah vektor. Dalam contoh ini, kita menggunakan
kondisi isprime(n).


\>N=2|3:2:99 // N berisi elemen 2 dan bilangan2 ganjil dari 3 s.d. 99


    [2,  3,  5,  7,  9,  11,  13,  15,  17,  19,  21,  23,  25,  27,  29,
    31,  33,  35,  37,  39,  41,  43,  45,  47,  49,  51,  53,  55,  57,
    59,  61,  63,  65,  67,  69,  71,  73,  75,  77,  79,  81,  83,  85,
    87,  89,  91,  93,  95,  97,  99]

\>N[nonzeros(isprime(N))] //pilih anggota2 N yang prima


    [2,  3,  5,  7,  11,  13,  17,  19,  23,  29,  31,  37,  41,  43,  47,
    53,  59,  61,  67,  71,  73,  79,  83,  89,  97]

## Format Output

Format output/hasil default EMT mencetak 12 digit. Untuk memastikan
bahwa kita melihat format default, kita mereset format tersebut.


\>defformat; pi/2


    1.57079632679

Secara internal, EMT menggunakan standar IEEE untuk angka ganda dengan
akurasi sekitar 16 digit desimal. Untuk melihat jumlah digit secara
penuh, gunakan perintah "longestformat", atau kita dapat menggunakan
operator "longest" untuk menampilkan hasil dalam format terpanjang.


\>longest pi


          3.141592653589793 

Berikut adalah representasi internal heksadesimal dari angka ganda.


\>printhex(pi)


    3.243F6A8885A30*16^0

Format output dapat diubah secara permanen dengan perintah format.


\>format(12,5); 1/3, pi, sin(1)


        0.33333 
        3.14159 
        0.84147 

Default-nya adalah format(12).


\>format(12); 1/3


    0.333333333333

Fungsi seperti "shortestformat", "shortformat", dan "longformat"
bekerja untuk vektor dengan cara berikut.


\>setscalarformat(5); pi


    3.1416

Fungsi "longestformat" juga mengatur format skalar.


\>longestformat; pi


    3.141592653589793

Sebagai referensi, berikut adalah daftar format keluaran yang paling
penting.


shortestformat shortformat longformat, longestformat 


format(length,digits) goodformat(length)


fracformat(length)


defformat


Akurasi internal EMT sekitar 16 tempat desimal, sesuai dengan standar
IEEE. Angka disimpan dalam format internal ini. 


Namun, format keluaran EMT dapat diatur dengan cara yang fleksibel.


\>longestformat; pi,


    3.141592653589793

\>format(10,5); pi


      3.14159 

Default-nya adalah defformat().


\>defformat; // default


Ada operator singkat yang hanya mencetak satu nilai. Operator
"longest" akan mencetak semua digit valid dari sebuah angka.


\>longest pi^2/2


          4.934802200544679 

Ada juga operator singkat untuk mencetak hasil dalam format pecahan.
Kita sudah menggunakannya di atas.


\>fraction 1+1/2+1/3+1/4


    25/12

Karena format internal menggunakan cara biner untuk menyimpan angka,
nilai 0.1 tidak akan direpresentasikan secara tepat. Kesalahan ini
bertambah sedikit demi sedikit, seperti yang Anda lihat dalam
perhitungan berikut.


\>longest 0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1-1


     -1.110223024625157e-16 

Namun dengan "longformat" default Anda tidak akan menyadarinya. Untuk
kenyamanan, keluaran angka yang sangat kecil adalah 0.


\>0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1-1


    0

# Expressions

Nama atau teks (string) bisa digunakan untuk menyimpan persamaan
matematika yang bisa dihitung oleh EMT. Untuk melakukannya, gunakan
tanda kurung setelah persamaannya. Jika ingin menggunakan teks sebagai
persamaan, gunakan aturan penamaan seperti "fx" atau "fxy", dan
sebagainya. Persamaan ini memiliki prioritas lebih tinggi dibandingkan
fungsi.


Variabel global juga bisa digunakan saat melakukan perhitungan.


\>r:=2; fx:="pi\*r^2"; longest fx()


          12.56637061435917 

Parameter diberikan ke x, y, dan z secara berurutan. Parameter
tambahan bisa ditambahkan menggunakan parameter yang sudah ditetapkan.


\>fx:="a\*sin(x)^2"; fx(5,a=-1)


    -0.919535764538

Perlu diingat bahwa ekspresi akan selalu menggunakan variabel global,


meskipun ada variabel dengan nama yang sama di dalam fungsi. (Jika


tidak, perhitungan ekspresi dalam fungsi bisa menghasilkan hasil yang


membingungkan bagi pengguna yang memanggil fungsi tersebut.)


\>at:=4; function f(expr,x,at) := expr(x); ...  
\>   f("at\*x^2",3,5) // computes 4\*3^2 not 5\*3^2


    36

Jika ingin menggunakan nilai lain untuk "at" selain dari nilai global,


kamu perlu menambahkan "at=nilai".


\>at:=4; function f(expr,x,a) := expr(x,at=a); ...  
\>   f("at\*x^2",3,5)


    45

Sebagai referensi, perlu dicatat bahwa kumpulan panggilan (dibahas di
tempat lain) bisa berisi ekspresi. Jadi, kita bisa membuat contoh di
atas seperti berikut.


am fungsi bisa menghasilkan hasil yang membingungkan bagi pengguna
yang memanggil fungsi tersebut.)


\>at:=4; function f(expr,x) := expr(x); ...  
\>   f({{"at\*x^2",at=5}},3)


    45

Ekspresi pada x sering digunakan seperti fungsi.


erlu diingat bahwa jika kamu mendefinisikan fungsi dengan nama yang
sama seperti ekspresi simbolik global, variabel tersebut akan dihapus
untuk menghindari kebingungan antara ekspresi simbolik dan fungsi.


\>f &= 5\*x;

\>function f(x) := 6\*x;

\>f(2)


    12

Sebagai aturan, ekspresi simbolik atau numerik sebaiknya diberi nama
seperti fx, fxy, dan sebagainya. Skema penamaan ini tidak boleh
digunakan untuk fungsi.


\>fx &= diff(x^x,x); $&fx


$$x^{x}\,\left(\log x+1\right)$$Ada bentuk khusus dari ekspresi yang memungkinkan penggunaan variabel
apa pun sebagai parameter tanpa nama saat menghitung ekspresi, tidak
hanya "x", "y", dan sebagainya. Untuk ini, mulailah ekspresi dengan
"@(variabel) ...".


\>"@(a,b) a^2+b^2", %(4,5)


    @(a,b) a^2+b^2
    41

Ini memungkinkan untuk memanipulasi ekspresi dengan variabel lain
dalam fungsi EMT yang memerlukan ekspresi di "x".


Cara paling sederhana untuk mendefinisikan fungsi adalah dengan
menyimpan rumusnya dalam ekspresi simbolik atau numerik. Jika variabel
utamanya adalah x, ekspresi tersebut bisa dihitung seperti fungsi.


Seperti yang terlihat pada contoh berikut, variabel global dapat
terlihat selama perhitungan.


\>fx &= x^3-a\*x;  ...  
\>   a=1.2; fx(0.5)


    -0.475

Semua variabel lain dalam ekspresi bisa ditentukan dalam perhitungan
menggunakan parameter yang telah ditetapkan.


\>fx(0.5,a=1.1)


    -0.425

Ekspresi tidak harus simbolik. Ini diperlukan jika ekspresi mengandung
fungsi yang hanya dikenal di kernel numerik, bukan di Maxima.


# Matematika Simbolik

EMT melakukan matematika simbolik dengan bantuan Maxima. Untuk detail
lebih lanjut, mulailah dengan tutorial berikut atau lihat referensi
untuk Maxima. Para ahli Maxima harus memperhatikan bahwa ada perbedaan
dalam sintaks antara sintaks asli Maxima dan sintaks default ekspresi
simbolik di EMT.


Matematika simbolik terintegrasi secara mulus ke dalam Euler dengan
menggunakan &amp;. Setiap ekspresi yang diawali dengan &amp; adalah ekspresi
simbolik. Ekspresi tersebut dihitung dan dicetak oleh Maxima.


Pertama-tama, Maxima memiliki aritmetika "tak hingga" yang dapat
menangani angka yang sangat besar.


\>$&33!


$$8683317618811886495518194401280000000$$Dengan cara ini, Anda bisa menghitung hasil besar secara tepat. Mari
kita hitung


Latex: C(44,10) = \frac{44!}{34! \cdot 10!}


\>$& 33!/(24!\*10!) // nilai C(33,10)


$$3856710$$Tentu saja, Maxima memiliki fungsi yang lebih efisien untuk ini
(begitu juga dengan bagian numerik dari EMT).


\>$binomial(44,10) //menghitung C(44,10) menggunakan fungsi binomial()


$$2481256778$$Untuk mempelajari lebih lanjut tentang fungsi tertentu, klik dua kali
pada fungsi tersebut. Misalnya, coba klik dua kali pada "&amp;binomial" di
baris perintah sebelumnya. Ini akan membuka dokumentasi Maxima yang
disediakan oleh pembuat program tersebut.


Kamu juga akan belajar bahwa hal berikut ini juga bisa dilakukan.


Latex: C(x,3)=\frac{x!}{(x-3)!3!}=\frac{(x-2)(x-1)x}{6}


\>$binomial(x,3) // C(x,3)


$$\frac{\left(x-2\right)\,\left(x-1\right)\,x}{6}$$Jika kamu ingin mengganti x dengan nilai tertentu, gunakan "with".


\>$&binomial(x,3) with x=10 // substitusi x=10 ke C(x,3)


$$120$$Dengan cara ini, kamu bisa menggunakan solusi dari satu persamaan
dalam persamaan lainnya.


Ekspresi simbolik dicetak oleh Maxima dalam bentuk 2D. Ini disebabkan
oleh sebuah tanda simbolik khusus dalam string.


Seperti yang akan kamu lihat dalam contoh sebelumnya dan berikutnya,
jika kamu memiliki LaTeX terinstal, kamu bisa mencetak ekspresi
simbolik dengan LaTeX. Jika tidak, perintah berikut akan menghasilkan
pesan kesalahan.


Untuk mencetak ekspresi simbolik dengan LaTeX, gunakan $ di depan &amp;
(atau kamu bisa menghilangkan &amp;) sebelum perintah. Jangan jalankan
perintah Maxima dengan $, jika kamu tidak memiliki LaTeX terinstal.


\>$(3+x)/(x^2+1)


$$\frac{x+3}{x^2+1}$$Ekspresi simbolik diproses oleh Euler. Jika kamu memerlukan sintaks
yang kompleks dalam satu ekspresi, kamu bisa membungkus ekspresi
tersebut dalam "...". Menggunakan lebih dari sekadar ekspresi
sederhana dimungkinkan, tetapi sangat tidak disarankan.


\>&"v := 5; v^2"


    
                                      25
    

Untuk melengkapi, perlu dicatat bahwa ekspresi simbolik bisa digunakan
dalam program, tetapi harus dibungkus dalam tanda kutip. Selain itu,
lebih efektif untuk memanggil Maxima saat waktu kompilasi jika
memungkinkan.


\>$&expand((1+x)^4), $&factor(diff(%,x)) // diff: turunan, factor: faktor


$$x^4+4\,x^3+6\,x^2+4\,x+1$$$$4\,\left(x+1\right)^3$$Sekali lagi, % mengacu pada hasil sebelumnya.


Untuk mempermudah, kita simpan solusi ke dalam variabel simbolik.
Variabel simbolik didefinisikan dengan "&amp;=".


\>fx &= (x+1)/(x^4+1); $&fx


$$\frac{x+1}{x^4+1}$$Ekspresi simbolik bisa digunakan dalam ekspresi simbolik lainnya.


\>$&factor(diff(fx,x))


$$\frac{-3\,x^4-4\,x^3+1}{\left(x^4+1\right)^2}$$\>&factor(15!)


    
                                1307674368000
    

\>::: factor(30!)


    
                       26  14  7  4   2   2
                      2   3   5  7  11  13  17 19 23 29
    

\>:: factor(20!)


    
                            18  8  4  2
                           2   3  5  7  11 13 17 19
    

Jika kamu ahli dalam Maxima, kamu mungkin ingin menggunakan sintaks
asli Maxima. Kamu bisa melakukannya dengan ":::"


\>::: av:g$ av^2;


    
                                       2
                                      g
    

\>fx &= x^3\*exp(x), $fx


    
                                     3  x
                                    x  E
    

$$x^3\,e^{x}$$Variabel seperti itu bisa digunakan dalam ekspresi simbolik lainnya.
Perhatikan bahwa dalam perintah berikut, sisi kanan dari &amp;= dihitung
terlebih dahulu sebelum penugasan ke Fx.


\>&(fx with x=5), $%, &float(%)


    
                                         5
                                    125 E
    

$$125\,e^5$$    
                              18551.64488782208
    

\>$factor(diff(fx,x,2))


$$x\,\left(x^2+6\,x+6\right)\,e^{x}$$Untuk mendapatkan kode LaTeX dari sebuah ekspresi, kamu bisa
menggunakan perintah tex.


\>tex(fx)


    x^3\,e^{x}

Ekspresi simbolik bisa dihitung seperti ekspresi numerik.


\>fx(0.5)


    0.206090158838

Dalam ekspresi simbolik, ini tidak berfungsi karena Maxima tidak
mendukungnya. Sebagai gantinya, gunakan sintaks "with" (bentuk yang
lebih baik dari perintah at(...) di Maxima).


\>$&fx with x=1/2


$$\frac{\sqrt{e}}{8}$$Penugasan juga bisa bersifat simbolik.


\>$&fx with x=1+t


$$\left(t+1\right)^3\,e^{t+1}$$Perintah solve menyelesaikan ekspresi simbolik untuk sebuah variabel
di Maxima. Hasilnya adalah vektor dari solusi.


\>$&solve(x^2+x=4,x)


$$\left[ x=\frac{-\sqrt{17}-1}{2} , x=\frac{\sqrt{17}-1}{2} \right] $$Bandingkan dengan perintah "solve" numerik di Euler, yang memerlukan
nilai awal, dan opsionalnya nilai target.


\>solve("x^2+x",1,y=4)


    1.56155281281

Nilai numerik dari solusi simbolik bisa dihitung dengan mengevaluasi
hasil simbolik tersebut. Euler akan mengabaikan penugasan seperti x=
dan sebagainya. Jika kamu tidak memerlukan hasil numerik untuk
perhitungan selanjutnya, kamu juga bisa membiarkan Maxima menemukan
nilai numeriknya.


\>sol &= solve(x^2+2\*x=4,x); $&sol, sol(), $&float(sol)


$$\left[ x=-\sqrt{5}-1 , x=\sqrt{5}-1 \right] $$    [-3.23607,  1.23607]

$$\left[ x=-3.23606797749979 , x=1.23606797749979 \right] $$Untuk mendapatkan solusi simbolik tertentu, kamu bisa menggunakan
"with" dan sebuah indeks.


\>$&solve(x^2+x=1,x), x2 &= x with %[2]; $&x2


$$\left[ x=\frac{-\sqrt{5}-1}{2} , x=\frac{\sqrt{5}-1}{2} \right] $$$$\frac{\sqrt{5}-1}{2}$$Untuk menyelesaikan sistem persamaan, gunakan vektor persamaan.
Hasilnya adalah vektor dari solusi.


\>sol &= solve([x+y=3,x^2+y^2=5],[x,y]); $&sol, $&x\*y with sol[1]


$$\left[ \left[ x=2 , y=1 \right]  , \left[ x=1 , y=2 \right] 
  \right] $$$$2$$Ekspresi simbolik bisa memiliki tanda (flags), yang menunjukkan
perlakuan khusus di Maxima. Beberapa tanda bisa digunakan sebagai
perintah juga, sementara yang lain tidak bisa. Tanda ditambahkan
dengan "|" (bentuk yang lebih baik dari "ev(...,flags)").


\>$& diff((x^3-1)/(x+1),x) //turunan bentuk pecahan


$$\frac{3\,x^2}{x+1}-\frac{x^3-1}{\left(x+1\right)^2}$$\>$& diff((x^3-1)/(x+1),x) | ratsimp //menyederhanakan pecahan


$$\frac{2\,x^3+3\,x^2+1}{x^2+2\,x+1}$$\>$&factor(%)


$$\frac{2\,x^3+3\,x^2+1}{\left(x+1\right)^2}$$# Fungsi

Di EMT, fungsi adalah program yang didefinisikan dengan perintah
"function". Fungsi bisa berupa satu baris atau beberapa baris.


Fungsi satu baris bisa bersifat numerik atau simbolik. Fungsi satu
baris numerik didefinisikan dengan ":=".


\>function f(x) := x\*sqrt(x^2+1)


Untuk gambaran umum, kami menunjukkan semua kemungkinan definisi untuk
fungsi satu baris. Fungsi ini bisa dihitung seperti fungsi bawaan
Euler lainnya.


\>f(4)


    16.4924225025

Fungsi ini juga akan berfungsi untuk vektor, mengikuti bahasa matriks
Euler, karena ekspresi yang digunakan dalam fungsi tersebut telah
diproses untuk vektor.


\>f(0:0.1:1)


    [0,  0.100499,  0.203961,  0.313209,  0.430813,  0.559017,  0.699714,
    0.854459,  1.0245,  1.21083,  1.41421]

Fungsi bisa digambar. Alih-alih memberikan ekspresi, kita hanya perlu
memberikan nama fungsi.


Berbeda dengan ekspresi simbolik atau numerik, nama fungsi harus
diberikan dalam bentuk string.


\>solve("f",1,y=1)


    0.786151377757

Secara default, jika kamu perlu menimpa fungsi bawaan, kamu harus
menambahkan kata kunci "overwrite". Menimpa fungsi bawaan bisa
berbahaya dan dapat menyebabkan masalah bagi fungsi lain yang
bergantung padanya.


Kamu masih bisa memanggil fungsi bawaan dengan menggunakan "_..." jika
itu adalah fungsi di inti Euler.


\>function overwrite sin (x) := \_sin(x°) // redine sine in degrees

\>sin(90)


    1

Lebih baik kita hapus penetapan ulang fungsi sin ini.


\>forget sin; sin(pi/2)


    1

## Parameter Bawaan

Fungsi numerik bisa memiliki parameter bawaan.


\>function f(x,a=4) := a\*x^2


Jika parameter ini diabaikan, nilai bawaan akan digunakan.


\>f(6)


    144

Menetapkannya akan menggantikan nilai bawaan.


\>f(6,7)


    252

Parameter yang ditetapkan juga menggantikan nilai bawaan. Ini
digunakan oleh banyak fungsi Euler seperti plot2d, plot3d.


\>f(6,a=4)


    144

Jika sebuah variabel bukan parameter, variabel tersebut harus bersifat
global. Fungsi satu baris bisa mengakses variabel global.


\>function f(x) := a\*x^2

\>a=4; f(2)


    16

Namun, parameter yang ditetapkan akan menggantikan nilai global.


Jika argumen tidak ada dalam daftar parameter yang sudah ditentukan,
ia harus dideklarasikan dengan ":="!


\>f(3,a:=6)


    54

Fungsi simbolik didefinisikan dengan "&amp;=". Mereka didefinisikan di
Euler dan Maxima, dan berfungsi di kedua lingkungan tersebut. Ekspresi
yang mendefinisikannya diproses melalui Maxima sebelum definisi
diterapkan.


\>function g(x) &= x^3-x\*exp(-x); $&g(x)


$$x^3-x\,e^ {- x }$$Fungsi simbolik bisa digunakan dalam ekspresi simbolik.


\>$&diff(g(x),x), $&% with x=4/3


$$x\,e^ {- x }-e^ {- x }+3\,x^2$$$$\frac{e^ {- \frac{4}{3} }}{3}+\frac{16}{3}$$Fungsi simbolik juga bisa digunakan dalam ekspresi numerik. Tentu
saja, ini hanya akan berhasil jika EMT dapat menginterpretasikan semua
yang ada di dalam fungsi tersebut.


\>g(5+g(1))


    178.635099908

Fungsi simbolik bisa digunakan untuk mendefinisikan fungsi simbolik
atau ekspresi lainnya.


\>function G(x) &= factor(integrate(g(x),x)); $&G(c) // integrate: mengintegralkan


$$\frac{e^ {- c }\,\left(c^4\,e^{c}+4\,c+4\right)}{4}$$\>solve(&g(x),0.5)


    0.703467422498

Yang berikut ini juga berhasil, karena Euler menggunakan ekspresi
simbolik dalam fungsi g jika tidak menemukan variabel simbolik g, dan
jika ada fungsi simbolik g.


\>solve(&g,0.5)


    0.703467422498

\>function P(x,n) &= (2\*x-1)^n; $&P(x,n)


$$\left(2\,x-1\right)^{n}$$\>function Q(x,n) &= (x+2)^n; $&Q(x,n)


$$\left(x+2\right)^{n}$$\>$&P(x,4), $&expand(%)


$$\left(2\,x-1\right)^4$$$$16\,x^4-32\,x^3+24\,x^2-8\,x+1$$\>P(3,4)


    625

\>$&P(x,4)+ Q(x,3), $&expand(%)


$$\left(2\,x-1\right)^4+\left(x+2\right)^3$$$$16\,x^4-31\,x^3+30\,x^2+4\,x+9$$\>$&P(x,4)-Q(x,3), $&expand(%), $&factor(%)


$$\left(2\,x-1\right)^4-\left(x+2\right)^3$$$$16\,x^4-33\,x^3+18\,x^2-20\,x-7$$$$16\,x^4-33\,x^3+18\,x^2-20\,x-7$$\>$&P(x,4)\*Q(x,3), $&expand(%), $&factor(%)


$$\left(x+2\right)^3\,\left(2\,x-1\right)^4$$$$16\,x^7+64\,x^6+24\,x^5-120\,x^4-15\,x^3+102\,x^2-52\,x+8$$$$\left(x+2\right)^3\,\left(2\,x-1\right)^4$$\>$&P(x,4)/Q(x,1), $&expand(%), $&factor(%)


$$\frac{\left(2\,x-1\right)^4}{x+2}$$$$\frac{16\,x^4}{x+2}-\frac{32\,x^3}{x+2}+\frac{24\,x^2}{x+2}-\frac{8
 \,x}{x+2}+\frac{1}{x+2}$$$$\frac{\left(2\,x-1\right)^4}{x+2}$$\>function f(x) &= x^3-x; $&f(x)


$$x^3-x$$Dengan &amp;=, fungsi tersebut bersifat simbolik dan bisa digunakan dalam
ekspresi simbolik lainnya.


\>$&integrate(f(x),x)


$$\frac{x^4}{4}-\frac{x^2}{2}$$Dengan :=, fungsi tersebut bersifat numerik. Contoh yang baik adalah
integral tertentu seperti


yang tidak bisa dihitung secara simbolik.


Jika kita mendefinisikan ulang fungsi dengan kata kunci "map," fungsi
tersebut dapat digunakan untuk vektor x. Secara internal, fungsi akan
dipanggil untuk semua nilai x satu kali, dan hasilnya disimpan dalam
vektor.


\>function map f(x) := integrate("x^x",1,x)

\>f(0:0.5:2)


    [-0.783431,  -0.410816,  0,  0.676863,  2.05045]

Fungsi bisa memiliki nilai bawaan untuk parameter.


\>function mylog (x,base=10) := ln(x)/ln(base);


Sekarang fungsi tersebut bisa dipanggil dengan atau tanpa parameter
"base".


\>mylog(100), mylog(2^6.7,2)


    2
    6.7

Selain itu, kamu bisa menggunakan parameter yang ditetapkan.


\>mylog(E^2,base=E)


    2

Seringkali, kita ingin menggunakan fungsi untuk vektor di satu tempat,
dan untuk elemen individual di tempat lain. Ini bisa dilakukan dengan
parameter vektor.


\>function f([a,b]) &= a^2+b^2-a\*b+b; $&f(a,b), $&f(x,y)


$$b^2-a\,b+b+a^2$$$$y^2-x\,y+y+x^2$$Fungsi simbolik seperti itu bisa digunakan untuk variabel simbolik.


Tapi fungsi tersebut juga bisa digunakan untuk vektor numerik.


\>v=[3,4]; f(v)


    17

Ada juga fungsi yang sepenuhnya simbolik, yang tidak bisa digunakan
secara numerik.


\>function lapl(expr,x,y) &&= diff(expr,x,2)+diff(expr,y,2)//turunan parsial kedua


    
                     diff(expr, y, 2) + diff(expr, x, 2)
    

\>$&realpart((x+I\*y)^4), $&lapl(%,x,y)


$$y^4-6\,x^2\,y^2+x^4$$$$0$$Namun, tentu saja, fungsi ini bisa digunakan dalam ekspresi simbolik
atau dalam definisi fungsi simbolik.


\>function f(x,y) &= factor(lapl((x+y^2)^5,x,y)); $&f(x,y)


$$10\,\left(y^2+x\right)^3\,\left(9\,y^2+x+2\right)$$Untuk merangkum:


&amp;= mendefinisikan fungsi simbolik,


= mendefinisikan fungsi numerik,


&amp;= mendefinisikan fungsi yang sepenuhnya simbolik.


# Menyelesaikan Ekspresi

Ekspresi bisa diselesaikan secara numerik dan simbolik.


Untuk menyelesaikan ekspresi sederhana dengan satu variabel, kita bisa
menggunakan fungsi solve(). Fungsi ini memerlukan nilai awal untuk
memulai pencarian. Secara internal, solve() menggunakan metode sekant.


\>solve("x^2-2",3)


    1.41421356237

Ini juga berlaku untuk ekspresi simbolik. Ambil contoh fungsi berikut.


\>$&solve(x^2=2,x)


$$\left[ x=-\sqrt{2} , x=\sqrt{2} \right] $$\>$&solve(x^2-2,x)


$$\left[ x=-\sqrt{2} , x=\sqrt{2} \right] $$\>$&solve(a\*x^2+b\*x+c=0,x)


$$\left[ x=\frac{-\sqrt{b^2-4\,a\,c}-b}{2\,a} , x=\frac{\sqrt{b^2-4\,
 a\,c}-b}{2\,a} \right] $$\>$&solve([a\*x+b\*y=c,d\*x+e\*y=f],[x,y])


$$\left[ \left[ x=-\frac{c\,e}{b\,\left(d-5\right)-a\,e} , y=\frac{c
 \,\left(d-5\right)}{b\,\left(d-5\right)-a\,e} \right]  \right] $$\>px &= 4\*x^8+x^7-x^4-x; $&px


$$4\,x^8+x^7-x^4-x$$Sekarang kita mencari titik di mana polinomialnya adalah 2. Dalam
solve(), nilai target default y=0 bisa diubah dengan variabel yang
ditetapkan. Kita gunakan y=2 dan periksa dengan mengevaluasi
polinomial pada hasil sebelumnya.


\>solve(px,1,y=2), px(%)


    0.966715594851
    2

Menyelesaikan ekspresi simbolik dalam bentuk simbolik menghasilkan
daftar solusi. Kita menggunakan pemecah simbolik solve() yang
disediakan oleh Maxima.


\>sol &= solve(x^2-x-1,x); $&sol


$$\left[ x=\frac{1-\sqrt{5}}{2} , x=\frac{\sqrt{5}+1}{2} \right] $$Cara termudah untuk mendapatkan nilai numerik adalah dengan
mengevaluasi solusi secara numerik seperti ekspresi.


\>longest sol()


        -0.6180339887498949       1.618033988749895 

Untuk menggunakan solusi secara simbolik dalam ekspresi lain, cara
termudah adalah dengan "with".


\>                                       


    &x^2 with sol[1], $&expand(x^2-x-1 with sol[2])
    &x^2 with sol[1], $&expand(x^2-x-1 with sol[2]) ...
</pre>
Menyelesaikan sistem persamaan secara simbolik bisa dilakukan dengan
vektor persamaan dan pemecah simbolik solve(). Jawabannya adalah
daftar dari daftar persamaan.


\>$&solve([x+y=2,x^3+2\*y+x=4],[x,y])


$$\left[ \left[ x=-1 , y=3 \right]  , \left[ x=1 , y=1 \right]  , 
 \left[ x=0 , y=2 \right]  \right] $$Fungsi f() bisa mengakses variabel global. Namun, seringkali kita
ingin menggunakan parameter lokal.


  a^x-x^a = 0.1  

with a=3.


\>function f(x,a) := x^a-a^x;


Salah satu cara untuk menyertakan parameter tambahan ke f() adalah
dengan menggunakan daftar yang berisi nama fungsi dan parameter (cara
lainnya adalah dengan menggunakan parameter titik koma).


\>solve({{"f",3}},2,y=0.1)


    2.54116291558

Ini juga berlaku untuk ekspresi. Namun, dalam hal ini, elemen daftar
yang bernama harus digunakan. (Lebih lanjut tentang daftar bisa
ditemukan di tutorial tentang sintaks EMT).


\>solve({{"x^a-a^x",a=3}},2,y=0.1)


    2.54116291558

# Menyelsaikan Pertidaksamaan

Untuk menyelesaikan pertidaksamaan, EMT tidak akan dapat melakukannya,


melainkan dengan bantuan Maxima, artinya secara eksak (simbolik).


Perintah Maxima yang digunakan adalah fourier_elim(), yang harus


dipanggil dengan perintah "load(fourier_elim)" terlebih dahulu.


\>&load(fourier\_elim)


    
            C:/Program Files/Euler x64/maxima/share/maxima/5.35.1/share/f\
    ourier_elim/fourier_elim.lisp
    

\>$&fourier\_elim([x^2 - 1\>0],[x]) // x^2-1 \> 0


$$\left[ 1<x \right] \lor \left[ x<-1 \right] $$\>$&fourier\_elim([x^2 - 1<0],[x]) // x^2-1 < 0


$$\left[ -1<x , x<1 \right] $$\>$&fourier\_elim([x^2 - 1 # 0],[x]) // x^-1 <\> 0


$$\left[ -1<x , x<1 \right] \lor \left[ 1<x \right] \lor \left[ x<-1
  \right] $$\>$&fourier\_elim([x # 6],[x])


$$\left[ x<6 \right] \lor \left[ 6<x \right] $$\>$&fourier\_elim([x < 1, x \> 1],[x]) // tidak memiliki penyelesaian


$${\it emptyset}$$\>$&fourier\_elim([minf < x, x < inf],[x]) // solusinya R


$${\it universalset}$$\>$&fourier\_elim([x^3 - 1 \> 0],[x])


$$\left[ 1<x , x^2+x+1>0 \right] \lor \left[ x<1 , -x^2-x-1>0
  \right] $$\>$&fourier\_elim([cos(x) < 1/2],[x]) // ??? gagal


$$\left[ 1-2\,\cos x>0 \right] $$\>$&fourier\_elim([y-x < 5, x - y < 7, 10 < y],[x,y]) // sistem pertidaksamaan


$$\left[ y-5<x , x<y+7 , 10<y \right] $$\>$&fourier\_elim([y-x < 5, x - y < 7, 10 < y],[y,x])


$$\left[ {\it max}\left(10 , x-7\right)<y , y<x+5 , 5<x \right] $$\>$&fourier\_elim((x + y < 5) and (x - y \>8),[x,y])


$$\left[ y+8<x , x<5-y , y<-\frac{3}{2} \right] $$\>$&fourier\_elim(((x + y < 5) and x < 1) or  (x - y \>8),[x,y])


$$\left[ y+8<x \right] \lor \left[ x<{\it min}\left(1 , 5-y\right)
  \right] $$\>&fourier\_elim([max(x,y) \> 6, x # 8, abs(y-1) \> 12],[x,y])


    
            [6 &lt; x, x &lt; 8, y &lt; - 11] or [8 &lt; x, y &lt; - 11]
     or [x &lt; 8, 13 &lt; y] or [x = y, 13 &lt; y] or [8 &lt; x, x &lt; y, 13 &lt; y]
     or [y &lt; x, 13 &lt; y]
    

\>$&fourier\_elim([(x+6)/(x-9) <= 6],[x])


$$\left[ x=12 \right] \lor \left[ 12<x \right] \lor \left[ x<9
  \right] $$# Bahasa Matriks

Dokumentasi inti EMT berisi pembahasan mendetail tentang bahasa
matriks Euler.


Vektor dan matriks dimasukkan dengan tanda kurung siku, elemen
dipisahkan oleh koma, dan baris dipisahkan oleh titik koma.


\>A=[2,3;4,5]


                2             3 
                4             5 

Produk matriks dinyatakan dengan titik.


\>b=[3;4]


                3 
                4 

\>b' // transpose b


    [3,  4]

\>inv(A) //inverse A


             -2.5           1.5 
                2            -1 

\>A.b //perkalian matriks


               18 
               32 

\>A.inv(A)


                1             0 
                0             1 

Poin utama dari bahasa matriks adalah bahwa semua fungsi dan operator
bekerja pada setiap elemen secara terpisah.


\>A.A


               16            21 
               28            37 

\>A^2 //perpangkatan elemen2 A


                4             9 
               16            25 

\>A.A.A


              116           153 
              204           269 

\>power(A,3) //perpangkatan matriks


              116           153 
              204           269 

\>A/A //pembagian elemen-elemen matriks yang seletak


                1             1 
                1             1 

\>A/b //pembagian elemen2 A oleh elemen2 b kolom demi kolom (karena b vektor kolom)


         0.666667             1 
                1          1.25 

\>A\\b // hasilkali invers A dan b, A^(-1)b 


             -1.5 
                2 

\>inv(A).b


             -1.5 
                2 

\>A\\A   //A^(-1)A


                1             0 
                0             1 

\>inv(A).A


                1             0 
                0             1 

\>A\*A //perkalin elemen-elemen matriks seletak


                4             9 
               16            25 

Ini bukan produk matriks, tetapi perkalian elemen per elemen. Hal yang
sama berlaku untuk vektor.


\>b^2 // perpangkatan elemen-elemen matriks/vektor


                9 
               16 

Jika salah satu operand adalah vektor atau skalar, itu akan diperluas
dengan cara yang alami.


\>2\*A


                4             6 
                8            10 

Misalnya, jika operandnya adalah vektor kolom, elemennya diterapkan ke
semua baris A.


\>[1,2]\*A


                2             6 
                4            10 

Jika operandnya adalah vektor baris, elemennya diterapkan ke semua
kolom A.


\>A\*[2,3]


                4             9 
                8            15 

Kita bisa membayangkan perkalian ini seolah-olah vektor baris v telah
digandakan untuk membentuk matriks dengan ukuran yang sama dengan A.


\>dup([1,2],2) // dup: menduplikasi/menggandakan vektor [1,2] sebanyak 2 kali


                1             2 
                1             2 

\>A\*dup([1,2],2)


                2             6 
                4            10 

Ini juga berlaku untuk dua vektor di mana satu adalah vektor baris dan
yang lainnya adalah vektor kolom. Kita menghitung i*j untuk i dan j
dari 1 hingga 5. Triknya adalah mengalikan 1:5 dengan transposenya.
Bahasa matriks Euler secara otomatis menghasilkan tabel nilai.


\>(1:5)\*(1:5)' // hasilkali elemen-elemen vektor baris dan vektor kolom


                1             2             3             4             5 
                2             4             6             8            10 
                3             6             9            12            15 
                4             8            12            16            20 
                5            10            15            20            25 

Sekali lagi, ingatlah bahwa ini bukan produk matriks!


\>(1:6).(1:6)' // hasilkali vektor baris dan vektor kolom


    91

\>sum((1:5)\*(1:5)) // sama hasilnya


    55

Bahkan operator seperti &lt; atau == bekerja dengan cara yang sama.


\>(1:10)<6 // menguji elemen-elemen yang kurang dari 6


    [1,  1,  1,  1,  1,  0,  0,  0,  0,  0]

Misalnya, kita bisa menghitung jumlah elemen yang memenuhi kondisi
tertentu dengan fungsi sum().


\>sum((1:10)<6) // banyak elemen yang kurang dari 6


    5

Euler memiliki operator perbandingan, seperti "==", yang memeriksa
kesetaraan.


Kita mendapatkan vektor yang berisi 0 dan 1, di mana 1 menunjukkan
benar.


\>t=(1:10)^2; t==25 //menguji elemen2 t yang sama dengan 25 (hanya ada 1)


    [0,  0,  0,  0,  1,  0,  0,  0,  0,  0]

Dari vektor seperti itu, "nonzeros" memilih elemen-elemen yang tidak
nol.


Dalam hal ini, kita mendapatkan indeks dari semua elemen yang lebih
besar dari 50.


\>nonzeros(t\>50) //indeks elemen2 t yang lebih besar daripada 50


    [8,  9,  10]

Tentu saja, kita bisa menggunakan vektor indeks ini untuk mendapatkan
nilai yang sesuai dalam t.


\>t[nonzeros(t\>50)] //elemen2 t yang lebih besar daripada 50


    [64,  81,  100]

Sebagai contoh, mari kita temukan semua kuadrat dari angka 1 hingga
1000 yang merupakan 5 modulo 11 dan 3 modulo 13.


\>t=1:1000; nonzeros(mod(t^2,11)==5 && mod(t^2,13)==3)


    [4,  48,  95,  139,  147,  191,  238,  282,  290,  334,  381,  425,
    433,  477,  524,  568,  576,  620,  667,  711,  719,  763,  810,  854,
    862,  906,  953,  997]

EMT tidak sepenuhnya efektif untuk perhitungan bilangan bulat. Secara
internal, ia menggunakan floating point presisi ganda. Namun, sering
kali sangat berguna.


Kita bisa memeriksa keprimaan.


Mari kita cari tahu berapa banyak kuadrat ditambah 1 yang merupakan
bilangan prima.


\>t=1:1000; length(nonzeros(isprime(t^2+1)))


    112

Fungsi nonzeros() hanya bekerja untuk vektor. Untuk matriks, ada
mnonzeros().


\>seed(2); A=random(3,4)


         0.765761      0.401188      0.406347      0.267829 
          0.13673      0.390567      0.495975      0.952814 
         0.548138      0.006085      0.444255      0.539246 

Fungsi ini mengembalikan indeks elemen-elemen yang tidak nol.


\>function f(x) ...


    
    endfunction
</pre>
Indeks-indeks ini dapat digunakan untuk mengatur elemen-elemen ke
nilai tertentu.


\>mset(A,k,0) //mengganti elemen2 suatu matriks pada indeks tertentu


    Variable or function k not found.
    Error in:
    mset(A,k,0) //mengganti elemen2 suatu matriks pada indeks tert ...
            ^

Fungsi mset() juga bisa mengatur elemen-elemen pada indeks-indeks
tersebut dengan entri dari matriks lain.


\>mset(A,k,-random(size(A)))


    Variable or function k not found.
    Error in:
    mset(A,k,-random(size(A))) ...
            ^

\>mget(A,k)


    Variable or function k not found.
    Error in:
    mget(A,k) ...
            ^

Dan memungkinkan untuk mendapatkan elemen-elemen tersebut dalam sebuah
vektor.


Fungsi berguna lainnya adalah extrema, yang mengembalikan nilai
minimal dan maksimal di setiap baris matriks beserta posisinya.


\>ex=extrema(A)


         0.267829             4      0.765761             1 
          0.13673             1      0.952814             4 
         0.006085             2      0.548138             1 

\>ex[,3]'


    [0.765761,  0.952814,  0.548138]

Ini, tentu saja, sama dengan fungsi max().


\>max(A)'


    [0.765761,  0.952814,  0.548138]

Namun, dengan mget(), kita bisa mengekstrak indeks-indeks tersebut dan
menggunakan informasi ini untuk mengambil elemen dari posisi yang sama
dari matriks lain.


\>j=(1:rows(A))'|ex[,4], mget(-A,j)


                1             1 
                2             4 
                3             1 
    [-0.765761,  -0.952814,  -0.548138]

# Fungsi Matriks Lainnya (Membangun Matriks)

Untuk membangun matriks, kita bisa menumpuk satu matriks di atas yang
lainnya. Jika keduanya tidak memiliki jumlah kolom yang sama, matriks
yang lebih pendek akan diisi dengan 0.


\> 

\>v=1:3; v\_v ...  
\>     


Demikian pula, kita bisa menempelkan matriks di samping matriks lain,
jika keduanya memiliki jumlah baris yang sama.


\>A=random(3,4); A|v'


    Commands must be separated by semicolon or comma!
    Found: v=1:3; v_v v=1:3; v_v v=1:3; v_v v=1:3; v_v v=1:3; v_v v=1:3; v_v v=1:3; v_v v=1:3; v_v v=1:3; v_v v=1:3; v_v A=random(3,4); A|v' (character 118)
    You can disable this in the Options menu.
    Error in:
    v=1:3; v_v v=1:3; v_v v=1:3; v_v v=1:3; v_v v=1:3; v_v v=1:3;  ...
               ^

Jika mereka tidak memiliki jumlah baris yang sama, matriks yang lebih
pendek akan diisi dengan 0.


Ada pengecualian untuk aturan ini. Sebuah angka riil yang ditempelkan
pada matriks akan digunakan sebagai kolom yang diisi dengan angka riil
tersebut.


\>A|1


         0.765761      0.401188      0.406347      0.267829             1 
          0.13673      0.390567      0.495975      0.952814             1 
         0.548138      0.006085      0.444255      0.539246             1 

Dimungkinkan untuk membuat matriks dari vektor baris dan vektor kolom.


\>[v;v]


                1             2             3 
                1             2             3 

\>[v',v']


                1             1 
                2             2 
                3             3 

Tujuan utamanya adalah untuk menginterpretasikan vektor ekspresi
sebagai vektor kolom.


\>"[x,x^2]"(v')


                1             1 
                2             4 
                3             9 

Untuk mendapatkan ukuran matriks A, kita bisa menggunakan
fungsi-fungsi berikut.


\>C=zeros(2,4); rows(C), cols(C), size(C), length(C)


    2
    4
    [2,  4]
    4

Untuk vektor, ada fungsi length().


\>length(2:10)


    9

Ada banyak fungsi lain yang menghasilkan matriks.


\>ones(2,2)


                1             1 
                1             1 

Ini juga bisa digunakan dengan satu parameter. Untuk mendapatkan
vektor dengan angka selain 1, gunakan yang berikut.


\>random(2,2)


         0.896177      0.251157 
         0.153047      0.126917 

Berikut adalah fungsi berguna lainnya yang mengubah struktur
elemen-elemen matriks menjadi matriks lain.


\>redim(1:9,3,3) // menyusun elemen2 1, 2, 3, ..., 9 ke bentuk matriks 3x3


                1             2             3 
                4             5             6 
                7             8             9 

Dengan fungsi berikut, kita bisa menggunakan fungsi ini dan fungsi dup
untuk menulis fungsi rep(), yang mengulang vektor sebanyak kali.


\>function rep(v,n) := redim(dup(v,n),1,n\*cols(v))

\>rep(1:3,5)


    [1,  2,  3,  1,  2,  3,  1,  2,  3,  1,  2,  3,  1,  2,  3]

Fungsi multdup() menggandakan elemen-elemen dari sebuah vektor.


\>multdup(1:3,5), multdup(1:3,[2,3,2])


    [1,  1,  1,  1,  1,  2,  2,  2,  2,  2,  3,  3,  3,  3,  3]
    [1,  1,  2,  2,  2,  3,  3]

Fungsi flipx() dan flipy() membalik urutan baris atau kolom dari
sebuah matriks. Misalnya, fungsi flipx() membalik secara horizontal.


\>flipx(1:5) //membalik elemen2 vektor baris


    [5,  4,  3,  2,  1]

Untuk rotasi, Euler memiliki fungsi rotleft() dan rotright().


\>rotleft(1:5) // memutar elemen2 vektor baris


    [2,  3,  4,  5,  1]

Fungsi khusus adalah drop(v, i), yang menghapus elemen-elemen dengan
indeks dalam i dari vektor v.


\>drop(10:20,3)


    [10,  11,  13,  14,  15,  16,  17,  18,  19,  20]

Perhatikan bahwa vektor dalam drop(v, i) merujuk pada indeks elemen di
i bukan nilai elemen tersebut. Jika Anda ingin menghapus elemen, Anda
perlu menemukan elemen-elemen tersebut terlebih dahulu. Fungsi
indexof(v, x) dapat digunakan untuk menemukan elemen x dalam vektor
terurut v.


\>v=primes(50), i=indexof(v,10:20), drop(v,i)


    [2,  3,  5,  7,  11,  13,  17,  19,  23,  29,  31,  37,  41,  43,  47]
    [0,  5,  0,  6,  0,  0,  0,  7,  0,  8,  0]
    [2,  3,  5,  7,  23,  29,  31,  37,  41,  43,  47]

Seperti yang Anda lihat, tidak ada masalah jika menyertakan indeks
yang berada di luar jangkauan (seperti 0), indeks ganda, atau indeks
yang tidak terurut.


\>drop(1:10,shuffle([0,0,5,5,7,12,12]))


    [1,  2,  3,  4,  6,  8,  9,  10]

Ada beberapa fungsi khusus untuk mengatur diagonal atau untuk
menghasilkan matriks diagonal.


Kita mulai dengan matriks identitas.


\>A=id(5) // matriks identitas 5x5


                1             0             0             0             0 
                0             1             0             0             0 
                0             0             1             0             0 
                0             0             0             1             0 
                0             0             0             0             1 

Kemudian, kita atur diagonal bawah (-1) menjadi 1:4.


\>setdiag(A,-1,1:4) //mengganti diagonal di bawah diagonal utama


                1             0             0             0             0 
                1             1             0             0             0 
                0             2             1             0             0 
                0             0             3             1             0 
                0             0             0             4             1 

Perhatikan bahwa kita tidak mengubah matriks A. Kita mendapatkan
matriks baru sebagai hasil dari setdiag().


Berikut adalah fungsi yang mengembalikan matriks tri-diagonal.


\>A=redim(1:9,3,3)


                1             2             3 
                4             5             6 
                7             8             9 

Sekarang kita bisa mengekstrak diagonalnya.


\>d=getdiag(A,0)


    [1,  5,  9]

Misalnya, kita bisa membagi matriks dengan diagonalnya. Bahasa matriks
memastikan bahwa vektor kolom d diterapkan ke matriks baris demi
baris.


\>fraction A/d'


            1         2         3 
          4/5         1       6/5 
          7/9       8/9         1 

# Faktoriasi

Hampir semua fungsi di Euler juga bekerja untuk input matriks dan
vektor, selama ini masuk akal.


Misalnya, fungsi sqrt() menghitung akar kuadrat dari semua elemen
vektor atau matriks.


\>sqrt(1:3)


    [1,  1.41421,  1.73205]

Jadi, Anda bisa dengan mudah membuat tabel nilai. Ini adalah salah
satu cara untuk memplot sebuah fungsi (alternatifnya menggunakan
ekspresi).


\>t=-1:0.1:1; s=t^3-t


    [0,  0.171,  0.288,  0.357,  0.384,  0.375,  0.336,  0.273,  0.192,
    0.099,  0,  -0.099,  -0.192,  -0.273,  -0.336,  -0.375,  -0.384,
    -0.357,  -0.288,  -0.171,  0]

EMT memperluas operator untuk skalar, vektor, dan matriks dengan cara
yang jelas.


Misalnya, vektor kolom dikalikan dengan vektor baris akan diperluas
menjadi matriks, jika operator diterapkan. Dalam hal ini, 


v adalah vektor yang ditranspos (vektor kolom).


\>shortest (1:5)\*(1:5)'


         1      2      3      4      5 
         2      4      6      8     10 
         3      6      9     12     15 
         4      8     12     16     20 
         5     10     15     20     25 

Perhatikan bahwa ini berbeda dari produk matriks. Produk matriks
dilambangkan dengan titik "." dalam EMT.


\>(1:5).(1:5)'


    55

Secara default, vektor baris dicetak dalam format kompak.


\>[1,2,3,4]


    [1,  2,  3,  4]

Untuk matriks, operator khusus . menunjukkan perkalian matriks, dan A'
menunjukkan transpos. Matriks 1x1 dapat digunakan seperti angka riil.


\>v:=[1,2]; v.v', %^2


    5
    25

Untuk mentranspos matriks, kita menggunakan apostrof (').


\>v=1:4; v'


                1 
                2 
                3 
                4 

Jadi, kita bisa menghitung matriks A dikalikan dengan vektor b.


\>A=[1,2,3,4;5,6,7,8]; A.v'


               30 
               70 

Perhatikan bahwa v masih merupakan vektor baris. Jadi, v'.v berbeda
dengan v.v' .


\>v'.v


                1             2             3             4 
                2             4             6             8 
                3             6             9            12 
                4             8            12            16 

v.v' menghitung norma kuadrat dari vektor baris v. Hasilnya adalah
matriks 1x1, yang berfungsi seperti angka riil.


\>v.v'


    30

Ada juga fungsi norm (bersama dengan banyak fungsi lain dalam Aljabar
Linier).


\>norm(v)^2


    30

Operator dan fungsi mematuhi bahasa matriks Euler. Berikut ringkasan
aturan yang berlaku:


* 
Fungsi yang diterapkan pada vektor atau matriks akan diterapkan pada
* setiap elemen secara individual.


* 
Operator yang beroperasi pada dua matriks dengan ukuran yang sama
* akan diterapkan secara berpasangan pada elemen-elemen matriks
* tersebut.


* 
Jika kedua matriks memiliki dimensi yang berbeda, keduanya akan
* diperluas secara logis sehingga ukurannya sama.


Contohnya, nilai skalar yang dikalikan dengan vektor akan mengalikan
nilai tersebut dengan setiap elemen vektor. Demikian juga, matriks
yang dikalikan dengan vektor (menggunakan *, bukan .) akan memperluas
vektor ke ukuran matriks dengan menggandakannya.


Berikut adalah contoh sederhana dengan operator ^.


\>[1,2,3]^2


    [1,  4,  9]

Berikut ini adalah contoh yang lebih rumit. Vektor baris yang
dikalikan dengan vektor kolom akan memperluas keduanya dengan
menggandakannya. Ini berarti elemen-elemen dari vektor baris dan kolom
akan dipasangkan secara otomatis untuk melakukan operasi penggandaan
antara elemen-elemen tersebut.


\>v:=[1,2,3]; v\*v'


                1             2             3 
                2             4             6 
                3             6             9 

Perlu dicatat bahwa produk skalar menggunakan produk matriks, bukan
operator *. Dalam operasi produk skalar, vektor baris dikalikan dengan
vektor kolom melalui aturan perkalian matriks, di mana hasilnya adalah
sebuah skalar (atau elemen tunggal) yang merupakan penjumlahan dari
hasil perkalian elemen-elemen yang sesuai.


\>v.v'


    14

Ada banyak fungsi untuk matriks. Berikut adalah daftar singkat.
Konsultasikan dokumentasi untuk informasi lebih lanjut mengenai
perintah-perintah ini:


    sum,prod computes the sum and products of the rows  
    cumsum,cumprod does the same cumulatively  
    computes the extremal values of each row  
    extrema returns a vector with the extremal information  
    diag(A,i) returns the i-th diagonal  
    setdiag(A,i,v) sets the i-th diagonal  
    id(n) the identity matrix  
    det(A) the determinant  
    charpoly(A) the characteristic polynomial  
    eigenvalues(A) the eigenvalues  

\>v\*v, sum(v\*v), cumsum(v\*v)


    [1,  4,  9]
    14
    [1,  5,  14]

Operator : menghasilkan vektor baris dengan jarak yang sama, dengan
opsi penentuan langkah (step size).


\>1:4, 1:2:10


    [1,  2,  3,  4]
    [1,  3,  5,  7,  9]

Untuk menggabungkan matriks dan vektor, tersedia operator "|" untuk
penggabungan horizontal dan "_" untuk penggabungan vertikal.


\>[1,2,3]|[4,5], [1,2,3]\_1


    [1,  2,  3,  4,  5]
                1             2             3 
                1             1             1 

Elemen-elemen dari sebuah matriks disebut dengan "A[i,j]".


\>A:=[1,2,3;4,5,6;7,8,9]; A[2,3]


    6

Untuk vektor baris atau kolom, v[i] adalah elemen ke-i dari vektor
tersebut. Untuk matriks, ini mengembalikan baris ke-i dari matriks.


\>v:=[2,4,6,8]; v[3], A[3]


    6
    [7,  8,  9]

Indeks juga dapat berupa vektor baris dari indeks. Tanda : menunjukkan
semua indeks.


\>v[1:2], A[:,2]


    [2,  4]
                2 
                5 
                8 

\>A[,2:3]


                2             3 
                5             6 
                8             9 

\>A{4}


    4

\>redim(A,1,prod(size(A))), flatten(A)


    [1,  2,  3,  4,  5,  6,  7,  8,  9]
    [1,  2,  3,  4,  5,  6,  7,  8,  9]

\>M = deg(w)|w|cos(w)|sin(w)


    Wrong argument.
    Cannot use a string matrix here.
    
    Try "trace errors" to inspect local variables after errors.
    deg:
        return x/pi*180;
    Error in:
    M = deg(w)|w|cos(w)|sin(w) ...
              ^

Menggunakan bahasa matriks, kita bisa menghasilkan beberapa tabel dari
beberapa fungsi sekaligus.


Dalam contoh berikut, kita menghitung [j] untuk i dari 1 hingga n.
Kita mendapatkan sebuah matriks, di mana setiap baris adalah tabel
dari


t^i untuk satu. Artinya, matriks tersebut memiliki elemen-elemen


Fungsi yang tidak dapat digunakan untuk input vektor perlu
"divectorisasi". Ini dapat dicapai dengan kata kunci "map" dalam
definisi fungsi. Dengan cara ini, fungsi tersebut akan dievaluasi
untuk setiap elemen dari parameter vektor.


Integrasi numerik integrate() hanya bekerja untuk batas interval
skalar. Jadi, kita perlu menderivasikannya.


\>function map f(x) := integrate("x^x",1,x)


Kata kunci "map" membuat fungsi menjadi vektorisasi. Fungsi tersebut
sekarang akan berfungsi untuk vektor angka.


\>f([1:5])


    [0,  2.05045,  13.7251,  113.336,  1241.03]

# Sub Matriks dan Elemen Matriks

Untuk mengakses elemen matriks, gunakan notasi kurung siku.


\>A=[1,2,3;4,5,6;7,8,9], A[2,2]


                1             2             3 
                4             5             6 
                7             8             9 
    5

\>A[2]


    [4,  5,  6]

\>v=1:3; v[2]


    2

Kita bahkan bisa mengurutkan ulang A menggunakan vektor indeks. Untuk
lebih jelasnya, kita tidak mengubah A di sini, tetapi menghitung versi


A yang sudah diurutkan ulang.


\>A[1:3,2:3]


                2             3 
                5             6 
                8             9 

\>A[:,3]


                3 
                6 
                9 

Sebagai alternatif, biarkan indeks pertama kosong.


\>A[,2:3]


                2             3 
                5             6 
                8             9 

Kita juga bisa mendapatkan baris terakhir dari A.


\>A[1,1]=4


                4             2             3 
                4             5             6 
                7             8             9 

\>A[1]=[-1,-1,-1]


               -1            -1            -1 
                4             5             6 
                7             8             9 

\>A[1:2,1:2]=0


                0             0            -1 
                0             0             6 
                7             8             9 

Peringatan: Indeks yang melebihi batas akan mengembalikan matriks
kosong atau pesan kesalahan, tergantung pada pengaturan sistem. Secara
default, akan muncul pesan kesalahan. Namun, indeks negatif dapat
digunakan untuk mengakses elemen matriks dari akhir.


\>A[4]


    Row index 4 out of bounds!
    Error in:
    A[4] ...
        ^

# Pengurutan dan Pengacakan

Fungsi sort() mengurutkan vektor baris.


Seringkali kita perlu mengetahui indeks dari vektor yang sudah
diurutkan dalam vektor aslinya. Ini bisa digunakan untuk mengurutkan
vektor lain dengan cara yang sama.


Mari kita acak urutan vektor.


\>v=shuffle(1:10)


    [2,  5,  10,  9,  3,  4,  8,  1,  6,  7]

\>{vs,ind}=sort(v); v[ind]


    [1,  2,  3,  4,  5,  6,  7,  8,  9,  10]

Ini juga berlaku untuk vektor yang berisi string.


\>s=["a","d","e","a","aa","e"]


    a
    d
    e
    a
    aa
    e

\>{ss,ind}=sort(s); ss


    a
    a
    aa
    d
    e
    e

\>ind


    [4,  1,  5,  2,  6,  3]

\>intrandom(1,10,10), unique(%


    [9,  1,  7,  7,  8,  7,  9,  10,  6,  2]
    Closing bracket missing in function call!
    Error in:
    intrandom(1,10,10), unique(% ...
                                ^

\>unique(s)


    a
    aa
    d
    e

# Aljabar Linear

EMT memiliki banyak fungsi untuk menyelesaikan sistem linier, sistem
jarang (sparse), atau masalah regresi.


Untuk sistem linier Ax=b, Anda dapat menggunakan algoritma Gauss,
invers matriks, atau pendekatan regresi linier. Operator A/b
menggunakan versi dari algoritma Gauss.


\>A=[1,2;3,4]; b=[5;6]; A\\b


               -4 
              4.5 

Untuk contoh lain, kita menghasilkan matriks berukuran 200x200 dan
jumlah dari baris-barisnya. Kemudian kita menyelesaikan Ax=b
menggunakan invers matriks. Kita mengukur kesalahan sebagai deviasi
maksimum dari semua elemen dari 1, yang tentu saja adalah solusi yang
benar.


\>A=normal(200,200); b=sum(A); longest totalmax(abs(inv(A).b-1))


      2.848832281188152e-13 

Jika sistem tidak memiliki solusi, penyesuaian linier meminimalkan
norma kesalahan Ax=b.


\>A=[1,2,3;4,5,6;7,8,9]


                1             2             3 
                4             5             6 
                7             8             9 

\>det(A)


    0

# Matriks Simbolik

Maxima memiliki matriks simbolik. Tentu saja, Maxima bisa digunakan
untuk masalah aljabar linier sederhana seperti ini. Kita bisa
mendefinisikan matriks untuk Euler dan Maxima dengan &amp;:=, dan kemudian
menggunakannya dalam ekspresi simbolik. Bentuk [...] yang biasa
digunakan untuk mendefinisikan matriks juga bisa digunakan di Euler
untuk mendefinisikan matriks simbolik.


\>A &= [a,1,1;1,a,1;1,1,a]; $A


$$\begin{pmatrix}a & 1 & 1 \\ 1 & a & 1 \\ 1 & 1 & a \\ \end{pmatrix}$$\>$&det(A), $&factor(%)


$$a\,\left(a^2-1\right)-2\,a+2$$$$\left(a-1\right)^2\,\left(a+2\right)$$\>$&invert(A) with a=0


$$\begin{pmatrix}-\frac{1}{2} & \frac{1}{2} & \frac{1}{2} \\ \frac{1
 }{2} & -\frac{1}{2} & \frac{1}{2} \\ \frac{1}{2} & \frac{1}{2} & -
 \frac{1}{2} \\ \end{pmatrix}$$\>A &= [1,a;b,2]; $A


$$\begin{pmatrix}1 & a \\ b & 2 \\ \end{pmatrix}$$\>$&eigenvectors([a,1;1,a]), &%[2][1][1]


$$\left[ \left[ \left[ a-1 , a+1 \right]  , \left[ 1 , 1 \right] 
  \right]  , \left[ \left[ \left[ 1 , -1 \right]  \right]  , \left[ 
 \left[ 1 , 1 \right]  \right]  \right]  \right] $$    
                                   [1, - 1]
    

Matriks simbolik dapat dievaluasi dalam Euler secara numerik seperti
halnya ekspresi simbolik lainnya.


\>A(a=4,b=5)


                1             4 
                5             2 

\>$&A with [a=4,b=5]


$$\begin{pmatrix}1 & 4 \\ 5 & 2 \\ \end{pmatrix}$$\>&A[1,1]:=t+1; $&A


$$\begin{pmatrix}t+1 & a \\ b & 2 \\ \end{pmatrix}$$Ada fungsi simbolik di Maxima untuk membuat vektor dan matriks.


Untuk ini, lihat dokumentasi Maxima atau tutorial tentang Maxima di
EMT.


\>B &:= [1,2;3,4]; $B, $&invert(B)


$$\begin{pmatrix}1 & 2 \\ 3 & 4 \\ \end{pmatrix}$$$$\begin{pmatrix}-2 & 1 \\ \frac{3}{2} & -\frac{1}{2} \\ 
 \end{pmatrix}$$\>$&invert(B)()


               -2             1 
              1.5          -0.5 

Perhatikan, bahwa dengan &amp;:= matriks B telah didefinisikan sebagai
simbolik dalam ekspresi simbolik dan sebagai numerik dalam ekspresi
numerik. Jadi kita dapat menggunakannya di sini.


\>longest B.xinv(B)


                          1                       0 
                          0                       1 

\>A=[1,2,3;4,5,6;7,8,9]; real(eigenvalues(A))


    [16.1168,  -1.11684,  0]

\>$&eigenvalues(@A)


$$\left[ \left[ \frac{15-3\,\sqrt{33}}{2} , \frac{3\,\sqrt{33}+15}{2}
  , 0 \right]  , \left[ 1 , 1 , 1 \right]  \right] $$# Nilai Numerik dalam Ekspresi simbolik

Ekspresi simbolis hanyalah sebuah string yang berisi ekspresi. jika
kita ingin menentukan nilai untuk ekspresi simbolik dan numerik
ekspresi, kita harus menggunakan "&amp;:=".


\>A &:= [1,pi;4,5]


                1       3.14159 
                4             5 

Masih terdapat perbedaan antara numerik dan simbolik membentuk. Saat
menerjemahkan matriks ke bentuk simbolik, pecahan perkiraan real akan
digunakan.


\>mxmset(A); $&A


$$\begin{pmatrix}1 & 3.141592653589793 \\ 4 & 5 \\ \end{pmatrix}$$\>$&bfloat(sqrt(2)), $&float(sqrt(2))


$$1.4142135623730950488016887242097_B \times 10^{0}$$$$1.414213562373095$$\>&fpprec:=100; &bfloat(pi)


    
            3.14159265358979323846264338327950288419716939937510582097494\
    4592307816406286208998628034825342117068b0
    

Variabel numerik dapat digunakan dalam ekspresi simbolik apa pun yang
menggunakan "@var". Perhatikan bahwa ini hanya diperlukan, jika
variabel telah didefinisikan dengan ":=" atau "=" sebagai variabel
numerik.


\>B:=[1,pi;3,4]; $&det(@B)


$$-5.424777960769379$$# Demo - Suku Bunga

Di bawah ini, kami menggunakan Euler Math Toolbox (EMT) untuk
menghitung suku bunga. Kami melakukannya secara numerik dan simbolis
untuk menunjukkan kepada Anda bagaimana Euler dapat digunakan
memecahkan masalah kehidupan nyata. Asumsikan Anda memiliki modal awal
sebesar 5.000 (katakanlah dalam dolar).


\>K=5000


    5000

\>K\*1.03


    5150

\>+K\*3%


    150

\>q=1+3%, K\*q


    1.03
    5150

\>K\*q^10


    6719.58189672

\>format(12,2); K\*q^10


        6719.58 

\>K\*q^(0:10)


    Real 1 x 11 matrix
    
        5000.00     5150.00     5304.50     5463.64     ...

\>short 0:10


    [0,  1,  2,  3,  4,  5,  6,  7,  8,  9,  10]

\>VK=K\*q^(0:10);

\>function oneyear (K) := round(K\*q,2)


\> ...  
\>   longest oneyear(1234.57), longest 1234.57\*q


                    1271.61 
                  1271.6071 

\>VKr=iterate("oneyear",5000,10)


    Real 1 x 11 matrix
    
        5000.00     5150.00     5304.50     5463.64     ...

\>VKr'


        5000.00 
        5150.00 
        5304.50 
        5463.64 
        5627.55 
        5796.38 
        5970.27 
        6149.38 
        6333.86 
        6523.88 
        6719.60 

\>VKr[2], VKr[1:3]


        5150.00 
        5000.00     5150.00     5304.50 

\>VKr[-1], VK[-1]


        6719.60 
        6719.58 

# Menyelesaikan Persamaan

Sekarang kita mengambil fungsi yang lebih maju, yang masing-masing
menambahkan tingkat uang tertentu tahun.


\>function onepay (K) := K\*q+R


\> ...  
\>   function onepay (K) := K\*q+R

\>R=200; iterate("onepay",5000,10)


    Real 1 x 11 matrix
    
        5000.00     5350.00     5710.50     6081.82     ...

\>R=-200; iterate("onepay",5000,10)


    Real 1 x 11 matrix
    
        5000.00     4950.00     4898.50     4845.45     ...

\>VKR=iterate("onepay",5000,50)


    Real 1 x 51 matrix
    
        5000.00     4950.00     4898.50     4845.45     ...

\>min(nonzeros(VKR<0))


          48.00 

Alasannya adalah bukan nol (VKR&lt;0) mengembalikan vektor indeks i, di
mana VKR[i]&lt;0, dan min menghitung indeks minimal.


Karena vektor selalu dimulai dengan indeks 1, maka jawabannya adalah
47 tahun.


Fungsi iterate() mempunyai satu trik lagi. Ini dapat mengambil kondisi
akhir sebagai sebuah argumen. Kemudian akan mengembalikan nilai dan
jumlah iterasi.


\>{x,n}=iterate("onepay",5000,till="x<0"); x, n,


         -19.83 
          47.00 

Mari kita coba menjawab pertanyaan yang lebih ambigu. Asumsikan kita
mengetahui nilainya adalah 0 setelah 50 tahun. Berapa tingkat
bunganya?


Ini adalah pertanyaan yang hanya bisa dijawab secara numerik. Di bawah
ini, kami akan melakukannya mendapatkan rumus yang diperlukan. Maka
Anda akan melihat bahwa tidak ada yang mudah rumus untuk tingkat
bunga. Namun untuk saat ini, kami menargetkan solusi numerik.


Langkah pertama adalah mendefinisikan fungsi yang melakukan iterasi
sebanyak n kali. Kami tambahkan semua parameter ke fungsi ini.


\>function f(K,R,P,n) := iterate("x\*(1+P/100)+R",K,n;P,R)[-1]


Iterasinya sama seperti di atas


x_{n+1} = x_n \cdot \left(1+ \frac{P}{100}\right) + R


Namun kami tidak lagi menggunakan nilai global R dalam ekspresi kami.
Fungsi seperti iterate() memiliki trik khusus di Euler. Anda dapat
meneruskan nilai variabel dalam ekspresi sebagai parameter titik koma.
Dalam hal ini P dan R.


Selain itu, kami hanya tertarik pada nilai terakhir. Jadi kita ambil
indeksnya [-1].


Mari kita coba tes.


\>f(5000,-200,3,47)


         -19.83 

\>solve("f(5000,-200,x,50)",3)


           3.15 

per tahun. Kami mengambil nilai awal 3% untuk algoritma. Pemecahannya()


Kita bisa menggunakan fungsi yang sama untuk menyelesaikan pertanyaan berikut: Berapa banyak yang bisa kita
hapus per tahun sehingga modal awal habis setelah asumsi 20 tahun
tingkat bunga 3% per tahun.


\>solve("f(5000,x,3,20)",-200)


        -336.08 

# Solusi Simbolis Masalah Suku Bunga

Kita dapat menggunakan bagian simbolik Euler untuk mempelajari
masalahnya. Pertama kita definisikan fungsi kami onepay() secara
simbolis.


\>function op(K) &= K\*q+R; $&op(K)


$$R+q\,K$$\>$&op(op(op(op(K)))), $&expand(%)


$$q\,\left(q\,\left(q\,\left(R+q\,K\right)+R\right)+R\right)+R$$$$q^3\,R+q^2\,R+q\,R+R+q^4\,K$$\>&sum(q^k,k,0,n-1); $& % = ev(%,simpsum)


$$\sum_{k=0}^{n-1}{q^{k}}=\frac{q^{n}-1}{q-1}$$\>function fs(K,R,P,n) &= (1+P/100)^n\*K + ((1+P/100)^n-1)/(P/100)\*R; $&fs(K,R,P,n)


$$\frac{100\,\left(\left(\frac{P}{100}+1\right)^{n}-1\right)\,R}{P}+K
 \,\left(\frac{P}{100}+1\right)^{n}$$\>longest f(5000,-200,3,47), longest fs(5000,-200,3,47)


         -19.82504734650985 
         -19.82504734652684 

\>solve("fs(5000,-330,3,x)",30)


          20.51 

\>$&limit(R(5000,0,x,10),x,0)


$$\lim_{x\rightarrow 0}{R\left(5000 , 0 , x , 10\right)}$$\>fn &= solve(equ,n) | ratsimp; $&fn


$$\left[  \right] $$# Plot2D

# Menggambar Grafik 2D dengan EMT

Notebook ini menjelaskan tentang cara menggambar berbagaikurva dan
grafik 2D dengan software EMT. EMT menyediakan fungsi plot2d() untuk
menggambar berbagai kurva dan grafik dua dimensi (2D).


## Plots Dasar

Ada beberapa fungsi dasar dalam membuat grafik. Ada koordinat layar,
yang selalu berkisar antara 0 hingga 1024 di setiap sumbu, tidak
peduli apakah layar tersebut berbentuk kotak atau tidak. Ada juga
koordinat grafik, yang bisa diatur dengan fungsi setplot(). Cara
pemetaan antara koordinat layar dan koordinat grafik bergantung pada
jendela grafik yang sedang aktif. Misalnya, fungsi shrinkwindow()
secara default menyisakan ruang untuk label sumbu dan judul grafik.


Dalam contoh ini, kita hanya menggambar beberapa garis acak dengan
berbagai warna. Untuk detail lebih lanjut tentang fungsi-fungsi ini,
pelajari fungsi-fungsi inti dari EMT.


\>clg; // clear screen

\>window(0,0,1024,1024); // use all of the window

\>setplot(0,1,0,1); // set plot coordinates

\>hold on; // start overwrite mode

\>n=100; X=random(n,2); Y=random(n,2);  // get random points

\>colors=rgb(random(n),random(n),random(n)); // get random colors

\>loop 1 to n; color(colors[#]); plot(X[#],Y[#]); end; // plot


\>hold off; // end overwrite mode

\>reset;


Penting untuk menahan grafik, karena perintah plot() akan menghapus
jendela grafik yang ada.


Untuk menghapus semua yang telah kita buat, kita menggunakan perintah
reset().


Untuk menampilkan gambar hasil plot di layar notebook, perintah
plot2d() dapat diakhiri dengan titik dua (:). Cara lain adalah
perintah plot2d() diakhiri dengan titik koma (;), kemudian menggunakan
perintah insimg() untuk menampilkan gambar hasil plot.


Untuk contoh lainnya, kita menggambar sebuah grafik kecil di dalam
grafik yang lebih besar. Ini dilakukan dengan mendefinisikan jendela
grafik yang lebih kecil. Perhatikan bahwa jendela ini tidak
menyediakan ruang untuk label sumbu di luar jendela grafik. Kita perlu
menambahkan margin jika diperlukan. Juga, perhatikan bahwa kita
menyimpan dan mengembalikan jendela penuh, serta mempertahankan grafik
yang sedang ada saat kita menggambar grafik kecil tersebut.


\>plot2d("x^3-x");

\>xw=200; yw=100; ww=300; hw=300;

\>ow=window();

\>window(xw,yw,xw+ww,yw+hw);

\>hold on;

\>barclear(xw-50,yw-10,ww+60,ww+60);

\>plot2d("x^4-x",grid=6):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-097.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-097.png)

\>hold off;

\>window(ow);


Untuk membuat plot dengan beberapa gambar, kita bisa menggunakan
fungsi figure().


## Aspek Plot

Secara default, plot menggunakan jendela plot berbentuk kotak. Kamu
bisa mengubah ini menggunakan fungsi aspect(). Jangan lupa untuk
mengatur ulang aspek setelahnya. Kamu juga bisa mengubah pengaturan
default ini melalui menu dengan memilih "Set Aspect" untuk rasio aspek
tertentu atau sesuai ukuran jendela grafis saat ini.


Namun, kamu juga bisa mengubahnya hanya untuk satu plot. Caranya
adalah dengan mengubah ukuran area plot saat ini dan menyesuaikan
jendela agar label-labelnya memiliki ruang yang cukup.


\>aspect(2); // rasio panjang dan lebar 2:1

\>plot2d(["sin(x)","cos(x)"],0,2pi):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-098.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-098.png)

\>aspect();

\>reset;


Fungsi reset() mengembalikan pengaturan plot ke default, termasuk
rasio aspek.


Plot 2D di Euler


EMT Math Toolbox memiliki plot 2D, baik untuk data maupun fungsi. EMT
menggunakan fungsi plot2d untuk membuat plot dari fungsi dan data.


Kamu juga bisa membuat plot di Maxima menggunakan Gnuplot atau di
Python menggunakan Matplotlib.


Euler dapat membuat plot 2D dari:


* 
ekspresi


* 
fungsi, variabel, atau kurva yang diparameterisasi,


* 
vektor nilai x-y,


* 
kumpulan titik di bidang,


* 
kurva implisit dengan level atau wilayah level,


* 
fungsi kompleks.


Gaya plot termasuk berbagai gaya untuk garis dan titik, plot batang,
dan plot berbayangan.


Plot Ekspresi atau Variabel


Satu ekspresi dalam "x" (misalnya "4*x^2") atau nama fungsi (misalnya
"f") akan menghasilkan grafik dari fungsi tersebut.


Berikut adalah contoh paling dasar, yang menggunakan rentang default
dan mengatur rentang y yang sesuai untuk menyesuaikan plot fungsi
tersebut.


Catatan: Jika kamu mengakhiri baris perintah dengan tanda titik dua
":", plot akan dimasukkan ke jendela teks. Jika tidak, tekan TAB untuk
melihat plot jika jendela plot tertutup.


\>plot2d("x^2"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-099.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-099.png)

\>aspect(1.5); plot2d("x^3-x"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-100.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-100.png)

\>a:=5.6; plot2d("exp(-a\*x^2)/a"); insimg(30); // menampilkan gambar hasil plot setinggi 25 baris


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-101.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-101.png)

Dari beberapa contoh sebelumnya Anda dapat melihat bahwa aslinya
gambar plot menggunakan sumbu X dengan rentang nilai dari -2 sampai
dengan 2. Untuk mengubah rentang nilai X dan Y, Anda dapat menambahkan
nilai-nilai batas X (dan Y) di belakang ekspresi yang digambar.


Rentang plot diatur dengan parameter-parameter berikut:


* 
a, b  : rentang x (default: -2, 2)

* 
c, d  : rentang y (default: disesuaikan dengan nilai)

* 
r     :sebagai alternatif, radius di sekitar pusat plot

* 
cx, cy: koordinat pusat plot (default: 0, 0)


\>plot2d("x^3-x",-1,2):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-102.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-102.png)

\>plot2d("sin(x)",-2\*pi,2\*pi): // plot sin(x) pada interval [-2pi, 2pi]


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-103.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-103.png)

\>plot2d("cos(x)","sin(3\*x)",xmin=0,xmax=2pi):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-104.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-104.png)

Sebagai alternatif untuk titik dua ":", kamu bisa menggunakan perintah
insimg(lines), yang menyisipkan plot dan menggunakan sejumlah baris
teks yang ditentukan.


Dalam opsi, plot dapat diatur untuk muncul:


- di jendela terpisah yang bisa diubah ukurannya,


- di jendela notebook.


Gaya plot tambahan dapat dicapai dengan menggunakan perintah plot
khusus.


Jika plot tersembunyi, tekan tombol tabulator untuk melihatnya.


Untuk membagi jendela menjadi beberapa plot, gunakan perintah
figure(). Dalam contoh ini, kita memplot x^1 hingga x^4 ke dalam 4
bagian jendela. Perintah figure(0) mengatur ulang jendela ke
pengaturan default.


\>reset; 

\>figure(2,2); ...  
\>   for n=1 to 4; figure(n); plot2d("x^"+n); end; ...  
\>   figure(0):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-105.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-105.png)

Dalam plot2d(), tersedia gaya alternatif dengan menggunakan grid=x.
Untuk memberikan gambaran, kami menunjukkan berbagai gaya grid dalam
satu gambar (lihat perintah figure() di bawah). Gaya grid=0 tidak
termasuk. Gaya ini tidak menampilkan grid dan tidak ada bingkai.


\>figure(3,3); ...  
\>   for k=1:9; figure(k); plot2d("x^3-x",-2,1,grid=k); end; ...  
\>   figure(0):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-106.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-106.png)

Jika argumen pada plot2d() adalah ekspresi yang diikuti oleh empat
angka, angka-angka ini adalah rentang x dan y untuk plot tersebut.


Alternatifnya, a, b, c, d dapat ditentukan sebagai parameter yang
ditetapkan sebagai a=... dll.


Pada contoh berikut, kita mengubah gaya kisi, menambahkan label, dan
menggunakan label vertikal untuk sumbu y.


\>aspect(1.5); plot2d("sin(x)",0,2pi,-1.2,1.2,grid=3,xl="x",yl="sin(x)"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-107.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-107.png)

\>plot2d("sin(x)+cos(2\*x)",0,4pi):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-108.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-108.png)

Gambar-gambar yang dihasilkan dengan menyisipkan plot ke dalam jendela
teks disimpan di direktori yang sama dengan notebook, secara default
dalam subdirektori bernama "images". Gambar-gambar ini juga digunakan
saat mengekspor ke HTML.


Kamu bisa dengan mudah menandai gambar apa pun dan menyalinnya ke
clipboard dengan menekan Ctrl-C. Tentu saja, kamu juga bisa mengekspor
grafik saat ini dengan fungsi-fungsi di menu File.


Fungsi atau ekspresi dalam plot2d dievaluasi secara adaptif. Untuk
kecepatan lebih, matikan plot adaptif dengan &lt;adaptive dan tentukan
jumlah subinterval dengan n=.... Ini hanya perlu dilakukan dalam
kasus-kasus yang jarang.


\>plot2d("sign(x)\*exp(-x^2)",-1,1,<adaptive,n=10000):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-109.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-109.png)

\>plot2d("x^x",r=1.2,cx=1,cy=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-110.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-110.png)

Perhatikan bahwa x^x tidak ditentukan untuk x&lt;=0. Fungsi plot2d
menangkap kesalahan ini, dan mulai membuat plot segera setelah
fungsinya ditentukan. Ini berfungsi untuk semua fungsi yang
mengembalikan NAN di luar jangkauan definisinya.


\>plot2d("log(x)",-0.1,2):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-111.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-111.png)

Parameter square=true (atau &gt;square) memilih rentang y secara otomatis
sehingga hasilnya adalah jendela plot persegi. Perhatikan bahwa secara
default, Euler menggunakan spasi persegi di dalam jendela plot.


\>plot2d("x^3-x",\>square):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-112.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-112.png)

\>plot2d(''integrate("sin(x)\*exp(-x^2)",0,x)'',0,2): // plot integral


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-113.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-113.png)

Jika Anda memerlukan lebih banyak ruang untuk label y, panggil
shrinkwindow() dengan parameter lebih kecil, atau tetapkan nilai
positif untuk "lebih kecil" di plot2d().


\>plot2d("gamma(x)",1,10,yl="y-values",smaller=6,<vertical):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-114.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-114.png)

Ekspresi simbolik juga dapat digunakan karena disimpan sebagai
ekspresi string sederhana.


\>x=linspace(0,2pi,1000); plot2d(sin(5x),cos(7x)):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-115.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-115.png)

\>a:=5.6; expr &= exp(-a\*x^2)/a; // define expression

\>plot2d(expr,-2,2): // plot from -2 to 2


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-116.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-116.png)

\>plot2d(expr,r=1,thickness=2): // plot in a square around (0,0)


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-117.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-117.png)

\>plot2d(&diff(expr,x),\>add,style="--",color=red): // add another plot


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-118.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-118.png)

\>plot2d(&diff(expr,x,2),a=-2,b=2,c=-2,d=1): // plot in rectangle


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-119.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-119.png)

\>plot2d(&diff(expr,x),a=-2,b=2,\>square): // keep plot square


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-120.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-120.png)

\>plot2d("x^2",0,1,steps=1,color=red,n=10):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-121.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-121.png)

\>plot2d("x^2",\>add,steps=2,color=blue,n=10):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-122.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-122.png)

# Fungsi dalam satu Parameter

Fungsi plot yang paling penting untuk plot planar adalah plot2d().
Fungsi ini diimplementasikan dalam bahasa Euler di file "plot.e", yang
dimuat di awal program.


Berikut beberapa contoh penggunaan suatu fungsi. Seperti biasa di EMT,
fungsi yang berfungsi untuk fungsi atau ekspresi lain, Anda bisa
meneruskan parameter tambahan (selain x) yang bukan variabel global ke
fungsi dengan parameter titik koma atau dengan kumpulan panggilan.


\>function f(x,a) := x^2/a+a\*x^2-x; // define a function

\>a=0.3; plot2d("f",0,1;a): // plot with a=0.3


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-123.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-123.png)

\>plot2d("f",0,1;0.4): // plot with a=0.4


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-124.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-124.png)

\>plot2d({{"f",0.2}},0,1): // plot with a=0.2


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-125.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-125.png)

\>plot2d({{"f(x,b)",b=0.1}},0,1): // plot with 0.1


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-126.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-126.png)

\>function f(x) := x^3-x; ...  
\>   plot2d("f",r=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-127.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-127.png)

Berikut ini ringkasan fungsi yang diterima


* 
ekspresi atau ekspresi simbolik di x

* 
fungsi atau fungsi simbolik dengan nama "f"

* 
fungsi simbolik hanya dengan nama f


Fungsi plot2d() juga menerima fungsi simbolik. Untuk fungsi simbolik,
namanya saja yang berfungsi.


\>function f(x) &= diff(x^x,x)


    
                                x
                               x  (log(x) + 1)
    

\>plot2d(f,0,2):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-128.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-128.png)

Tentu saja, untuk ekspresi atau ekspresi simbolik, nama variabel sudah
cukup untuk memplotnya.


\>expr &= sin(x)\*exp(-x)


    
                                  - x
                                 E    sin(x)
    

\>plot2d(expr,0,3pi):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-129.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-129.png)

\>function f(x) &= x^x;

\>plot2d(f,r=1,cx=1,cy=1,color=blue,thickness=2);

\>plot2d(&diff(f(x),x),\>add,color=red,style="-.-"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-130.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-130.png)

Untuk gaya garis ada berbagai pilihan.


* 
gaya="...". Pilih dari "-", "--", "-.", ".", ".-.", "-.-".

* 
Warna: Lihat di bawah untuk warna.

* 
ketebalan: Defaultnya adalah 1.


Warna dapat dipilih sebagai salah satu warna default, atau sebagai
warna RGB.


* 
0..15: indeks warna default.

* 
konstanta warna: putih, hitam, merah, hijau, biru, cyan, zaitun,
* abu-abu muda, abu-abu, abu-abu tua, oranye, hijau muda, pirus, biru
* muda, oranye muda, kuning

* 
rgb(merah,hijau,biru): parameternya real di [0,1].


\>plot2d("exp(-x^2)",r=2,color=red,thickness=3,style="--"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-131.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-131.png)

Berikut adalah tampilan warna EMT yang telah ditentukan sebelumnya.


\>aspect(2); columnsplot(ones(1,16),lab=0:15,grid=0,color=0:15)

\>insimg (15)


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-132.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-132.png)

Tapi Anda bisa menggunakan warna apa saja.


\>columnsplot(ones(1,16),grid=0,color=rgb(0,0,linspace(0,1,15))):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-133.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-133.png)

# Menggambar Beberapa Kurva pada bidang koordinat yang sama

Plot lebih dari satu fungsi (multiple function) ke dalam satu jendela
dapat dilakukan dengan berbagai cara. Salah satu metodenya adalah
menggunakan &gt;add untuk beberapa panggilan ke plot2d secara
keseluruhan, kecuali panggilan pertama. Kami telah menggunakan fitur
ini pada contoh di atas.


\>aspect(); plot2d("cos(x)",r=2,grid=6); plot2d("x",style=".",\>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-134.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-134.png)

\>aspect(1.5); plot2d("sin(x)",0,2pi); plot2d("cos(x)",color=blue,style="--",\>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-135.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-135.png)

Salah satu kegunaan &gt;add adalah untuk menambahkan titik pada kurva.


\>plot2d("sin(x)",0,pi); plot2d(2,sin(2),\>points,\>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-136.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-136.png)

Kita tambahkan titik perpotongan dengan label (pada posisi "cl" untuk
kiri tengah), dan masukkan hasilnya ke dalam buku catatan. Kami juga
menambahkan judul pada plot.


\>plot2d(["cos(x)","x"],r=1.1,cx=0.5,cy=0.5, ...  
\>    color=[black,blue],style=["-","."], ...  
\>    grid=1);


    Illegal parameter after named parameter!
    Error in:
    ... .5,  color=[black,blue],style=["-","."],  grid=1); ...
                                                         ^

\>x0=solve("cos(x)-x",1);  ...  
\>    plot2d(x0,x0,\>points,\>add,title="Intersection Demo");  ...  
\>     label("cos(x) = x",x0,x0,pos="cl",offset=20):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-137.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-137.png)

Dalam demo berikut, kita memplot fungsi sin(x)=sin(x)/x dan ekspansi
Taylor ke-8 dan ke-16. Kami menghitung perluasan ini menggunakan
Maxima melalui ekspresi simbolik.


Plot ini dilakukan dalam perintah multi-baris berikut dengan tiga
panggilan ke plot2d(). Yang kedua dan ketiga memiliki kumpulan tanda
&gt;add, yang membuat plot menggunakan rentang sebelumnya.


Kami menambahkan kotak label yang menjelaskan fungsinya.


\>$taylor(sin(x)/x,x,0,4)


$$\frac{x^4}{120}-\frac{x^2}{6}+1$$\>plot2d("sinc(x)",0,4pi,color=green,thickness=2); ...  
\>     plot2d(&taylor(sin(x)/x,x,0,8),\>add,color=blue,style="--"); ...  
\>     plot2d(&taylor(sin(x)/x,x,0,16),\>add,color=red,style="-.-"); ...  
\>     labelbox(["sinc","T8","T16"],styles=["-","--","-.-"], ...  
\>       colors=[black,blue,red]):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-139.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-139.png)

Dalam contoh berikut, kami menghasilkan Polinomial Bernstein.


lateks: B_i(x) = \binom{n}{i} x^i (1-x)^{n-i}


\>plot2d("(1-x)^10",0,1); // plot first function

\>for i=1 to 10; plot2d("bin(10,i)\*x^i\*(1-x)^(10-i)",\>add); end;

\>insimg;


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-140.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-140.png)

Cara kedua adalah dengan menggunakan pasangan matriks bernilai x dan
matriks bernilai y yang berukuran sama.


Kami menghasilkan matriks nilai dengan satu Polinomial Bernstein di
setiap baris. Untuk ini, kita cukup menggunakan vektor kolom i. Lihat
pendahuluan tentang bahasa matriks untuk mempelajari lebih detail.


\>x=linspace(0,1,500);

\>n=10; k=(0:n)'; // n is row vector, k is column vector

\>y=bin(n,k)\*x^k\*(1-x)^(n-k); // y is a matrix then

\>plot2d(x,y):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-141.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-141.png)

Perhatikan bahwa parameter warna dapat berupa vektor. Kemudian setiap
warna digunakan untuk setiap baris matriks.


\>x=linspace(0,1,200); y=x^(1:10)'; plot2d(x,y,color=1:10):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-142.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-142.png)

Metode lain adalah menggunakan vektor ekspresi (string). Anda kemudian
dapat menggunakan susunan warna, susunan gaya, dan susunan ketebalan
dengan panjang yang sama.


\>plot2d(["sin(x)","cos(x)"],0,2pi,color=4:5): 


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-143.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-143.png)

\>plot2d(["sin(x)","cos(x)"],0,2pi): // plot vector of expressions


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-144.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-144.png)

Kita bisa mendapatkan vektor seperti itu dari Maxima menggunakan
makelist() dan mxm2str().


\>v &= makelist(binomial(10,i)\*x^i\*(1-x)^(10-i),i,0,10) // make list


    
                    10            9              8  2             7  3
            [(1 - x)  , 10 (1 - x)  x, 45 (1 - x)  x , 120 (1 - x)  x , 
               6  4             5  5             4  6             3  7
    210 (1 - x)  x , 252 (1 - x)  x , 210 (1 - x)  x , 120 (1 - x)  x , 
              2  8              9   10
    45 (1 - x)  x , 10 (1 - x) x , x  ]
    

\>mxm2str(v) // get a vector of strings from the symbolic vector


    (1-x)^10
    10*(1-x)^9*x
    45*(1-x)^8*x^2
    120*(1-x)^7*x^3
    210*(1-x)^6*x^4
    252*(1-x)^5*x^5
    210*(1-x)^4*x^6
    120*(1-x)^3*x^7
    45*(1-x)^2*x^8
    10*(1-x)*x^9
    x^10

\>plot2d(mxm2str(v),0,1): // plot functions


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-145.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-145.png)

Alternatif lain adalah dengan menggunakan bahasa matriks Euler.


Jika suatu ekspresi menghasilkan matriks fungsi, dengan satu fungsi di
setiap baris, semua fungsi tersebut akan diplot ke dalam satu plot.


Untuk ini, gunakan vektor parameter dalam bentuk vektor kolom. Jika
array warna ditambahkan maka akan digunakan untuk setiap baris plot.


\>n=(1:10)'; plot2d("x^n",0,1,color=1:10):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-146.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-146.png)

Ekspresi dan fungsi satu baris dapat melihat variabel global.


Jika Anda tidak dapat menggunakan variabel global, Anda perlu
menggunakan fungsi dengan parameter tambahan, dan meneruskan parameter
ini sebagai parameter titik koma.


Berhati-hatilah, untuk meletakkan semua parameter yang ditetapkan di
akhir perintah plot2d. Dalam contoh ini kita meneruskan a=5 ke fungsi
f, yang kita plot dari -10 hingga 10.


\>function f(x,a) := 1/a\*exp(-x^2/a); ...  
\>   plot2d("f",-10,10;5,thickness=2,title="a=5"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-147.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-147.png)

Alternatifnya, gunakan koleksi dengan nama fungsi dan semua parameter
tambahan. Daftar khusus ini disebut kumpulan panggilan, dan ini adalah
cara yang lebih disukai untuk meneruskan argumen ke suatu fungsi yang
kemudian diteruskan sebagai argumen ke fungsi lain.


Pada contoh berikut, kita menggunakan loop untuk memplot beberapa
fungsi (lihat tutorial tentang pemrograman loop).


\>plot2d({{"f",1}},-10,10); ...  
\>   for a=2:10; plot2d({{"f",a}},\>add); end:


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-148.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-148.png)

Kita dapat mencapai hasil yang sama dengan cara berikut menggunakan
bahasa matriks EMT. Setiap baris matriks f(x,a) merupakan satu fungsi.
Selain itu, kita dapat mengatur warna untuk setiap baris matriks. Klik
dua kali pada fungsi getspectral() untuk penjelasannya.


\>x=-10:0.01:10; a=(1:10)'; plot2d(x,f(x,a),color=getspectral(a/10)):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-149.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-149.png)

## Label Teks

Dekorasi sederhana pun bisa


* 
judul dengan judul = "..."

* 
label x dan y dengan xl="...", yl="..."

* 
label teks lain dengan label("...",x,y)


Perintah label akan memplot ke plot saat ini pada koordinat plot
(x,y). Hal ini memerlukan argumen posisional.


\>plot2d("x^3-x",-1,2,title="y=x^3-x",yl="y",xl="x"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-150.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-150.png)

\>expr := "log(x)/x"; ...  
\>     plot2d(expr,0.5,5,title="y="+expr,xl="x",yl="y"); ...  
\>     label("(1,0)",1,0); label("Max",E,expr(E),pos="lc"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-151.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-151.png)

Ada juga fungsi labelbox(), yang dapat menampilkan fungsi dan teks.
Dibutuhkan vektor string dan warna, satu item untuk setiap fungsi.


\>function f(x) &= x^2\*exp(-x^2);  ...  
\>   plot2d(&f(x),a=-3,b=3,c=-1,d=1);  ...  
\>   plot2d(&diff(f(x),x),\>add,color=blue,style="--"); ...  
\>   labelbox(["function","derivative"],styles=["-","--"], ...  
\>      colors=[black,blue],w=0.4):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-152.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-152.png)

Kotak ini berlabuh di kanan atas secara default, tetapi &gt;kiri berlabuh
di kiri atas. Anda dapat memindahkannya ke tempat mana pun yang Anda
suka. Posisi jangkar berada di pojok kanan atas kotak, dan angkanya
merupakan pecahan dari ukuran jendela grafis. Lebarnya otomatis.


Untuk plot titik, kotak label juga berfungsi. Tambahkan parameter
&gt;points, atau vektor bendera, satu untuk setiap label.


Pada contoh berikut, hanya ada satu fungsi. Jadi kita bisa menggunakan
string sebagai pengganti vektor string. Kami mengatur warna teks
menjadi hitam untuk contoh ini.


\>n=10; plot2d(0:n,bin(n,0:n),\>addpoints); ...  
\>   labelbox("Binomials",styles="[]",\>points,x=0.1,y=0.1, ...  
\>   tcolor=black,\>left):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-153.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-153.png)

Gaya plot ini juga tersedia di statplot(). Seperti di plot2d() warna
dapat diatur untuk setiap baris plot. Masih banyak lagi plot khusus
untuk keperluan statistik (lihat tutorial tentang statistik).


\>statplot(1:10,random(2,10),color=[red,blue]):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-154.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-154.png)

Fitur serupa adalah fungsi textbox().


Lebarnya secara default adalah lebar maksimal baris teks. Tapi itu
bisa diatur oleh pengguna juga.


\>function f(x) &= exp(-x)\*sin(2\*pi\*x); ...  
\>   plot2d("f(x)",0,2pi); ...  
\>   textbox(latex("\\text{Example of a damped oscillation}\\ f(x)=e^{-x}sin(2\\pi x)"),w=0.85):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-155.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-155.png)

Label teks, judul, kotak label, dan teks lainnya dapat berisi string
Unicode (lihat sintaks EMT untuk mengetahui lebih lanjut tentang
string Unicode).


\>plot2d("x^3-x",title=u"x &rarr; x&sup3; - x"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-156.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-156.png)

Label pada sumbu x dan y bisa vertikal, begitu juga dengan sumbunya.


\>plot2d("sinc(x)",0,2pi,xl="x",yl=u"x &rarr; sinc(x)",\>vertical):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-157.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-157.png)

## LaTeX

Anda juga dapat memplot rumus LaTeX jika Anda telah menginstal sistem
LaTeX. Saya merekomendasikan MiKTeX. Jalur ke biner "lateks" dan
"dvipng" harus berada di jalur sistem, atau Anda harus mengatur LaTeX
di menu opsi.


Perhatikan, penguraian LaTeX lambat. Jika Anda ingin menggunakan LaTeX
dalam plot animasi, Anda harus memanggil latex() sebelum loop satu
kali dan menggunakan hasilnya (gambar dalam matriks RGB).


Pada plot berikut, kami menggunakan LaTeX untuk label x dan y, label,
kotak label, dan judul plot.


\>plot2d("exp(-x)\*sin(x)/x",a=0,b=2pi,c=0,d=1,grid=6,color=blue, ...  
\>    title=latex("\\text{Function $\\Phi$}"), ...  
\>    xl=latex("\\phi"),yl=latex("\\Phi(\\phi)")); ...  
\>   textbox( ...  
\>     latex("\\Phi(\\phi) = e^{-\\phi} \\frac{\\sin(\\phi)}{\\phi}"),x=0.8,y=0.5); ...  
\>   label(latex("\\Phi",color=blue),1,0.4):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-158.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-158.png)

Seringkali, kita menginginkan spasi dan label teks yang tidak
konformal pada sumbu x. Kita bisa menggunakan xaxis() dan yaxis()
seperti yang akan kita tunjukkan nanti.


Cara termudah adalah membuat plot kosong dengan bingkai menggunakan
grid=4, lalu menambahkan grid dengan ygrid() dan xgrid(). Pada contoh
berikut, kami menggunakan tiga string LaTeX untuk label pada sumbu x
dengan xtick().


\>plot2d("sinc(x)",0,2pi,grid=4,<ticks); ...  
\>   ygrid(-2:0.5:2,grid=6); ...  
\>   xgrid([0:2]\*pi,<ticks,grid=6);  ...  
\>   xtick([0,pi,2pi],["0","\\pi","2\\pi"],\>latex):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-159.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-159.png)

Tentu saja fungsinya juga bisa digunakan.


\>function map f(x) ...


    if x>0 then return x^4
    else return x^2
    endif
    endfunction
</pre>
Parameter "peta" membantu menggunakan fungsi untuk vektor. Untuk


plot, itu tidak perlu. Tapi untuk menunjukkan vektorisasi itu


berguna, kita menambahkan beberapa poin penting ke plot di x=-1, x=0
dan x=1.


Pada plot berikut, kami juga memasukkan beberapa kode LaTeX. Kami
menggunakannya untuk


dua label dan kotak teks. Tentu saja, Anda hanya bisa menggunakannya


LaTeX jika Anda telah menginstal LaTeX dengan benar.


\>plot2d("f",-1,1,xl="x",yl="f(x)",grid=6);  ...  
\>   plot2d([-1,0,1],f([-1,0,1]),\>points,\>add); ...  
\>   label(latex("x^3"),0.72,f(0.72)); ...  
\>   label(latex("x^2"),-0.52,f(-0.52),pos="ll"); ...  
\>   textbox( ...  
\>     latex("f(x)=\\begin{cases} x^3 & x\>0 \\\\ x^2 & x \\le 0\\end{cases}"), ...  
\>     x=0.7,y=0.2):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-160.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-160.png)

## Interaksi Pengguna

Saat memplot suatu fungsi atau ekspresi, parameter &gt;pengguna
memungkinkan pengguna untuk memperbesar dan menggeser plot dengan
tombol kursor atau mouse. Pengguna bisa


* 
perbesar dengan + atau -

* 
pindahkan plot dengan tombol kursor

* 
pilih jendela plot dengan mouse

* 
atur ulang tampilan dengan spasi

* 
keluar dengan kembali


Tombol spasi akan mengatur ulang plot ke jendela plot aslinya.


Saat memplot data, flag &gt;user hanya akan menunggu penekanan tombol.


\>plot2d({{"x^3-a\*x",a=1}},\>user,title="Press any key!"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-161.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-161.png)

\>plot2d("exp(x)\*sin(x)",user=true, ...  
\>     title="+/- or cursor keys (return to exit)"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-162.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-162.png)

Berikut ini menunjukkan cara interaksi pengguna tingkat lanjut (lihat
tutorial tentang pemrograman untuk detailnya).


Fungsi bawaan mousedrag() menunggu aktivitas mouse atau keyboard. Ini
melaporkan mouse ke bawah, mouse digerakkan atau mouse ke atas, dan
penekanan tombol. Fungsi dragpoints() memanfaatkan ini, dan
memungkinkan pengguna menyeret titik mana pun dalam plot.


Kita membutuhkan fungsi plot terlebih dahulu. Misalnya, kita melakukan
interpolasi pada 5 titik dengan polinomial. Fungsi tersebut harus
diplot ke dalam area plot yang tetap.


\>function plotf(xp,yp,select) ...


    endfunction
</pre>
\>                 


     d=interp(xp,yp);
      plot2d("interpval(xp,d,x)";d,xp,r=2);
      plot2d(xp,yp,>points,>add);
      if select>0 then
        plot2d(xp[select],yp[select],color=red,>points,>add);
      endif;
      title("Drag one point, or press space or return!");
    endfunction
</pre>
Perhatikan parameter titik koma di plot2d (d dan xp), yang diteruskan
ke evaluasi fungsi interp(). Tanpa ini, kita harus menulis fungsi
plotinterp() terlebih dahulu, mengakses nilainya secara global.


Sekarang kita menghasilkan beberapa nilai acak, dan membiarkan
pengguna menyeret titiknya.


\>t=-1:0.5:1; dragpoints("plotf",t,random(size(t))-0.5):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-163.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-163.png)

Perhatikan parameter titik koma di plot2d (d dan xp), yang diteruskan
ke evaluasi fungsi interp(). Tanpa ini, kita harus menulis fungsi
plotinterp() terlebih dahulu, mengakses nilainya secara global.


Sekarang kita menghasilkan beberapa nilai acak, dan membiarkan
pengguna menyeret titiknya.


\>function plotf([a,b]) := plot2d("exp(a\*x)\*cos(2pi\*b\*x)",0,2pi;a,b);


Kemudian kita memerlukan nama untuk parameter, nilai awal dan matriks
rentang nx2, opsional garis judul.


Ada penggeser interaktif, yang dapat menetapkan nilai oleh pengguna.
Fungsi dragvalues() menyediakan ini.


\>dragvalues("plotf",["a","b"],[-1,2],[[-2,2];[1,10]], ...  
\>     heading="Drag these values:",hcolor=black):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-164.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-164.png)

Dimungkinkan untuk membatasi nilai yang diseret menjadi bilangan
bulat. Sebagai contoh, kita menulis fungsi plot, yang memplot
polinomial Taylor berderajat n ke fungsi kosinus.


\>function plotf(n) ...


    plot2d("cos(x)",0,2pi,>square,grid=6);
    plot2d(&"taylor(cos(x),x,0,@n)",color=blue,>add);
    textbox("Taylor polynomial of degree "+n,0.1,0.02,style="t",>left);
    endfunction
</pre>
Sekarang kita izinkan derajat n bervariasi dari 0 hingga 20 dalam 20
perhentian. Hasil dragvalues() digunakan untuk memplot sketsa dengan n
ini, dan untuk memasukkan plot ke dalam buku catatan.


\>nd=dragvalues("plotf","degree",2,[0,20],20,y=0.8, ...  
\>    heading="Drag the value:"); ...  
\>   plotf(nd):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-165.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-165.png)

Berikut ini adalah demonstrasi sederhana dari fungsinya. Pengguna
dapat menggambar jendela plot, meninggalkan jejak titik.


\>function dragtest ...


     plot2d(none,r=1,title="Drag with the mouse, or press any key!");
      start=0;
      repeat
        {flag,m,time}=mousedrag();
        if flag==0 then return; endif;
        if flag==2 then
          hold on; mark(m[1],m[2]); hold off;
        endif;
      end
    endfunction
</pre>
\>dragtest // lihat hasilnya dan cobalah lakukan!


## Gaya Plot 2D

Secara default, EMT menghitung tick sumbu otomatis dan menambahkan
label ke setiap tick. Ini dapat diubah dengan parameter grid. Gaya
default sumbu dan label dapat diubah. Selain itu, label dan judul
dapat ditambahkan secara manual. Untuk menyetel ulang ke gaya default,
gunakan reset().


\>aspect(); insimg;


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-166.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-166.png)

\>figure(3,4); ...  
\>   figure(1); plot2d("x^3-x",grid=0); ... // no grid, frame or axis

\> figure(2); plot2d("x^3-x",grid=1); ... // x-y-axis

\> figure(3); plot2d("x^3-x",grid=2); ... // default ticks

\> figure(4); plot2d("x^3-x",grid=3); ... // x-y- axis with labels insid

\> figure(5); plot2d("x^3-x",grid=4); ... // no ticks, only labels

\> figure(6); plot2d("x^3-x",grid=5); ... // default, but no margin

\> figure(7); plot2d("x^3-x",grid=6); ... // axes only

\> figure(8); plot2d("x^3-x",grid=7); ... // axes only, ticks

\> figure(9); plot2d("x^3-x",grid=8); ... // axes only, finer

\> figure(10); plot2d("x^3-x",grid=9); ... // default, small ticks

\> figure(11); plot2d("x^3-x",grid=10); ...// no ticks, axes only

\> figure(0):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-167.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-167.png)

Parameter &lt;frame mematikan frame, dan framecolor=blue mengatur frame
menjadi warna biru.


Jika Anda menginginkan tanda centang Anda sendiri, Anda dapat
menggunakan style=0, dan menambahkan semuanya nanti.


\>aspect(1.5);

\>plot2d("x^3-x",grid=0); // plot

\>frame; xgrid([-1,0,1]); ygrid(0): // add frame and grid


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-168.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-168.png)

Untuk judul plot dan label sumbu, lihat contoh berikut.


\>plot2d("exp(x)",-1,1);

\>textcolor(black); // set the text color to black

\>title(latex("y=e^x")); // title above the plot

\>xlabel(latex("x")); // "x" for x-axis

\>ylabel(latex("y"),\>vertical); // vertical "y" for y-axis

\>label(latex("(0,1)"),0,1,color=blue): // label a point


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-169.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-169.png)

Sumbu dapat digambar secara terpisah dengan xaxis() dan yaxis().


\>plot2d("x^3-x",<grid,<frame);

\>xaxis(0,xx=-2:1,style="-\>"); yaxis(0,yy=-5:5,style="-\>"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-170.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-170.png)

Teks pada plot dapat diatur dengan label(). Dalam contoh berikut, "lc"
berarti bagian tengah bawah. Ini menetapkan posisi label relatif
terhadap koordinat plot.


\>function f(x) &= x^3-x


    
                                     3
                                    x  - x
    

\>plot2d(f,-1,1,\>square);

\>x0=fmin(f,0,1); // compute point of minimum

\>label("Rel. Min.",x0,f(x0),pos="lc"): // add a label there


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-171.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-171.png)

Ada juga kotak teks.


\>plot2d(&f(x),-1,1,-2,2); // function

\>plot2d(&diff(f(x),x),\>add,style="--",color=red); // derivative

\>labelbox(["f","f'"],["-","--"],[black,red]): // label box


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-172.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-172.png)

\>plot2d(["exp(x)","1+x"],color=[black,blue],style=["-","-.-"]


    Closing bracket missing in function call!
    Error in:
    ... p(x)","1+x"],color=[black,blue],style=["-","-.-"] ...
                                                         ^

\>gridstyle("-\>",color=gray,textcolor=gray,framecolor=gray);...  
\>    plot2d("x^3-x",grid=1);   ...  
\>    settitle("y=x^3-x",color=black); ...  
\>    label("x",2,0,pos="bc",color=gray);  ...  
\>    label("y",0,6,pos="cl",color=gray); ...  
\>    reset():


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-173.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-173.png)

Untuk kontrol lebih lanjut, sumbu x dan sumbu y dapat dilakukan secara
manual.


Perintah fullwindow() memperluas jendela plot karena kita tidak lagi
memerlukan tempat untuk label di luar jendela plot. Gunakan
shrinkwindow() atau reset() untuk menyetel ulang ke default.


\>fullwindow; ...  
\>    gridstyle(color=darkgray,textcolor=darkgray); ...  
\>    plot2d(["2^x","1","2^(-x)"],a=-2,b=2,c=0,d=4,<grid,color=4:6,<frame); ...  
\>    xaxis(0,-2:1,style="-\>"); xaxis(0,2,"x",<axis); ...  
\>    yaxis(0,4,"y",style="-\>"); ...  
\>    yaxis(-2,1:4,\>left); ...  
\>    yaxis(2,2^(-2:2),style=".",<left); ...  
\>    labelbox(["2^x","1","2^-x"],colors=4:6,x=0.8,y=0.2); ...  
\>    reset:


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-174.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-174.png)

Berikut adalah contoh lain, di mana string Unicode digunakan dan
sumbunya berada di luar area plot.


\>aspect(1.5);

\>plot2d(["sin(x)","cos(x)"],0,2pi,color=[red,green],<grid,<frame); ...  
\>    xaxis(-1.1,(0:2)\*pi,xt=["0",u"&pi;",u"2&pi;"],style="-",\>ticks,\>zero);  ...  
\>    xgrid((0:0.5:2)\*pi,<ticks); ...  
\>    yaxis(-0.1\*pi,-1:0.2:1,style="-",\>zero,\>grid); ...  
\>    labelbox(["sin","cos"],colors=[red,green],x=0.5,y=0.2,\>left); ...  
\>    xlabel(u"&phi;"); ylabel(u"f(&phi;)"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-175.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-175.png)

# Merencanakan Data 2D

Jika x dan y adalah vektor data, maka data tersebut akan digunakan
sebagai koordinat x dan y pada suatu kurva. Dalam hal ini, a, b, c,
dan d, atau radius r dapat ditentukan, atau jendela plot akan
menyesuaikan secara otomatis dengan data. Alternatifnya, &gt;persegi
dapat diatur untuk mempertahankan rasio aspek persegi.


Merencanakan ekspresi hanyalah singkatan dari plot data. Untuk plot
data, Anda memerlukan satu atau beberapa baris nilai x, dan satu atau
beberapa baris nilai y. Dari rentang dan nilai x, fungsi plot2d akan
menghitung data yang akan diplot, secara default dengan evaluasi
fungsi yang adaptif. Untuk plot titik gunakan "&gt;titik", untuk garis
dan titik campuran gunakan "&gt;addpoints".


Tapi Anda bisa memasukkan data secara langsung.


* 
Gunakan vektor baris untuk x dan y untuk satu fungsi.

* 
Matriks untuk x dan y diplot baris demi baris.


Berikut adalah contoh dengan satu baris untuk x dan y.


\>x=-10:0.1:10; y=exp(-x^2)\*x; plot2d(x,y):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-176.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-176.png)

Data juga dapat diplot sebagai poin. Gunakan points=true untuk ini.
Plotnya berfungsi seperti poligon, tetapi hanya menggambar sudutnya
saja.


* 
style="...": Pilih dari "[]", "&lt;&gt;", "o", ".", "..", "+", "*", "[]#",
* "&lt; &gt;#", "o#", "..#", "#", "|".


Untuk memplot kumpulan titik, gunakan &gt;titik. Jika warna merupakan
vektor warna, masing-masing titik


mendapat warna berbeda. Untuk matriks koordinat dan vektor kolom,
warna diterapkan pada baris matriks.


Parameter &gt;addpoints menambahkan titik ke segmen garis untuk plot
data.


\>xdata=[1,1.5,2.5,3,4]; ydata=[3,3.1,2.8,2.9,2.7]; // data

\>plot2d(xdata,ydata,a=0.5,b=4.5,c=2.5,d=3.5,style="."); // lines

\>plot2d(xdata,ydata,\>points,\>add,style="o"): // add points


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-177.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-177.png)

\>p=polyfit(xdata,ydata,1); // get regression line

\>plot2d("polyval(p,x)",\>add,color=red): // add plot of line


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-178.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-178.png)

# Menggambar Daerah Yang Dibatasi Kurva

Plot data sebenarnya berbentuk poligon. Kita juga dapat memplot kurva
atau kurva terisi.


* 
terisi=benar mengisi plot.

* 
style="...": Pilih dari "#", "/", "\", "\/".

* 
Fillcolor : Lihat di atas untuk mengetahui warna yang tersedia.


Warna isian ditentukan oleh argumen "fillcolor", dan pada &lt;outline
opsional, mencegah menggambar batas untuk semua gaya kecuali gaya
default.


\>t=linspace(0,2pi,1000); // parameter for curve

\>x=sin(t)\*exp(t/pi); y=cos(t)\*exp(t/pi); // x(t) and y(t)

\>figure(1,2); aspect(16/9)

\>figure(1); plot2d(x,y,r=10); // plot curve

\>figure(2); plot2d(x,y,r=10,\>filled,style="/",fillcolor=red); // fill curve

\>figure(0):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-179.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-179.png)

Dalam contoh berikut kita memplot elips terisi dan dua segi enam
terisi menggunakan kurva tertutup dengan 6 titik dengan gaya isian
berbeda.


\>x=linspace(0,2pi,1000); plot2d(sin(x),cos(x)\*0.5,r=1,\>filled,style="/"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-180.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-180.png)

\>t=linspace(0,2pi,6); ...  
\>   plot2d(cos(t),sin(t),\>filled,style="/",fillcolor=red,r=1.2):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-181.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-181.png)

\>t=linspace(0,2pi,6); plot2d(cos(t),sin(t),\>filled,style="#"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-182.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-182.png)

Contoh lainnya adalah septagon yang kita buat dengan 7 titik pada
lingkaran satuan.


\>t=linspace(0,2pi,7);  ...  
\>   plot2d(cos(t),sin(t),r=1,\>filled,style="/",fillcolor=red):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-183.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-183.png)

Berikut adalah himpunan nilai maksimal dari empat kondisi linier yang
kurang dari atau sama dengan 3. Ini adalah A[k].v&lt;=3 untuk semua baris
A. Untuk mendapatkan sudut yang bagus, kita menggunakan n yang relatif
besar.


\>A=[2,1;1,2;-1,0;0,-1];

\>function f(x,y) := max([x,y].A');

\>plot2d("f",r=4,level=[0;3],color=green,n=111):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-184.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-184.png)

Poin utama dari bahasa matriks adalah memungkinkan pembuatan tabel
fungsi dengan mudah.


\>t=linspace(0,2pi,1000); x=cos(3\*t); y=sin(4\*t);


Kami sekarang memiliki nilai vektor x dan y. plot2d() dapat memplot
nilai-nilai ini


sebagai kurva yang menghubungkan titik-titik tersebut. Plotnya bisa
diisi. Dalam hal ini


ini menghasilkan hasil yang bagus karena aturan belitan, yang
digunakan untuk


isi.


\>plot2d(x,y,<grid,<frame,\>filled):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-185.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-185.png)

Vektor interval diplot terhadap nilai x sebagai wilayah terisi


antara nilai interval yang lebih rendah dan lebih tinggi.


Hal ini dapat berguna untuk memplot kesalahan perhitungan. Tapi itu
bisa


juga dapat digunakan untuk memplot kesalahan statistik.


\>t=0:0.1:1; ...  
\>    plot2d(t,interval(t-random(size(t)),t+random(size(t))),style="|");  ...  
\>    plot2d(t,t,add=true):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-186.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-186.png)

Jika x adalah vektor yang diurutkan, dan y adalah vektor interval,
maka plot2d akan memplot rentang interval yang terisi pada bidang.
Gaya isiannya sama dengan gaya poligon.


\>t=-1:0.01:1; x=~t-0.01,t+0.01~; y=x^3-x;

\>plot2d(t,y):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-187.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-187.png)

Dimungkinkan untuk mengisi wilayah nilai untuk fungsi tertentu. Untuk


ini, level harus berupa matriks 2xn. Baris pertama adalah batas bawah


dan baris kedua berisi batas atas.


\>expr := "2\*x^2+x\*y+3\*y^4+y"; // define an expression f(x,y)

\>plot2d(expr,level=[0;1],style="-",color=blue): // 0 <= f(x,y) <= 1


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-188.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-188.png)

Kita juga dapat mengisi rentang nilai seperti


\>plot2d("(x^2+y^2)^2-x^2+y^2",r=1.2,level=[-1;0],style="/"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-189.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-189.png)

\>plot2d("cos(x)","sin(x)^3",xmin=0,xmax=2pi,\>filled,style="/"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-190.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-190.png)

# Grafik Fungsi Parametrik

Nilai x tidak perlu diurutkan. (x,y) hanya menggambarkan sebuah kurva.
Jika x diurutkan, kurva tersebut merupakan grafik suatu fungsi.


Dalam contoh berikut, kita memplot spiral


Kita perlu menggunakan banyak titik untuk tampilan yang halus atau
fungsi adaptive() untuk mengevaluasi ekspresi (lihat fungsi adaptive()
untuk lebih jelasnya).


\>t=linspace(0,1,1000); ...  
\>   plot2d(t\*cos(2\*pi\*t),t\*sin(2\*pi\*t),r=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-191.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-191.png)

Sebagai alternatif, dimungkinkan untuk menggunakan dua ekspresi untuk
kurva. Berikut ini plot kurva yang sama seperti di atas.


\>plot2d("x\*cos(2\*pi\*x)","x\*sin(2\*pi\*x)",xmin=0,xmax=1,r=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-192.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-192.png)

\>t=linspace(0,1,1000); r=exp(-t); x=r\*cos(2pi\*t); y=r\*sin(2pi\*t);

\>plot2d(x,y,r=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-193.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-193.png)

Pada contoh berikutnya, kita memplot kurvanya


dengan


\>t=linspace(0,2pi,1000); r=1+sin(3\*t)/2; x=r\*cos(t); y=r\*sin(t); ...  
\>   plot2d(x,y,\>filled,fillcolor=red,style="/",r=1.5):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-194.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-194.png)

# Menggambar Grafik Bilangan Kompleks

Serangkaian bilangan kompleks juga dapat diplot. Kemudian titik-titik
grid akan dihubungkan. Jika sejumlah garis kisi ditentukan (atau
vektor garis kisi 1x2) dalam argumen cgrid, hanya garis kisi tersebut
yang terlihat.


Matriks bilangan kompleks secara otomatis akan diplot sebagai
kisi-kisi pada bidang kompleks.


Pada contoh berikut, kita memplot gambar lingkaran satuan di bawah
fungsi eksponensial. Parameter cgrid menyembunyikan beberapa kurva
grid.


\>aspect(); r=linspace(0,1,50); a=linspace(0,2pi,80)'; z=r\*exp(I\*a);...  
\>   aspect(); r=linspace(0,1,50); a=linspace(0,2pi,80)'; z=r\*exp(I\*a);...  
\>   plot2d(z,a=-1.25,b=1.25,c=-1.25,d=1.25,cgrid=10):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-195.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-195.png)

\>aspect(1.25); r=linspace(0,1,50); a=linspace(0,2pi,200)'; z=r\*exp(I\*a);

\>plot2d(exp(z),cgrid=[40,10]):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-196.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-196.png)

\>r=linspace(0,1,10); a=linspace(0,2pi,40)'; z=r\*exp(I\*a);

\>plot2d(exp(z),\>points,\>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-197.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-197.png)

Vektor bilangan kompleks secara otomatis diplot sebagai kurva pada
bidang kompleks dengan bagian nyata dan bagian imajiner.


Dalam contoh, kita memplot lingkaran satuan dengan


lateks: \gamma(t) = e^{it}


\>t=linspace(0,2pi,1000); ...  
\>   plot2d(exp(I\*t)+exp(4\*I\*t),r=2):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-198.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-198.png)

# Plot Statistik

Ada banyak fungsi yang dikhususkan pada plot statistik. Salah satu
plot yang sering digunakan adalah plot kolom.


Jumlah kumulatif dari nilai terdistribusi normal 0-1 menghasilkan
jalan acak.


\>plot2d(cumsum(randnormal(1,1000))):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-199.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-199.png)

Penggunaan dua baris menunjukkan jalan dalam dua dimensi.


\>X=cumsum(randnormal(2,1000)); plot2d(X[1],X[2]):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-200.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-200.png)

\>columnsplot(cumsum(random(10)),style="/",color=blue):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-201.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-201.png)

\>title("Temperature"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-202.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-202.png)

\>k=0:10;

\>plot2d(k,bin(10,k),\>bar):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-203.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-203.png)

\>plot2d(k,bin(10,k)); plot2d(k,bin(10,k),\>points,\>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-204.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-204.png)

\>plot2d(normal(1000),normal(1000),\>points,grid=6,style=".."):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-205.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-205.png)

\>plot2d(normal(1,1000),\>distribution,style="O"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-206.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-206.png)

\>plot2d("qnormal",0,5;2.5,0.5,\>filled):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-207.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-207.png)

Untuk memplot distribusi statistik eksperimental, Anda dapat
menggunakan distribution=n dengan plot2d.


\>w=randexponential(1,1000); // exponential distribution

\>plot2d(w,\>distribution): // or distribution=n with n intervals


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-208.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-208.png)

Atau Anda dapat menghitung distribusi dari data dan memplot hasilnya
dengan &gt;bar di plot3d, atau dengan plot kolom.


\>w=normal(1000); // 0-1-normal distribution

\>{x,y}=histo(w,10,v=[-6,-4,-2,-1,0,1,2,4,6]); // interval bounds v

\>plot2d(x,y,\>bar):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-209.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-209.png)

Fungsi statplot() mengatur gaya dengan string sederhana.


\>statplot(1:10,cumsum(random(10)),"b"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-210.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-210.png)

\>n=10; i=0:n; ...  
\>   plot2d(i,bin(n,i)/2^n,a=0,b=10,c=0,d=0.3); ...  
\>   plot2d(i,bin(n,i)/2^n,points=true,style="ow",add=true,color=blue):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-211.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-211.png)

Selain itu, data dapat diplot sebagai batang. Dalam hal ini, x harus
diurutkan dan satu elemen lebih panjang dari y. Batangnya akan
memanjang dari x[i] hingga x[i+1] dengan nilai y[i]. Jika x berukuran
sama dengan y, maka x akan diperpanjang satu elemen dengan spasi
terakhir.


Gaya isian dapat digunakan seperti di atas.


\>n=10; k=bin(n,0:n); ...  
\>   plot2d(-0.5:n+0.5,k,bar=true,fillcolor=lightgray):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-212.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-212.png)

Data untuk plot batang (batang=1) dan histogram (histogram=1) dapat
diberikan secara eksplisit dalam xv dan yv, atau dapat dihitung dari
distribusi empiris dalam xv dengan &gt;distribusi (atau distribusi=n).
Histogram nilai xv akan dihitung secara otomatis dengan &gt;histogram.
Jika &gt;even ditentukan, nilai xv akan dihitung dalam interval bilangan
bulat.


\>plot2d(normal(10000),distribution=50):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-213.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-213.png)

\>k=0:10; m=bin(10,k); x=(0:11)-0.5; plot2d(x,m,\>bar):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-214.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-214.png)

\>columnsplot(m,k):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-215.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-215.png)

\>plot2d(random(600)\*6,histogram=6):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-216.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-216.png)

Untuk distribusi, terdapat parameter distribution=n, yang menghitung
nilai secara otomatis dan mencetak distribusi relatif dengan n
sub-interval.


\>plot2d(normal(1,1000),distribution=10,style="\\/"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-217.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-217.png)

Dengan parameter even=true, ini akan menggunakan interval bilangan
bulat.


\>plot2d(intrandom(1,1000,10),distribution=10,even=true):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-218.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-218.png)

Perhatikan bahwa ada banyak plot statistik yang mungkin berguna.
Silahkan lihat tutorial tentang statistik.


\>columnsplot(getmultiplicities(1:6,intrandom(1,6000,6))):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-219.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-219.png)

\>plot2d(normal(1,1000),\>distribution); ...  
\>    plot2d("qnormal(x)",color=red,thickness=2,\>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-220.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-220.png)

Ada juga banyak plot khusus untuk statistik. Plot kotak menunjukkan
kuartil distribusi ini dan banyak outlier. Menurut definisinya,
outlier dalam plot kotak adalah data yang melebihi 1,5 kali rentang
50% tengah plot.


\>M=normal(5,1000); boxplot(quartiles(M)):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-221.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-221.png)

# Fungsi Implisit

Plot implisit menunjukkan penyelesaian garis level f(x,y)=level,
dengan "level" dapat berupa nilai tunggal atau vektor nilai. Jika
level = "auto", akan ada garis level nc, yang akan tersebar antara
fungsi minimum dan maksimum secara merata. Warna yang lebih gelap atau
lebih terang dapat ditambahkan dengan &gt;hue untuk menunjukkan nilai
fungsi. Untuk fungsi implisit, xv harus berupa fungsi atau ekspresi
parameter x dan y, atau alternatifnya, xv dapat berupa matriks nilai.


Euler dapat menandai garis level


dari fungsi apa pun.


Untuk menggambar himpunan f(x,y)=c untuk satu atau lebih konstanta c,
Anda dapat menggunakan plot2d() dengan plot implisitnya pada bidang.
Parameter c adalah level=c, dimana c dapat berupa vektor garis level.
Selain itu, skema warna dapat digambar di latar belakang untuk
menunjukkan nilai fungsi setiap titik dalam plot. Parameter "n"
menentukan kehalusan plot.


\>aspect(1.5);

\>plot2d("x^2+y^2-x\*y-x",r=1.5,level=0,contourcolor=red):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-222.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-222.png)

\>expr := "2\*x^2+x\*y+3\*y^4+y"; // define an expression f(x,y)

\>plot2d(expr,level=0): // Solutions of f(x,y)=0


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-223.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-223.png)

\>plot2d(expr,level=0:0.5:20,\>hue,contourcolor=white,n=200): // nice


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-224.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-224.png)

\>plot2d(expr,level=0:0.5:20,\>hue,\>spectral,n=200,grid=4): // nicer


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-225.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-225.png)

Ini juga berfungsi untuk plot data. Namun Anda harus menentukan
rentangnya


untuk label sumbu.


\>x=-2:0.05:1; y=x'; z=expr(x,y);

\>plot2d(z,level=0,a=-1,b=2,c=-2,d=1,\>hue):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-226.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-226.png)

\>plot2d("x^3-y^2",\>contour,\>hue,\>spectral):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-227.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-227.png)

\>plot2d("x^3-y^2",level=0,contourwidth=3,\>add,contourcolor=red):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-228.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-228.png)

\>z=z+normal(size(z))\*0.2;

\>plot2d(z,level=0.5,a=-1,b=2,c=-2,d=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-229.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-229.png)

\>z=z+normal(size(z))\*0.2;

\>plot2d(z,level=0.5,a=-1,b=2,c=-2,d=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-230.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-230.png)

\>plot2d(expr,level=[0:0.2:5;0.05:0.2:5.05],color=lightgray):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-231.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-231.png)

\>plot2d("x^2+y^3+x\*y",level=1,r=4,n=100):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-232.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-232.png)

\>plot2d("x^2+2\*y^2-x\*y",level=0:0.1:10,n=100,contourcolor=white,\>hue):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-233.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-233.png)

Dimungkinkan juga untuk mengisi set


dengan rentang level.


Dimungkinkan untuk mengisi wilayah nilai untuk fungsi tertentu. Untuk
ini, level harus berupa matriks 2xn. Baris pertama adalah batas bawah
dan baris kedua berisi batas atas.


\>plot2d(expr,level=[0;1],style="-",color=blue): // 0 <= f(x,y) <= 1


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-234.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-234.png)

Plot implisit juga dapat menunjukkan rentang level. Maka level harus
berupa matriks interval level 2xn, di mana baris pertama berisi awal
dan baris kedua berisi akhir setiap interval. Alternatifnya, vektor
baris sederhana dapat digunakan untuk level, dan parameter dl
memperluas nilai level ke interval.


\>plot2d("x^4+y^4",r=1.5,level=[0;1],color=blue,style="/"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-235.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-235.png)

\>plot2d("x^2+y^3+x\*y",level=[0,2,4;1,3,5],style="/",r=2,n=100):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-236.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-236.png)

\>plot2d("x^2+y^3+x\*y",level=-10:20,r=2,style="-",dl=0.1,n=100):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-237.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-237.png)

\>plot2d("sin(x)\*cos(y)",r=pi,\>hue,\>levels,n=100):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-238.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-238.png)

Dimungkinkan juga untuk menandai suatu wilayah


Hal ini dilakukan dengan menambahkan level dengan dua baris.


\>plot2d("(x^2+y^2-1)^3-x^2\*y^3",r=1.3, ...  
\>   style="#",color=red,<outline, ...  
\>   level=[-2;0],n=100):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-239.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-239.png)

Dimungkinkan untuk menentukan level tertentu. Misalnya, kita dapat
memplot solusi persamaan seperti


\>plot2d("x^3-x\*y+x^2\*y^2",r=6,level=1,n=100):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-240.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-240.png)

\>function starplot1 (v, style="/", color=green, lab=none) ...


    if !holding() then clg; endif;
    w=window(); window(0,0,1024,1024);
    h=holding(1);
      r=max(abs(v))*1.2;
      setplot(-r,r,-r,r);
      n=cols(v); t=linspace(0,2pi,n);
      v=v|v[1]; c=v*cos(t); s=v*sin(t);
      cl=barcolor(color); st=barstyle(style);
      loop 1 to n
        polygon([0,c[#],c[#+1]],[0,s[#],s[#+1]],1);
        if lab!=none then
          rlab=v[#]+r*0.1;
          {col,row}=toscreen(cos(t[#])*rlab,sin(t[#])*rlab);
          ctext(""+lab[#],col,row-textheight()/2);
        endif;
      end;
      barcolor(cl); barstyle(st);
      holding(h);
      window(w);
    endfunction
</pre>
Tidak ada tanda centang kotak atau sumbu di sini. Selain itu, kami
menggunakan jendela penuh untuk plotnya.


Kami memanggil reset sebelum kami menguji plot ini untuk mengembalikan
default grafis. Ini tidak perlu dilakukan jika Anda yakin plot Anda
berhasil.


\>reset; starplot1(normal(1,10)+5,color=red,lab=1:10):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-241.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-241.png)

Terkadang, Anda mungkin ingin merencanakan sesuatu yang plot2d tidak
bisa lakukan, tapi hampir.


Dalam fungsi berikut, kita membuat plot impuls logaritmik. plot2d
dapat melakukan plot logaritmik, tetapi tidak untuk batang impuls.


\>function logimpulseplot1 (x,y) ...


    {x0,y0}=makeimpulse(x,log(y)/log(10));
      plot2d(x0,y0,>bar,grid=0);
      h=holding(1);
      frame();
      xgrid(ticks(x));
      p=plot();
      for i=-10 to 10;
        if i<=p[4] and i>=p[3] then
           ygrid(i,yt="10^"+i);
        endif;
      end;
      holding(h);
    endfunction
</pre>
Mari kita uji dengan nilai yang terdistribusi secara eksponensial.


\>aspect(1.5); x=1:10; y=-log(random(size(x)))\*200; ...  
\>   logimpulseplot1(x,y):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-242.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-242.png)

Mari kita menganimasikan kurva 2D menggunakan plot langsung. Perintah
plot(x,y) hanya memplot kurva ke dalam jendela plot. setplot(a,b,c,d)
menyetel jendela ini.


Fungsi wait(0) memaksa plot muncul di jendela grafis. Jika tidak,
pengundian ulang akan dilakukan dalam interval waktu yang jarang.


\>function animliss (n,m) ...


    t=linspace(0,2pi,500);
    f=0;
    c=framecolor(0);
    l=linewidth(2);
    setplot(-1,1,-1,1);
    repeat
      clg;
      plot(sin(n*t),cos(m*t+f));
      wait(0);
      if testkey() then break; endif;
      f=f+0.02;
    end;
    framecolor(c);
    linewidth(l);
    endfunction
</pre>
Tekan tombol apa saja untuk menghentikan animasi ini.


\>animliss(2,3); // lihat hasilnya, jika sudah puas, tekan ENTER


# Plot Logaritmik

EMT menggunakan parameter "logplot" untuk skala logaritmik.


Plot logaritma dapat diplot menggunakan skala logaritma di y dengan
logplot=1, atau menggunakan skala logaritma di x dan y dengan
logplot=2, atau di x dengan logplot=3.


 - logplot=1: y-logaritma  
 - logplot=2: x-y-logaritma  
 - logplot=3: x-logaritma  

\>plot2d("exp(x^3-x)\*x^2",1,5,logplot=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-243.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-243.png)

\>plot2d("exp(x+sin(x))",0,100,logplot=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-244.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-244.png)

\>plot2d("exp(x+sin(x))",10,100,logplot=2):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-245.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-245.png)

\>plot2d("gamma(x)",1,10,logplot=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-246.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-246.png)

\>plot2d("log(x\*(2+sin(x/100)))",10,1000,logplot=3):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-247.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-247.png)

Ini juga berfungsi dengan plot data.


\>x=10^(1:20); y=x^2-x;

\>plot2d(x,y,logplot=2); 

\>hold off;


# Rujukan Lengkap Fungsi plot2d()

fungsi plot2d (xv, yv, btest, a, b, c, d, xmin, xmax, r, n, ..


logplot, kisi, bingkai, warna bingkai, kotak, warna, ketebalan, gaya,
..


otomatis, tambah, pengguna, delta, titik, titik tambahan, gaya titik,
batang, histogram, ..


distribusi, genap, langkah, milik, adaptif, rona, level, kontur, ..


nc, terisi, warna isi, garis besar, judul, xl, yl, peta, warna kontur,
..


lebar kontur, kutu, margin, kliping, cx, cy, insimg, spektral, ..


cgrid, vertikal, lebih kecil, dl, niveau, level)


Fungsi plot serbaguna untuk plot dalam bidang (plot 2D). Fungsi ini
dapat dilakukan


plot fungsi satu variabel, plot data, kurva pada bidang, plot batang,
grid


bilangan kompleks, dan plot implisit fungsi dua variabel.


Parameters


x,y       : equations, functions or data vectors


a,b,c,d   : Plot area (default a=-2,b=2)


r         : if r is set, then a=cx-r, b=cx+r, c=cy-r, d=cy+r


           r can be a vector [rx,ry] or a vector [rx1,rx2,ry1,ry2].


xmin,xmax : range of the parameter for curves


auto      : Determine y-range automatically (default)


square    : if true, try to keep square x-y-ranges


n         : number of intervals (default is adaptive)


grid      : 0 = no grid and labels,


            1 = axis only,


            2 = normal grid (see below for the number of grid lines)


            3 = inside axis


            4 = no grid


            5 = full grid including margin


            6 = ticks at the frame


            7 = axis only


            8 = axis only, sub-ticks


frame     : 0 = no frame


framecolor: color of the frame and the grid


margin    : number between 0 and 0.4 for the margin around the plot


color     : Color of curves. If this is a vector of colors,it will be
used for each row of a matrix of plots. In the case of point plots, it
should be a column vector. If a row vector or a full matrix of colors
is used for point plots, it will be used for each data point.


thickness : line thickness for curves


This value can be smaller than 1 for very thin lines.


style     : Plot style for lines, markers, and fills.


            For points use


            "[]", "&lt;&gt;", ".", "..", "...",


            "*", "+", "|", "-", "o"


            "[]#", "&lt;&gt;#", "o#" (filled shapes)


            "[]w", "&lt;&gt;w", "ow" (non-transparent)


            For lines use


            "-", "--", "-.", ".", ".-.", "-.-", "-&gt;"


            For filled polygons or bar plots use


            "#", "#O", "O", "/", "\", "\/",


            "+", "|", "-", "t"


points    : plot single points instead of line segments


addpoints : if true, plots line segments and points


add       : add the plot to the existing plot


user      : enable user interaction for functions


delta     : step size for user interaction


bar       : bar plot (x are the interval bounds, y the interval
values)


histogram : plots the frequencies of x in n subintervals


distribution=n : plots the distribution of x with n subintervals


even      : use inter values for automatic histograms.


steps     : plots the function as a step function (steps=1,2)


adaptive  : use adaptive plots (n is the minimal number of steps)


level     : plot level lines of an implicit function of two variables


outline   : draws boundary of level ranges.


If the level value is a 2xn matrix, ranges of levels will be drawn


in the color using the given fill style. If outline is true, it


will be drawn in the contour color. Using this feature, regions of


f(x,y) between limits can be marked.


hue       : add hue color to the level plot to indicate the function
value


contour   : Use level plot with automatic levels


nc        : number of automatic level lines


title     : plot title (default "")


xl, yl    : labels for the x- and y-axis


smaller   : if &gt;0, there will be more space to the left for labels.


vertical  :


  Mengaktifkan atau menonaktifkan label vertikal.Ini   mengubah
variabel global memberi label vertikal secara   lokal untuk satu plot.
Nilai 1 hanya ditetapkan secara   vertikal teks, nilai 2 menggunakan
label numerik   vertikal pada sumbu y.


filled    : fill the plot of a curve


fillcolor : fill color for bar and filled curves


outline   : boundary for filled polygons


logplot   : set logarithmic plots


            1 = logplot in y,


            2 = logplot in xy,


            3 = logplot in x


own       :


Sebuah string, yang menunjuk ke rutinitas plotnya sendiri. Dengan&gt;
pengguna, Anda mendapatkan interaksi pengguna yang sama seperti di
plot2d. Kisarannya akan ditentukan sebelum setiap panggilan ke fungsi
Anda.


maps      : map expressions (0 is faster), functions are always
mapped.


contourcolor : color of contour lines


contourwidth : width of contour lines


clipping     : toggles the clipping (default is true)


title        :


Ini dapat digunakan untuk mendeskripsikan plot. Judulnya akan muncul
di atas plotnya. Selain itu, label untuk sumbu x dan y dapat
ditambahkan xl="string" atau yl="string". Label lain dapat ditambahkan
dengan fungsi label() atau labelbox(). Judulnya bisa berupa unicode
string atau gambar rumus Lateks.


cgrid     :


Menentukan jumlah garis grid untuk plot grid yang kompleks. Harus
berupa pembagi ukuran matriks dikurangi 1 (jumlah subinterval). cgrid
dapat berupa vektor [cx,cy].


Ringkasan


Fungsinya dapat diplot


- ekspresi, kumpulan panggilan atau fungsi dari satu variabel,


- kurva parametrik,


- x data versus y data,


- fungsi implisit,


- plot batang,


- jaringan kompleks,


- poligon.


Jika fungsi atau ekspresi untuk xv diberikan, plot2d() akan menghitung
nilai dalam rentang tertentu menggunakan fungsi atau ekspresi. Itu
ekspresi harus berupa ekspresi dalam variabel x. Kisarannya harus
ditentukan dalam parameter a dan b kecuali rentang default [-2,2]
harus digunakan. Rentang y akan dihitung secara otomatis, kecuali c
dan d ditentukan, atau radius r, yang menghasilkan rentang [-r,r]
untuk x dan y. Untuk plot fungsi, plot2d akan menggunakan evaluasi
adaptif fungsi secara default. Untuk mempercepat plot untuk fungsi
yang rumit, nonaktifkan ini dengan &lt;adaptive, dan secara opsional
mengurangi jumlah interval n. Selain itu, plot2d() akan secara default
menggunakan pemetaan. Yaitu, ini akan menghitung elemen plot untuk
elemen. Jika ekspresi atau fungsi Anda dapat menangani a vektor x,
Anda dapat menonaktifkannya dengan &lt;maps untuk evaluasi lebih cepat.


Perhatikan bahwa plot adaptif selalu dihitung elemen demi elemen. Jika
fungsi atau ekspresi untuk xv dan yv ditentukan, plot2d() akan
menghitung kurva dengan nilai xv sebagai koordinat x dan nilai yv
sebagai koordinat y. Dalam hal ini, seharusnya ada kisaran ditentukan
untuk parameter menggunakan xmin, xmax. Ekspresi terkandung dalam
string harus selalu berupa ekspresi dalam variabel parameter x.


# Contoh Soal dan penyelesaiannya

\>clg; // clear screen

\>window(0,0,2045,2045); // use all of the window 

\>setplot(0,2,0,2); // set plot coordinates

\>hold on; // start overwrite mode

\>n=150; X=random(n,4); Y=random(n,4); // get random points

\>colors=rgb(random(n),random(n),random(n)); // get random colors

\>loop 1 to n; color(colors[#]); plot(X[#],Y[#]); end; // plot

\>hold off; // end overwrite mode

\>insimg; // insert to notebook


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-248.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-248.png)

# PLOT3D

# Menggambar Plot 3D dengan EMT

Ini adalah pengantar plot 3D di Euler. Kita memerlukan plot 3D untuk
memvisualisasikan fungsi dua variabel.


Euler menggambar fungsi tersebut menggunakan algoritma penyortiran
untuk menyembunyikan bagian di latar belakang. Secara umum, Euler
menggunakan proyeksi pusat. Defaultnya adalah dari kuadran x-y positif
ke arah titik asal x=y=z=0, tetapi sudut=0° terlihat dari arah sumbu
y. Sudut pandang dan tinggi dapat diubah.


Euler dapat memplot


* 
permukaan dengan bayangan dan garis datar atau rentang datar,

* 
awan titik,

* 
kurva parametrik,

* 
permukaan implisit.


Plot 3D suatu fungsi menggunakan plot3d. Cara termudah adalah memplot
ekspresi dalam x dan y. Parameter r mengatur rentang plot di sekitar
(0,0).


\>aspect(1.5); plot3d("x^2+sin(y)",-5,5,0,6\*pi):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-249.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-249.png)

\>plot3d("x^2+x\*sin(y)",-5,5,0,6\*pi):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-250.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-250.png)

Silakan lakukan modifikasi agar gambar "talang bergelombang" tersebut tidak lurus melainkan melengkung/melingkar, baik
melingkar secara mendatar maupun melingkar turun/naik (seperti papan peluncur pada kolam renang. Temukan rumusnya.


# Fungsi Dua Variabel

Untuk grafik fungsi, gunakan


* 
ekspresi sederhana dalam x dan y,

* 
nama fungsi dua variabel

* 
atau matriks data.


Defaultnya adalah kisi kawat yang terisi dengan warna berbeda di kedua
sisinya. Perhatikan bahwa jumlah interval kisi default adalah 10,
tetapi plot menggunakan jumlah persegi panjang 40x40 default untuk
membuat permukaan. Ini dapat diubah.


* 
n=40, n=[40,40]: jumlah garis kisi di setiap arah

* 
kisi=10, kisi=[10,10]: jumlah garis kisi di setiap arah.


Kami menggunakan default n=40 dan kisi=10.


\>plot3d("x^2+y^2"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-251.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-251.png)

Interaksi pengguna dimungkinkan dengan parameter &gt;user. Pengguna dapat
menekan tombol berikut.


* 
kiri, kanan, atas, bawah: mengubah sudut pandang

* 
+, -: memperbesar atau memperkecil

* 
a: menghasilkan anaglif (lihat di bawah)

* 
l: mengubah arah sumber cahaya (lihat di bawah)

* 
spasi: mengatur ulang ke default

* 
return: mengakhiri interaksi


\>plot3d("exp(-x^2+y^2)",\>user, ...  
\>     title="Turn with the vector keys (press return to finish)"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-252.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-252.png)

Rentang plot untuk fungsi dapat ditentukan dengan


* 
a,b: rentang x

* 
c,d: rentang y

* 
r: persegi simetris di sekitar (0,0).

* 
n: jumlah subinterval untuk plot.


Ada beberapa parameter untuk menskalakan fungsi atau mengubah tampilan
grafik.


fscale: skala ke nilai fungsi (default adalah &lt;fscale).


scale: angka atau vektor 1x2 untuk diskalakan ke arah x dan y.


frame: jenis frame (default 1).


\>plot3d("exp(-(x^2+y^2)/5)",r=10,n=80,fscale=4,scale=1.2,frame=3,\>user):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-253.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-253.png)

Tampilan dapat diubah dengan berbagai cara.


* 
jarak: jarak pandang ke plot.

* 
perbesaran: nilai perbesaran.

* 
sudut: sudut ke sumbu y negatif dalam radian.

* 
tinggi: tinggi tampilan dalam radian.


Nilai default dapat diperiksa atau diubah dengan fungsi view(). Fungsi
ini mengembalikan parameter dalam urutan di atas.


\>view


    [5,  2.6,  2,  0.4]

Jarak yang lebih dekat membutuhkan zoom yang lebih sedikit. Efeknya
lebih seperti lensa sudut lebar.


Dalam contoh berikut, sudut=0 dan tinggi=0 terlihat dari sumbu y
negatif. Label sumbu untuk y disembunyikan dalam kasus ini.


\>plot3d("x^2+y",distance=3,zoom=1,angle=pi/2,height=0):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-254.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-254.png)

Plot selalu mengarah ke tengah kubus plot. Anda dapat memindahkan
bagian tengah dengan parameter center.


\>plot3d("x^4+y^2",a=0,b=1,c=-1,d=1,angle=-20°,height=20°, ...  
\>     center=[0.4,0,0],zoom=5):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-255.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-255.png)

Plot diskalakan agar sesuai dengan kubus satuan untuk dilihat. Jadi
tidak perlu mengubah jarak atau zoom tergantung pada ukuran plot.
Namun, label merujuk pada ukuran sebenarnya.


Jika Anda menonaktifkannya dengan scale=false, Anda perlu berhati-hati
agar plot tetap sesuai dengan jendela plot, dengan mengubah jarak
tampilan atau zoom, dan memindahkan bagian tengah.


\>plot3d("5\*exp(-x^2-y^2)",r=2,<fscale,<scale,distance=13,height=50°, ...  
\>     center=[0,0,-2],frame=3):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-256.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-256.png)

Plot polar juga tersedia. Parameter polar=true menggambar plot polar.
Fungsi tersebut harus tetap berupa fungsi x dan y. Parameter "fscale"
menskalakan fungsi dengan skalanya sendiri. Jika tidak, fungsi
tersebut diskalakan agar sesuai dengan kubus.


\>plot3d("1/(x^2+y^2+1)",r=5,\>polar, ...  
\>   fscale=2,\>hue,n=100,zoom=4,\>contour,color=blue):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-257.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-257.png)

\>function f(r) := exp(-r/2)\*cos(r); ...  
\>   plot3d("f(x^2+y^2)",\>polar,scale=[1,1,0.4],r=pi,frame=3,zoom=4):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-258.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-258.png)

Parameter rotate memutar fungsi dalam x di sekitar sumbu x.


* 
rotate=1: Menggunakan sumbu x

* 
rotate=2: Menggunakan sumbu z


\>plot3d("x^2+1",a=-1,b=1,rotate=true,grid=5):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-259.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-259.png)

\>plot3d("x^2+1",a=-1,b=1,rotate=2,grid=5):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-260.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-260.png)

\>plot3d("sqrt(25-x^2)",a=0,b=5,rotate=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-261.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-261.png)

\>plot3d("x\*sin(x)",a=0,b=6pi,rotate=2):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-262.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-262.png)

Berikut adalah plot dengan tiga fungsi.


\>plot3d("x","x^2+y^2","y",r=2,zoom=3.5,frame=3):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-263.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-263.png)

# Plot Kontur

Untuk plot, Euler menambahkan garis kisi. Sebagai gantinya,
dimungkinkan untuk menggunakan garis level dan rona satu warna atau
rona warna spektral. Euler dapat menggambar tinggi fungsi pada plot
dengan bayangan. Dalam semua plot 3D, Euler dapat menghasilkan anaglif
merah/sian.


* 
&gt;hue: Mengaktifkan bayangan terang alih-alih kabel.

* 
&gt;contour: Memplot garis kontur otomatis pada plot.

* 
level=... (atau level): Vektor nilai untuk garis kontur.


Defaultnya adalah level="auto", yang menghitung beberapa garis level
secara otomatis. Seperti yang Anda lihat di plot, level sebenarnya
adalah rentang level.


Gaya default dapat diubah. Untuk plot kontur berikut, kami menggunakan
kisi yang lebih halus untuk titik 100x100, menskalakan fungsi dan
plot, dan menggunakan sudut pandang yang berbeda.


\>plot3d("exp(-x^2-y^2)",r=2,n=100,level="thin", ...  
\>    \>contour,\>spectral,fscale=1,scale=1.1,angle=45°,height=20°):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-264.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-264.png)

\>plot3d("exp(x\*y)",angle=100°,\>contour,color=green):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-265.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-265.png)

Shading default menggunakan warna abu-abu. Namun, rentang warna
spektral juga tersedia.


* 
&gt;spectral: Menggunakan skema spektral default

* 
color=...: Menggunakan warna khusus atau skema spektral


Untuk plot berikut, kami menggunakan skema spektral default dan
menambah jumlah titik untuk mendapatkan tampilan yang sangat halus.


\>plot3d("x^2+y^2",\>spectral,\>contour,n=100):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-266.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-266.png)

Alih-alih garis level otomatis, kita juga dapat mengatur nilai garis
level. Ini akan menghasilkan garis level tipis, bukan rentang level.


\>plot3d("x^2-y^2",0,5,0,5,level=-1:0.1:1,color=redgreen):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-267.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-267.png)

Dalam plot berikut, kami menggunakan dua pita level yang sangat lebar
dari -0,1 hingga 1, dan dari 0,9 hingga 1. Ini dimasukkan sebagai
matriks dengan batas level sebagai kolom.


Selain itu, kami melapisi kisi dengan 10 interval di setiap arah.


\>plot3d("x^2+y^3",level=[-0.1,0.9;0,1], ...  
\>     \>spectral,angle=30°,grid=10,contourcolor=gray):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-268.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-268.png)

Dalam contoh berikut, kami memplot himpunan, di mana


Kami menggunakan satu garis tipis untuk garis datar.


\>plot3d("x^y-y^x",level=0,a=0,b=6,c=0,d=6,contourcolor=red,n=100):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-269.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-269.png)

Dimungkinkan untuk menunjukkan bidang kontur di bawah plot. Warna dan
jarak ke plot dapat ditentukan.


\>plot3d("x^2+y^4",\>cp,cpcolor=green,cpdelta=0.2):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-270.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-270.png)

Berikut ini beberapa gaya lainnya. Kami selalu menonaktifkan bingkai,
dan menggunakan berbagai skema warna untuk plot dan kisi.


\>figure(2,2); ...  
\>   expr="y^3-x^2"; ...  
\>   figure(1);  ...  
\>     plot3d(expr,<frame,\>cp,cpcolor=spectral); ...  
\>   figure(2);  ...  
\>     plot3d(expr,<frame,\>spectral,grid=10,cp=2); ...  
\>   figure(3);  ...  
\>     plot3d(expr,<frame,\>contour,color=gray,nc=5,cp=3,cpcolor=greenred); ...  
\>   figure(4);  ...  
\>     plot3d(expr,<frame,\>hue,grid=10,\>transparent,\>cp,cpcolor=gray); ...  
\>   figure(0):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-271.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-271.png)

Ada beberapa skema spektral lain, yang diberi nomor dari 1 hingga 9.
Namun, Anda juga dapat menggunakan color=value, di mana value


* 
spektral: untuk rentang dari biru hingga merah

* 
putih: untuk rentang yang lebih redup

* 
kuning biru, ungu hijau, biru kuning, hijau merah

* 
biru kuning, hijau ungu, kuning biru, merah hijau


\>figure(3,3); ...  
\>   for i=1:9;  ...  
\>     figure(i); plot3d("x^2+y^2",spectral=i,\>contour,\>cp,<frame,zoom=4);  ...  
\>   end; ...  
\>   figure(0):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-272.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-272.png)

Sumber cahaya dapat diubah dengan l dan tombol kursor selama interaksi
pengguna. Sumber cahaya juga dapat diatur dengan parameter.


* 
light: arah cahaya

* 
amb: cahaya sekitar antara 0 dan 1


Perlu dicatat bahwa program tidak membuat perbedaan antara sisi plot.
Tidak ada bayangan. Untuk ini, Anda memerlukan Povray.


\>plot3d("-x^2-y^2", ...  
\>     hue=true,light=[0,1,1],amb=0,user=true, ...  
\>     title="Press l and cursor keys (return to exit)"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-273.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-273.png)

Parameter warna mengubah warna permukaan. Warna garis level juga dapat
diubah.


\>plot3d("-x^2-y^2",color=rgb(0.2,0.2,0),hue=true,frame=false, ...  
\>     zoom=3,contourcolor=red,level=-2:0.1:1,dl=0.01):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-274.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-274.png)

Warna 0 memberikan efek pelangi khusus.


\>plot3d("x^2/(x^2+y^2+1)",color=0,hue=true,grid=10):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-275.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-275.png)

Permukaannya juga bisa transparan.


\>plot3d("x^2+y^2",\>transparent,grid=10,wirecolor=red):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-276.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-276.png)

# Plot Implisit

Ada juga plot implisit dalam tiga dimensi. Euler menghasilkan potongan
melalui objek. Fitur plot3d mencakup plot implisit. Plot ini
menunjukkan himpunan nol dari suatu fungsi dalam tiga variabel.


Solusi dari


dapat divisualisasikan dalam potongan yang sejajar dengan bidang x-y,
x-z, dan y-z.


* 
implisit=1: potongan sejajar dengan bidang y-z

* 
implisit=2: potongan sejajar dengan bidang x-z

* 
implisit=4: potongan sejajar dengan bidang x-y


Tambahkan nilai-nilai ini, jika Anda suka. Dalam contoh ini, kami
memplot


\>plot3d("x^2+y^3+z\*y-1",r=5,implicit=3):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-277.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-277.png)

\>c=1; d=1;

\>plot3d("((x^2+y^2-c^2)^2+(z^2-1)^2)\*((y^2+z^2-c^2)^2+(x^2-1)^2)\*((z^2+x^2-c^2)^2+(y^2-1)^2)-d",r=2,<frame,\>implicit,\>user): 


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-278.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-278.png)

\>plot3d("x^2+y^2+4\*x\*z+z^3",\>implicit,r=2,zoom=2.5):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-279.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-279.png)

# Membuat Plot Data 3D

Sama seperti plot2d, plot3d menerima data. Untuk objek 3D, Anda perlu
menyediakan matriks nilai x, y, dan z, atau tiga fungsi atau ekspresi
fx(x,y), fy(x,y), fz(x,y).


Karena x,y,z adalah matriks, kami berasumsi bahwa (t,s) berjalan
melalui kisi persegi. Hasilnya, Anda dapat membuat plot gambar persegi
panjang di ruang angkasa.


Anda dapat menggunakan bahasa matriks Euler untuk menghasilkan
koordinat secara efektif.


Dalam contoh berikut, kami menggunakan vektor nilai t dan vektor kolom
nilai s untuk membuat parameter permukaan bola. Dalam gambar, kami
dapat menandai wilayah, dalam kasus kami wilayah kutub.


\>t=linspace(0,2pi,180); s=linspace(-pi/2,pi/2,90)'; ...  
\>   x=cos(s)\*cos(t); y=cos(s)\*sin(t); z=sin(s); ...  
\>   plot3d(x,y,z,\>hue, ...  
\>   color=blue,<frame,grid=[10,20], ...  
\>   values=s,contourcolor=red,level=[90°-24°;90°-22°], ...  
\>   scale=1.4,height=50°):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-280.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-280.png)

Berikut adalah contoh, yang merupakan grafik suatu fungsi.


\>t=-1:0.1:1; s=(-1:0.1:1)'; plot3d(t,s,t\*s,grid=10):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-281.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-281.png)

Namun, kita dapat membuat berbagai macam permukaan. Berikut ini adalah
permukaan yang sama sebagai fungsi


lateks: x = y \, z


\>plot3d(t\*s,t,s,angle=180°,grid=10):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-282.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-282.png)

With more effort, we can produce many surfaces.


In the following example we make a shaded view of a distorted ball. The usual coordinates for the ball are


with


We distored this with a factor


\>t=linspace(0,2pi,320); s=linspace(-pi/2,pi/2,160)'; ...  
\>   d=1+0.2\*(cos(4\*t)+cos(8\*s)); ...  
\>   plot3d(cos(t)\*cos(s)\*d,sin(t)\*cos(s)\*d,sin(s)\*d,hue=1, ...  
\>     light=[1,0,1],frame=0,zoom=5):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-283.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-283.png)

Tentu saja, titik awan juga memungkinkan. Untuk memplot data titik di
ruang, kita memerlukan tiga vektor untuk koordinat titik.


Gayanya sama seperti di plot2d dengan points=true;


\>n=500;  ...  
\>     plot3d(normal(1,n),normal(1,n),normal(1,n),points=true,style="."):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-284.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-284.png)

Anda juga dapat memplot kurva dalam 3D. Dalam kasus ini, lebih mudah
untuk menghitung titik-titik kurva terlebih dahulu. Untuk kurva dalam
bidang, kami menggunakan urutan koordinat dan parameter wire=true.


\>t=linspace(0,8pi,500); ...  
\>   plot3d(sin(t),cos(t),t/10,\>wire,zoom=3):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-285.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-285.png)

\>t=linspace(0,4pi,1000); plot3d(cos(t),sin(t),t/2pi,\>wire, ...  
\>   linewidth=3,wirecolor=blue):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-286.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-286.png)

\>X=cumsum(normal(3,100)); ...  
\>    plot3d(X[1],X[2],X[3],\>anaglyph,\>wire):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-287.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-287.png)

EMT juga dapat membuat grafik dalam mode anaglif. Untuk melihat grafik
tersebut, Anda memerlukan kacamata merah/sian.


\> plot3d("x^2+y^3",\>anaglyph,\>contour,angle=30°):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-288.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-288.png)

Seringkali, skema warna spektral digunakan untuk plot. Ini menekankan
tinggi fungsi.


\>plot3d("x^2\*y^3-y",\>spectral,\>contour,zoom=3.2):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-289.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-289.png)

Euler juga dapat memplot permukaan berparameter, ketika parameternya
adalah nilai x, y, dan z dari gambar kotak persegi panjang di ruang
tersebut.


Untuk demo berikut, kami menyiapkan parameter u dan v, dan
menghasilkan koordinat ruang dari parameter tersebut.


\>u=linspace(-1,1,10); v=linspace(0,2\*pi,50)'; ...  
\>   X=(3+u\*cos(v/2))\*cos(v); Y=(3+u\*cos(v/2))\*sin(v); Z=u\*sin(v/2); ...  
\>   plot3d(X,Y,Z,\>anaglyph,<frame,\>wire,scale=2.3):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-290.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-290.png)

Berikut adalah contoh yang lebih rumit, yang tampak megah dengan kaca
merah/cyan.


\>u:=linspace(-pi,pi,160); v:=linspace(-pi,pi,400)';  ...  
\>   x:=(4\*(1+.25\*sin(3\*v))+cos(u))\*cos(2\*v); ...  
\>   y:=(4\*(1+.25\*sin(3\*v))+cos(u))\*sin(2\*v); ...  
\>    z=sin(u)+2\*cos(3\*v); ...  
\>   plot3d(x,y,z,frame=0,scale=1.5,hue=1,light=[1,0,-1],zoom=2.8,\>anaglyph):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-291.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-291.png)

# Plot Statistik

Plot batang juga dimungkinkan. Untuk ini, kita harus menyediakan


* 
x: vektor baris dengan n+1 elemen

* 
y: vektor kolom dengan n+1 elemen

* 
z: matriks nilai nxn.


z dapat lebih besar, tetapi hanya nilai nxn yang akan digunakan.


Dalam contoh, pertama-tama kita menghitung nilai. Kemudian kita
menyesuaikan x dan y, sehingga vektor berpusat pada nilai yang
digunakan.


\>x=-1:0.1:1; y=x'; z=x^2+y^2; ...  
\>   xa=(x|1.1)-0.05; ya=(y\_1.1)-0.05; ...  
\>   plot3d(xa,ya,z,bar=true):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-292.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-292.png)

Dimungkinkan untuk membagi bidang permukaan menjadi dua bagian atau
lebih.


\>x=-1:0.1:1; y=x'; z=x+y; d=zeros(size(x)); ...  
\>   plot3d(x,y,z,disconnect=2:2:20):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-293.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-293.png)

Jika memuat atau membuat matriks data M dari sebuah file dan perlu
memplotnya dalam 3D, Anda dapat menskalakan matriks ke [-1,1] dengan
scale(M), atau menskalakan matriks dengan &gt;zscale. Ini dapat
dikombinasikan dengan faktor penskalaan individual yang diterapkan
sebagai tambahan.


\>i=1:20; j=i'; ...  
\>   plot3d(i\*j^2+100\*normal(20,20),\>zscale,scale=[1,1,1.5],angle=-40°,zoom=1.8):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-294.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-294.png)

\>Z=intrandom(5,100,6); v=zeros(5,6); ...  
\>   loop 1 to 5; v[#]=getmultiplicities(1:6,Z[#]); end; ...  
\>   columnsplot3d(v',scols=1:5,ccols=[1:5]):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-295.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-295.png)

# Permukaan Benda Putar

\>plot2d("(x^2+y^2-1)^3-x^2\*y^3",r=1.3, ...  
\>   style="#",color=red,<outline, ...  
\>   level=[-2;0],n=100):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-296.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-296.png)

\>ekspresi &= (x^2+y^2-1)^3-x^2\*y^3; $ekspresi


$$\left(y^2+x^2-1\right)^3-x^2\,y^3$$Kita ingin memutar kurva jantung di sekitar sumbu y. Berikut ini
adalah ekspresi yang mendefinisikan jantung:


Selanjutnya kita tetapkan


\>function fr(r,a) &= ekspresi with [x=r\*cos(a),y=r\*sin(a)] | trigreduce; $fr(r,a)


$$\left(r^2-1\right)^3+\frac{\left(\sin \left(5\,a\right)-\sin \left(
 3\,a\right)-2\,\sin a\right)\,r^5}{16}$$Hal ini memungkinkan untuk mendefinisikan fungsi numerik, yang
memecahkan r, jika a diberikan. Dengan fungsi itu kita dapat memplot
jantung yang diputar sebagai permukaan parametrik.


\>function map f(a) := bisect("fr",0,2;a); ...  
\>   t=linspace(-pi/2,pi/2,100); r=f(t);  ...  
\>   s=linspace(pi,2pi,100)'; ...  
\>   plot3d(r\*cos(t)\*sin(s),r\*cos(t)\*cos(s),r\*sin(t), ...  
\>   \>hue,<frame,color=red,zoom=4,amb=0,max=0.7,grid=12,height=50°):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-299.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-299.png)

Berikut ini adalah plot 3D dari gambar di atas yang diputar di sekitar
sumbu z. Kami mendefinisikan fungsi yang menggambarkan objek tersebut.


\>function f(x,y,z) ...


    r=x^2+y^2;
    return (r+z^2-1)^3-r*z^3;
     endfunction
</pre>
\>plot3d("f(x,y,z)", ...  
\>   xmin=0,xmax=1.2,ymin=-1.2,ymax=1.2,zmin=-1.2,zmax=1.4, ...  
\>   implicit=1,angle=-30°,zoom=2.5,n=[10,100,60],\>anaglyph):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-300.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-300.png)

# Plot 3D Khusus

Fungsi plot3d memang bagus, tetapi tidak memenuhi semua kebutuhan.
Selain rutinitas yang lebih mendasar, Anda dapat memperoleh plot
berbingkai dari objek apa pun yang Anda suka.


Meskipun Euler bukanlah program 3D, ia dapat menggabungkan beberapa
objek dasar. Kami mencoba memvisualisasikan parabola dan garis
singgungnya.


\>function myplot ...


      y=-1:0.01:1; x=(-1:0.01:1)';
      plot3d(x,y,0.2*(x-0.1)/2,<scale,<frame,>hue, ..
        hues=0.5,>contour,color=orange);
      h=holding(1);
      plot3d(x,y,(x^2+y^2)/2,<scale,<frame,>contour,>hue);
      holding(h);
    endfunction
</pre>
Sekarang framedplot() menyediakan bingkai dan mengatur tampilan.


\>framedplot("myplot",[-1,1,-1,1,0,1],height=0,angle=-30°, ...  
\>     center=[0,0,-0.7],zoom=3):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-301.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-301.png)

Dengan cara yang sama, Anda dapat memplot bidang kontur secara manual.
Perhatikan bahwa plot3d() menetapkan jendela ke fullwindow() secara
default, tetapi plotcontourplane() mengasumsikannya.


\>x=-1:0.02:1.1; y=x'; z=x^2-y^4;

\>function myplot (x,y,z) ...  
\>  
<pre class="udf">      zoom(2);
      wi=fullwindow();
      plotcontourplane(x,y,z,level="auto",<scale);
      plot3d(x,y,z,>hue,<scale,>add,color=white,level="thin");
      window(wi);
      reset();
    endfunction
</pre>
\>myplot(x,y,z):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-302.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-302.png)

# Animasi

Euler dapat menggunakan bingkai untuk melakukan pra-komputasi animasi.


Salah satu fungsi yang memanfaatkan teknik ini adalah rotate. Fungsi
ini dapat mengubah sudut pandang dan menggambar ulang plot 3D. Fungsi
ini memanggil addpage() untuk setiap plot baru. Terakhir, fungsi ini
menganimasikan plot tersebut.


Silakan pelajari sumber rotate untuk melihat detail selengkapnya.


\>function testplot () := plot3d("x^2+y^3"); ...  
\>   rotate("testplot"); testplot():


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-303.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-303.png)

# Menggambar Povray

Dengan bantuan file Euler povray.e, Euler dapat membuat file Povray.
Hasilnya sangat bagus untuk dilihat.


Anda perlu menginstal Povray (32bit atau 64bit) dari
  <a href="http://www.povray.org/, dan meletakkan subdirektori "bin" dari Povray ke dalam jalur lingkungan, atau mengatur variabel "defaultpovray" dengan jalur lengkap yang mengarah ke "pvengine.exe".">http://www.povray.org/, dan meletakkan subdirektori "bin" dari Povray ke dalam jalur lingkungan, atau mengatur variabel "defaultpovray" dengan jalur lengkap yang mengarah ke "pvengine.exe".</a>


Antarmuka Povray dari Euler membuat file Povray di direktori home
pengguna, dan memanggil Povray untuk mengurai file-file ini. Nama file
default adalah current.pov, dan direktori default adalah eulerhome(),
biasanya c:\Users\Username\Euler. Povray membuat file PNG, yang dapat
dimuat oleh Euler ke dalam buku catatan. Untuk membersihkan file-file
ini, gunakan povclear().


Fungsi pov3d memiliki semangat yang sama dengan plot3d. Fungsi ini
dapat menghasilkan grafik fungsi f(x,y), atau permukaan dengan
koordinat X,Y,Z dalam matriks, termasuk garis level opsional. Fungsi
ini memulai raytracer secara otomatis, dan memuat adegan ke dalam buku
catatan Euler.


Selain pov3d(), ada banyak fungsi, yang menghasilkan objek Povray.
Fungsi-fungsi ini mengembalikan string, yang berisi kode Povray untuk
objek. Untuk menggunakan fungsi-fungsi ini, mulai file Povray dengan
povstart(). Kemudian gunakan writeln(...) untuk menulis objek ke file
adegan. Terakhir, akhiri file dengan povend(). Secara default,
raytracer akan mulai, dan PNG akan dimasukkan ke dalam buku catatan
Euler.


Fungsi objek memiliki parameter yang disebut "look", yang memerlukan
string dengan kode Povray untuk tekstur dan penyelesaian objek. Fungsi
povlook() dapat digunakan untuk menghasilkan string ini. Fungsi ini
memiliki parameter untuk warna, transparansi, Phong Shading, dll.


Perhatikan bahwa alam semesta Povray memiliki sistem koordinat lain.
Antarmuka ini menerjemahkan semua koordinat ke sistem Povray. Jadi
Anda dapat terus berpikir dalam sistem koordinat Euler dengan z
menunjuk vertikal ke atas, dan sumbu x, y, z dalam arah kanan.


Anda perlu memuat berkas povray.


\>load povray;


Pastikan direktori bin Povray ada di jalur tersebut. Jika tidak, edit
variabel berikut sehingga berisi jalur ke povray yang dapat
dieksekusi.


\>defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

Untuk kesan pertama, kami membuat fungsi sederhana. Perintah berikut
menghasilkan file povray di direktori pengguna Anda, dan menjalankan
Povray untuk melakukan ray tracing pada file ini.


Jika Anda menjalankan perintah berikut, GUI Povray akan terbuka,
menjalankan file, dan menutup secara otomatis. Karena alasan keamanan,
Anda akan ditanya apakah Anda ingin mengizinkan file exe untuk
berjalan. Anda dapat menekan batal untuk menghentikan pertanyaan lebih
lanjut. Anda mungkin harus menekan OK di jendela Povray untuk mengakui
dialog awal Povray.


\>plot3d("x^2+y^2",zoom=2):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-304.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-304.png)

Kita dapat membuat fungsi tersebut transparan dan menambahkan
penyelesaian lainnya. Kita juga dapat menambahkan garis level pada
plot fungsi.


\>pov3d("x^2+y^3",axiscolor=red,angle=-45°,\>anaglyph, ...  
\>     look=povlook(cyan,0.2),level=-1:0.5:1,zoom=3.8);


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-305.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-305.png)

Terkadang perlu untuk mencegah penskalaan fungsi, dan menskalakan
fungsi secara manual.


Kami memplot himpunan titik pada bidang kompleks, di mana hasil kali
jarak ke 1 dan -1 sama dengan 1.


\>pov3d("((x-1)^2+y^2)\*((x+1)^2+y^2)/40",r=2, ...  
\>     angle=-120°,level=1/40,dlevel=0.005,light=[-1,1,1],height=10°,n=50, ...  
\>     <fscale,zoom=3.8);


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-306.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-306.png)

# Membuat Plot dengan Koordinat

Alih-alih menggunakan fungsi, kita dapat membuat plot dengan
koordinat. Seperti pada plot3d, kita memerlukan tiga matriks untuk
menentukan objek.


Dalam contoh ini, kita memutar fungsi di sekitar sumbu z.


\>function f(x) := x^3-x+1; ...  
\>   x=-1:0.01:1; t=linspace(0,2pi,50)'; ...  
\>   Z=x; X=cos(t)\*f(x); Y=sin(t)\*f(x); ...  
\>   pov3d(X,Y,Z,angle=40°,look=povlook(red,0.1),height=50°,axis=0,zoom=4,light=[10,5,15]);


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-307.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-307.png)

Dalam contoh berikut, kami memplot gelombang yang diredam. Kami
menghasilkan gelombang dengan bahasa matriks Euler.


Kami juga menunjukkan, bagaimana objek tambahan dapat ditambahkan ke
adegan pov3d. Untuk pembuatan objek, lihat contoh berikut. Perhatikan
bahwa plot3d menskalakan plot, sehingga sesuai dengan kubus satuan.


\>r=linspace(0,1,80); phi=linspace(0,2pi,80)'; ...  
\>   x=r\*cos(phi); y=r\*sin(phi); z=exp(-5\*r)\*cos(8\*pi\*r)/3;  ...  
\>   pov3d(x,y,z,zoom=6,axis=0,height=30°,add=povsphere([0.5,0,0.25],0.15,povlook(red)), ...  
\>     w=500,h=300);


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-308.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-308.png)

Dengan metode shading Povray yang canggih, hanya sedikit titik yang
dapat menghasilkan permukaan yang sangat halus. Hanya pada batas dan
bayangan, triknya mungkin menjadi jelas.


Untuk ini, kita perlu menambahkan vektor normal di setiap titik
matriks.


\>Z &= x^2\*y^3


    
                                     2  3
                                    x  y
    

Persamaan permukaannya adalah [x,y,Z]. Kita hitung dua turunan x dan y
dari persamaan ini dan ambil perkalian silang sebagai normalnya.


\>dx &= diff([x,y,Z],x); dy &= diff([x,y,Z],y);


Kami mendefinisikan normal sebagai perkalian silang turunan-turunan
ini dan mendefinisikan fungsi koordinat.


\>N &= crossproduct(dx,dy); NX &= N[1]; NY &= N[2]; NZ &= N[3]; N,


    
                                   3       2  2
                           [- 2 x y , - 3 x  y , 1]
    

Kami hanya menggunakan 25 poin.


\>x=-1:0.5:1; y=x';

\>pov3d(x,y,Z(x,y),angle=10°, ...  
\>     xv=NX(x,y),yv=NY(x,y),zv=NZ(x,y),<shadow);


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-309.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-309.png)

Berikut ini adalah simpul Trefoil yang dibuat oleh A. Busser di
Povray. Ada versi yang lebih baik dari simpul ini dalam
contoh-contohnya.


Lihat: Contoh\Simpul Trefoil | Simpul Trefoil


Untuk tampilan yang bagus dengan tidak terlalu banyak titik, kami
menambahkan vektor normal di sini. Kami menggunakan Maxima untuk
menghitung normal bagi kami. Pertama, tiga fungsi untuk koordinat
sebagai ekspresi simbolik.


\>X &= ((4+sin(3\*y))+cos(x))\*cos(2\*y); ...  
\>   Y &= ((4+sin(3\*y))+cos(x))\*sin(2\*y); ...  
\>   Z &= sin(x)+2\*cos(3\*y);


Kemudian dua vektor turunan ke x dan y.


\>dx &= diff([X,Y,Z],x); dy &= diff([X,Y,Z],y);


Sekarang normal, yang merupakan perkalian silang dari dua turunan.


\>dn &= crossproduct(dx,dy);


Sekarang mari kita evaluasi semua ini secara numerik.


\>x:=linspace(-%pi,%pi,40); y:=linspace(-%pi,%pi,100)';


Vektor normal adalah evaluasi ekspresi simbolik dn[i] untuk i=1,2,3.
Sintaks untuk ini adalah &amp;"ekspresi"(parameter). Ini adalah alternatif
untuk metode pada contoh sebelumnya, di mana kita mendefinisikan
ekspresi simbolik NX, NY, NZ terlebih dahulu.


\>pov3d(X(x,y),Y(x,y),Z(x,y),\>anaglyph,axis=0,zoom=5,w=450,h=350, ...  
\>     <shadow,look=povlook(blue), ...  
\>     xv=&"dn[1]"(x,y), yv=&"dn[2]"(x,y), zv=&"dn[3]"(x,y));


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-310.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-310.png)

Kita juga dapat membuat grid dalam 3D.


\>povstart(zoom=4); ...  
\>   x=-1:0.5:1; r=1-(x+1)^2/6; ...  
\>   t=(0°:30°:360°)'; y=r\*cos(t); z=r\*sin(t); ...  
\>   writeln(povgrid(x,y,z,d=0.02,dballs=0.05)); ...  
\>   povend();


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-311.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-311.png)

Dengan povgrid(), kurva dimungkinkan.


\>povstart(center=[0,0,1],zoom=3.6); ...  
\>   t=linspace(0,2,1000); r=exp(-t); ...  
\>   x=cos(2\*pi\*10\*t)\*r; y=sin(2\*pi\*10\*t)\*r; z=t; ...  
\>   writeln(povgrid(x,y,z,povlook(red))); ...  
\>   writeAxis(0,2,axis=3); ...  
\>   povend();


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-312.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-312.png)

# Objek Povray

Di atas, kami menggunakan pov3d untuk memplot permukaan. Antarmuka
povray di Euler juga dapat menghasilkan objek Povray. Objek-objek ini
disimpan sebagai string di Euler, dan perlu ditulis ke berkas Povray.


Kami memulai output dengan povstart().


\>povstart(zoom=4);


Pertama, kita mendefinisikan tiga silinder, dan menyimpannya dalam
string di Euler.


Fungsi povx() dll. hanya mengembalikan vektor [1,0,0], yang dapat
digunakan sebagai gantinya.


\>c1=povcylinder(-povx,povx,1,povlook(red)); ...  
\>   c2=povcylinder(-povy,povy,1,povlook(yellow)); ...  
\>   c3=povcylinder(-povz,povz,1,povlook(blue)); ...  
\>  
Rangkaian tersebut berisi kode Povray, yang tidak perlu kita pahami
saat itu.


\>c2


    cylinder { &lt;0,0,-1&gt;, &lt;0,0,1&gt;, 1
     texture { pigment { color rgb &lt;0.941176,0.941176,0.392157&gt; }  } 
     finish { ambient 0.2 } 
     }

Seperti yang Anda lihat, kami menambahkan tekstur ke objek dalam tiga
warna berbeda.


Hal itu dilakukan oleh povlook(), yang mengembalikan string dengan
kode Povray yang relevan. Kita dapat menggunakan warna Euler default,
atau menentukan warna kita sendiri. Kita juga dapat menambahkan
transparansi, atau mengubah cahaya sekitar.


\>povlook(rgb(0.1,0.2,0.3),0.1,0.5)


     texture { pigment { color rgbf &lt;0.101961,0.2,0.301961,0.1&gt; }  } 
     finish { ambient 0.5 } 
    

Sekarang kita mendefinisikan objek persimpangan dan menulis hasilnya
ke berkas.


\>writeln(povintersection([c1,c2,c3]));


Persimpangan tiga silinder sulit dibayangkan, jika Anda belum pernah
melihatnya sebelumnya.


\>povend;


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-313.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-313.png)

Fungsi-fungsi berikut menghasilkan fraktal secara rekursif.


Fungsi pertama menunjukkan bagaimana Euler menangani objek-objek
Povray sederhana. Fungsi povbox() mengembalikan string yang berisi
koordinat kotak, tekstur, dan hasil akhir.


\>function onebox(x,y,z,d) := povbox([x,y,z],[x+d,y+d,z+d],povlook());

\>function fractal (x,y,z,h,n) ...  
\>  
<pre class="udf">     if n==1 then writeln(onebox(x,y,z,h));
     else
       h=h/3;
       fractal(x,y,z,h,n-1);
       fractal(x+2*h,y,z,h,n-1);
       fractal(x,y+2*h,z,h,n-1);
       fractal(x,y,z+2*h,h,n-1);
       fractal(x+2*h,y+2*h,z,h,n-1);
       fractal(x+2*h,y,z+2*h,h,n-1);
       fractal(x,y+2*h,z+2*h,h,n-1);
       fractal(x+2*h,y+2*h,z+2*h,h,n-1);
       fractal(x+h,y+h,z+h,h,n-1);
     endif;
    endfunction
</pre>
\>povstart(fade=10,<shadow);

\>fractal(-1,-1,-1,2,4);

\>povend();


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-314.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-314.png)

Perbedaan memungkinkan pemisahan satu objek dari objek lainnya.
Seperti halnya persimpangan, ada beberapa objek CSG dari Povray.


\>povstart(light=[5,-5,5],fade=10);


Untuk demonstrasi ini, kami mendefinisikan objek dalam Povray,
alih-alih menggunakan string dalam Euler. Definisi langsung ditulis ke
berkas.


Koordinat kotak -1 berarti [-1,-1,-1].


\>povdefine("mycube",povbox(-1,1));


Kita dapat menggunakan objek ini dalam povobject(), yang mengembalikan
string seperti biasa.


\>c1=povobject("mycube",povlook(red));


Kita buat kubus kedua, lalu putar dan ubah skalanya sedikit.


\>c2=povobject("mycube",povlook(yellow),translate=[1,1,1], ...  
\>     rotate=xrotate(10°)+yrotate(10°), scale=1.2);


Lalu kita ambil selisih kedua benda tersebut.


\>writeln(povdifference(c1,c2));


Sekarang tambahkan tiga sumbu.


\>writeAxis(-1.2,1.2,axis=1); ...  
\>   writeAxis(-1.2,1.2,axis=2); ...  
\>   writeAxis(-1.2,1.2,axis=4); ...  
\>   povend();


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-315.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-315.png)

# Fungsi Implisit

Povray dapat memplot himpunan di mana f(x,y,z)=0, sama seperti
parameter implisit dalam plot3d. Namun, hasilnya terlihat jauh lebih
baik.


Sintaks untuk fungsi-fungsi tersebut sedikit berbeda. Anda tidak dapat
menggunakan output dari ekspresi Maxima atau Euler.


\>povstart(angle=70°,height=50°,zoom=4);

\>c=0.1; d=0.1; ...  
\>   writeln(povsurface("(pow(pow(x,2)+pow(y,2)-pow(c,2),2)+pow(pow(z,2)-1,2))\*(pow(pow(y,2)+pow(z,2)-pow(c,2),2)+pow(pow(x,2)-1,2))\*(pow(pow(z,2)+pow(x,2)-pow(c,2),2)+pow(pow(y,2)-1,2))-d",povlook(red))); ...  
\>   povend();


    Error : Povray error!
    
    Error generated by error() command
    
    povray:
        error("Povray error!");
    Try "trace errors" to inspect local variables after errors.
    povend:
        povray(file,w,h,aspect,exit); 

\>povstart(angle=25°,height=10°); 

\>writeln(povsurface("pow(x,2)+pow(y,2)\*pow(z,2)-1",povlook(blue),povbox(-2,2,"")));

\>povend();


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-316.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-316.png)

\>povstart(angle=70°,height=50°,zoom=4);


Buat permukaan implisit. Perhatikan sintaksis yang berbeda dalam
ekspresi.


\>writeln(povsurface("pow(x,2)\*y-pow(y,3)-pow(z,2)",povlook(green))); ...  
\>   writeAxes(); ...  
\>   povend();


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-317.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-317.png)

# Objek Mesh

Dalam contoh ini, kami menunjukkan cara membuat objek mesh, dan
menggambarnya dengan informasi tambahan.


Kami ingin memaksimalkan xy dalam kondisi x+y=1 dan menunjukkan
sentuhan tangensial garis-garis level.


\>povstart(angle=-10°,center=[0.5,0.5,0.5],zoom=7);


Kita tidak dapat menyimpan objek dalam string seperti sebelumnya,
karena terlalu besar. Jadi kita mendefinisikan objek dalam file Povray
menggunakan #declare. Fungsi povtriangle() melakukan ini secara
otomatis. Fungsi ini dapat menerima vektor normal seperti pov3d().


Berikut ini mendefinisikan objek mesh, dan langsung menuliskannya ke
dalam file.


\>x=0:0.02:1; y=x'; z=x\*y; vx=-y; vy=-x; vz=1;

\>mesh=povtriangles(x,y,z,"",vx,vy,vz);


Sekarang kita definisikan dua cakram, yang akan berpotongan dengan
permukaan.


\>cl=povdisc([0.5,0.5,0],[1,1,0],2); ...  
\>   ll=povdisc([0,0,1/4],[0,0,1],2);


Tuliskan permukaan dikurangi kedua cakram.


\>writeln(povdifference(mesh,povunion([cl,ll]),povlook(green)));


Tuliskan dua titik potongnya.


\>writeln(povintersection([mesh,cl],povlook(red))); ...  
\>   writeln(povintersection([mesh,ll],povlook(gray)));


Tuliskan titik maksimumnya.


\>writeln(povpoint([1/2,1/2,1/4],povlook(gray),size=2\*defaultpointsize));


Tambahkan sumbu dan selesaikan.


\>writeAxes(0,1,0,1,0,1,d=0.015); ...  
\>   povend();


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-318.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-318.png)

# Anaglif dalam Povray

Untuk menghasilkan anaglif untuk kacamata merah/sian, Povray harus
dijalankan dua kali dari posisi kamera yang berbeda. Ia menghasilkan
dua file Povray dan dua file PNG, yang dimuat dengan fungsi
loadanaglyph().


Tentu saja, Anda memerlukan kacamata merah/sian untuk melihat contoh
berikut dengan benar.


Fungsi pov3d() memiliki sakelar sederhana untuk menghasilkan anaglif.


\>pov3d("-exp(-x^2-y^2)/2",r=2,height=45°,\>anaglyph, ...  
\>     center=[0,0,0.5],zoom=3.5);


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-319.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-319.png)

Jika Anda membuat suatu pemandangan dengan objek, Anda perlu
memasukkan pembuatan pemandangan tersebut ke dalam suatu fungsi, dan
menjalankannya dua kali dengan nilai yang berbeda untuk parameter
anaglyph.


\>function myscene ...


      s=povsphere(povc,1);
      cl=povcylinder(-povz,povz,0.5);
      clx=povobject(cl,rotate=xrotate(90°));
      cly=povobject(cl,rotate=yrotate(90°));
      c=povbox([-1,-1,0],1);
      un=povunion([cl,clx,cly,c]);
      obj=povdifference(s,un,povlook(red));
      writeln(obj);
      writeAxes();
    endfunction
</pre>
Fungsi povanaglyph() melakukan semua ini. Parameternya seperti pada
povstart() dan povend() yang digabungkan.


\>povanaglyph("myscene",zoom=4.5);


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-320.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-320.png)

# Menentukan Objek Sendiri

Antarmuka povray Euler berisi banyak objek. Namun, Anda tidak terbatas
pada objek-objek ini. Anda dapat membuat objek sendiri, yang
menggabungkan objek lain, atau objek yang sama sekali baru.


Kami mendemonstrasikan sebuah torus. Perintah Povray untuk ini adalah
"torus". Jadi, kami mengembalikan string dengan perintah ini dan
parameternya. Perhatikan bahwa torus selalu berpusat di titik asal.


\>function povdonat (r1,r2,look="") ...


      return "torus {"+r1+","+r2+look+"}";
    endfunction
</pre>
Inilah torus pertama kita.


\>t1=povdonat(0.8,0.2)


    torus {0.8,0.2}

Mari kita gunakan objek ini untuk membuat torus kedua, diterjemahkan
dan diputar.


\>t2=povobject(t1,rotate=xrotate(90°),translate=[0.8,0,0])


    object { torus {0.8,0.2}
     rotate 90 *x 
     translate &lt;0.8,0,0&gt;
     }

Sekarang kita tempatkan objek-objek ini ke dalam sebuah scene. Untuk
tampilannya, kita gunakan Phong Shading.


\>povstart(center=[0.4,0,0],angle=0°,zoom=3.8,aspect=1.5); ...  
\>   writeln(povobject(t1,povlook(green,phong=1))); ...  
\>   writeln(povobject(t2,povlook(green,phong=1))); ...  
\>  
&gt;povend();


memanggil program Povray. Namun, jika terjadi kesalahan, program
tersebut tidak menampilkan kesalahan tersebut. Oleh karena itu, Anda
harus menggunakan


&gt;povend(&lt;exit);


jika ada yang tidak berhasil. Ini akan membiarkan jendela Povray
terbuka.


\>povend(h=320,w=480);


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-321.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-321.png)

Berikut adalah contoh yang lebih rinci. Kami memecahkan


dan menunjukkan titik-titik yang layak dan titik-titik optimum dalam
plot 3D.


\>A=[10,8,4;5,6,8;6,3,2;9,5,6];

\>b=[10,10,10,10]';

\>c=[1,1,1];


Pertama, mari kita periksa, apakah contoh ini punya solusi.


\>x=simplex(A,b,c,\>max,\>check)'


    [0,  1,  0.5]

Ya, benar.


Berikutnya kita mendefinisikan dua objek. Yang pertama adalah bidang
datar


\>function oneplane (a,b,look="") ...


      return povplane(a,b,look)
    endfunction
</pre>
Kemudian kita mendefinisikan irisan semua ruang setengah dan sebuah
kubus.


\>function adm (A, b, r, look="") ...


      ol=[];
      loop 1 to rows(A); ol=ol|oneplane(A[#],b[#]); end;
      ol=ol|povbox([0,0,0],[r,r,r]);
      return povintersection(ol,look);
    endfunction
</pre>
Sekarang, kita dapat merencanakan adegannya.


\>povstart(angle=120°,center=[0.5,0.5,0.5],zoom=3.5); ...  
\>   writeln(adm(A,b,2,povlook(green,0.4))); ...  
\>   writeAxes(0,1.3,0,1.6,0,1.5); ...  
\>  
Berikut ini adalah lingkaran di sekitar titik optimum.


\>writeln(povintersection([povsphere(x,0.5),povplane(c,c.x')], ...  
\>     povlook(red,0.9)));


Dan kesalahan dalam arah yang optimum.


\>writeln(povarrow(x,c\*0.5,povlook(red)));


Kita menambahkan teks ke layar. Teks hanyalah objek 3D. Kita perlu
menempatkan dan memutarnya sesuai dengan pandangan kita.


\>writeln(povtext("Linear Problem",[0,0.2,1.3],size=0.05,rotate=5°)); ...  
\>   povend();


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-322.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-322.png)

# Contoh Lainnya

Anda dapat menemukan beberapa contoh lainnya untuk Povray di Euler
dalam berkas berikut.


Lihat: Contoh/Bola Dandelin


Lihat: Contoh/Donat Math


Lihat: Contoh/Simpul Trefoil


Lihat: Contoh/Optimasi dengan Penskalaan Afinitas


# Contoh dari Nadzwa

Nadzwa adalah seorang peneliti yang sedang mempelajari distribusi suhu
pada sebuah permukaan datar yang berbentuk persegi. Permukaan ini
memiliki koordinat x dari y yang berkisar dari -2 hingga 2 dengan
selisih 0.1 dan y sebagai transpose dari x. Nadzwa ingin
memvisualisasikan distribusi suhu ini berdasarkan fungsi matematika
yang menggambarkan variasi suhu pada setiap titik, yaitu


dimana z mewakili suhu di titik dengan koordinat (x,y).


Selanjutnya Nadzwa ingin melakukan modifikasi pada x dan y dengan
mengurangi masing-masing nilai sebesar 0.05.


\>x=-2:0.5:2; y=x'; z=x^2+y^2;...  
\>   xa=(x|2.1)-0.5; ya=(y\_2.1)-0.5;...  
\>   plot3d(xa,ya,z,bar=true):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-323.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-323.png)

# Kalkulus EMT

\> 


Materi Kalkulus mencakup di antaranya:


* 
Fungsi (fungsi aljabar, trigonometri, eksponensial,logaritma,
*   komposisi fungsi)

* 
Limit Fungsi,

* 
Turunan Fungsi,

* 
Integral Tak Tentu,

* 
Integral Tentu dan Aplikasinya,

* 
Barisan dan Deret (kekonvergenan barisan dan deret).
* EMT (bersama Maxima) dapat digunakan untuk melakukan semua perhitungan
* di dalam kalkulus, baik secara numerik maupun analitik (eksak).


# Mendefiniskan Fungsi

Terdapat beberapa cara mendefinisikan fungsi pada EMT, yakni:


- Menggunakan format nama_fungsi := rumus fungsi (untuk fungsi


  numerik),


- Menggunakan format nama_fungsi &amp;= rumus fungsi (untuk fungsi


  simbolik, namun dapat dihitung secara numerik),


- Menggunakan format nama_fungsi &amp;&amp;= rumus fungsi (untuk fungsi


  simbolik murni, tidak dapat dihitung langsung),


- Fungsi sebagai program EMT.


Setiap format harus diawali dengan perintah function (bukan sebagai
ekspresi).


Berikut adalah adalah beberapa contoh cara mendefinisikan fungsi.


# Definisi Fungsi Aljabar

fungsi matematika yang didefinisikan menggunakan operasi aljabar dasar
seperti penjumlahan, pengurangan, perkalian, pembagian, serta pangkat
rasional.


Misalkan kita punya fungsi aljabar:


cari f(0), f(2), f(3) dan buatkan grafik 2d


\>function f(x) := 2\*x+3 // fungsi numerik

\>f(0)


    3

\>f(2)


    7

\>f(3)


    9

\>plot2d("2\*x+3"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-324.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-324.png)

Berikutnya kita definisikan fungsi:


\>function g(x) := sqrt(x^2-3\*x)/(x+1) 

\>g(3)


    0

\>g(0)


    0

dapat dilihat bahwa x=0 dan x=3 membuat nilai g(x)=0, artinya x=0 dan
x=3 adalah akar-akar dari persamaan pada pembilang di fungsi g(x).


\>plot2d("sqrt(x^2-3\*x)/(x+1)"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-325.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-325.png)

## latihan Soal

Misalkan kita punya fungsi aljabar:


cari g(0), g(5) dan buatkan plot 2d


\>function g(x) := sqrt(x^2-5x)/(2x-3)

\>g(0), g(5)


    0
    0

\>plot2d("sqrt(x^2-5x)/(2x-3)"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-326.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-326.png)

\>&load(fourier\_elim)


    
            C:/Program Files/Euler x64/maxima/share/maxima/5.35.1/share/f\
    ourier_elim/fourier_elim.lisp
    

\>$&fourier\_elim([x^2-3\*x\>=0], [x])


$$\left[ x=0 \right] \lor \left[ x=3 \right] \lor \left[ 3<x \right] 
 \lor \left[ x<0 \right] $$\>g(1) // kompleks, tidak dapat dihitung oleh fungsi numerik


    Floating point error!
    Error in sqrt
    Try "trace errors" to inspect local variables after errors.
    g:
        useglobal; return sqrt(x^2-5x)/(2x-3) 
    Error in:
    g(1) // kompleks, tidak dapat dihitung oleh fungsi numerik ...
        ^

Nb: Floating point error karena untuk x=1, g(x)=g(1) akan bernilai
imajiner, yaitu


Silahkan Anda plot kurva fungsi di atas!


\>function g(x):= sqrt(x^2-3\*x)/(x+1);

\>plot2d("g(x)",-10,10,-10,10):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-328.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-328.png)

\>function g(x):= sqrt(x^2 - 4\*x + 3)/(x - 2);

\>plot2d("g(x)",-10,10,-10,10):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-329.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-329.png)

\>function g(x):= sqrt(2\*x^2 - 8\*x + 6)/(x - 2);

\>plot2d("g(x)", -1, 5, -10, 10):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-330.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-330.png)

## Latihan Soal



Silakan plot kurva fungsi di atas untuk semua x dalam interval [-1,5]


\>function g(x):= sqrt(3\*x^2 - 12\*x + 9)/(x - 2);

\>plot2d("g(x)", -1, 5, -10, 10):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-331.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-331.png)

# Fungsi Trigonometri

Fungsi trigonometri adalah suatu fungsi yang grafiknya berulang secara
terus menerus dalam periode tertentu. Fungsi trigonometri mempelajari
hubungan antara sudut-sudut dan sisi-sisi dalam segitiga.


Ada enam fungsi trigonometri dasar yang digunakan dalam Trigonometri.
Enam fungsi trigonometri dasar adalah fungsi sinus , fungsi kosinus ,
fungsi sekan, fungsi co-sekan, fungsi tangen , dan fungsi cotangen .
Sisi-sisi segitiga siku-siku adalah sisi tegak lurus, sisi miring, dan
alas, yang digunakan untuk menghitung nilai sinus, cosinus, tangen,
sekan , cosekan , dan kotangen menggunakan rumus trigonometri.


## Rumus Fungsi Trigonometri



Rumus-rumus dasar untuk mencari fungsi-fungsi trigonometri adalah
sebagai berikut:


Seperti yang dapat kita amati dari rumus-rumus yang diberikan di atas,
sinus dan cosekan merupakan kebalikan satu sama lain. Demikian pula,
pasangan kebalikannya adalah cosinus dan sekan, dan tangen dan
cotangen.


## Fungsi Trigonometri dalam Empat Kuadran



Fungsi-fungsi trigonometri ini memiliki tanda numerik yang berbeda (+
atau -) di kuadran yang berbeda, yang didasarkan pada sumbu positif
atau negatif kuadran. Fungsi trigonometri Sin dan Cosec positif di
kuadran I dan II, dan negatif di kuadran III dan IV. Fungsi
trigonometri Tan dan Cot positif hanya di Kuadran I dan III, dan rasio
trigonometri Cos dan Sec positif hanya di kuadran I dan IV.


## Grafik Fungsi Trigonometri

\>plot2d("sin(x)",-2\*pi,2\*pi,grid=1);

\>title("Plot\_Sin(x)");

\>xlabel("Sumbu x");

\>ylabel("Sumbu y"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-332.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-332.png)

\>plot2d("cos(x)",-2\*pi,2\*pi,grid=1);

\>title("Plot\_Cos(x)");

\>xlabel("Sumbu x");

\>ylabel("Sumbu y"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-333.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-333.png)

\>plot2d("tan(x)",-2pi,2pi,grid=1);

\>title("Plot\_Tan(x)");

\>xlabel("Sumbu x");

\>ylabel("Sumbu y"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-334.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-334.png)

## Identitas Fungsi Trigonometri

* 
Identitas Timbal Balik
*   cosec (x) =\frac {1}{sin (x)}
*   sec (x)=\frac{1}{cos (x)}
*   cot (x)=frac{1}{tan (x)}


* 
Identitas Pythagoras
*   sin^2 (x)+cos^2(x)=1
*   1+tan^2(x)=sec^2(x)
*   1+cot^2(x)=cosec^2(x)


-Identitas Jumlah dan Selisih


* 
Identitas Tiga Sudut
*   Sin 3x = 3sin (x) - 4sin(3x)
*   Cos 3x = 4cos(3x) - 3cos (x)
*   Tan 3x = \frac{3tan(x)-tan(3x)}{1-3tan(2x)}


* 
Identitas Produk
*   2sinx cosy = sin(x+y) + sin(x-y)
*   2cosx cosy=cos(x+y)+cos(x-y)
*   2sinx siny=cos(x-y)-cos(x+y)


* 
Jumlah Identitas
*   sin(x)+sin(y)=2sin(\frac{x+y}{2})  cos(\frac{x-y}{2})
*   sin(x)-sin(y)=2cos(\frac{x+y}{2})  sin(\frac{x-y}{2})
*   cos(x)+cos(y)=2cos(\frac{x+y}{2})  cos(\frac{x-y}{2})
*   cos(x)-cos(y)=-2sin(\frac{x+y}{2}  sin(\frac{x-y}{2})


## Contoh Soal

\>function f(x) := -2 cos 3(x)

\>plot2d("-2 \*cos (3\*x)",-2\*pi,2\*pi,grid=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-335.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-335.png)

\>function f(x) := -3 sin 2(x)

\>plot2d("-3 \*sin (2\*x)",-2\*pi,2\*pi,grid=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-336.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-336.png)

## Latihan Soal



1. Buatlah grafik f(x)= -4 sin 3(x)


2. f(x)=2 sin x, tentukan nilai f(0), f(1/2pi), f(4/3pi)


\>function f(x) := -4 sin 3(x)

\>plot2d("-4 \*sin (3\*x)",-2\*pi,2\*pi,grid=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-337.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-337.png)

\>function f(x) := 2\*sin(x)

\>f(0), f(1/2pi), f(4/3pi)


    0
    0.316967773183
    0.823572192941

# Fungsi Eksponensial

## Definisi Fungsi Eksponen



Secara umum, fungsi eksponen didefinisikan sebagai:


Untuk a&gt;0 dan x bilangan rill sembarang




dimana a adalah bilangan basis atau pokok


Untuk meyakinkan definisi tersebut, kita akan menggunakan


\>3^2, exp(2\*ln(3))


    9
    9

---



Latihan


---

\>2^5, exp(5\*ln(2))


    32
    32

---

## Sifat-Sifat Fungsi Eksponen



Apabila a&gt;0, b&gt;0, x dan y adalah bilangan rasional, maka


Bukti:


\>a:=2


    2

\>x:=3


    3

\>y:=4


    4

\>ri:=(a^x)^y // ruas paling kiri


    4096

\>ra:=a^(x\*y) // ruas paling kanan


    4096

\>exp1:=exp(y\*ln(a^x))


    4096

\>exp2:=exp(y\*x\*ln(a))


    4096

\>exp3:=exp(x\*y\*ln(a))


    4096

\>ri, ra, exp1, exp2, exp3


    4096
    4096
    4096
    4096
    4096

---



Latihan


---

\>a:=3


    3

\>x:=2


    2

\>y:=3


    3

\>ri:=(a^x)^y


    729

\>ra:=a^(x\*y)


    729

\>exp1:=exp(y\*ln(a^x))


    729

\>exp2:=exp(y\*x\*ln(a))


    729

\>exp3:=exp(x\*y\*ln(a))


    729

\>ri, ra, exp1, exp2, exp3


    729
    729
    729
    729
    729

## Grafik Fungsi Eksponen



Bentuk umum dari grafik fungsi eksponen:




dimana k adalah konstanta dan a adalah basis atau bilangan pokok.


Syarat dari basis adalah




Grafik fungsi eksponen akan selalu simteri terhadap sumbu-y. Selain
itu, grafik fungsi eksponen ini selalu memotong sumbu-y di titik
(0,k).


Grafik fungsi eksponen ini memiliki 2 jenis:


1. Grafik fungsi Monoton Naik




2. Grafik fungsi Monoton Turun


---



Contoh Grafik Monoton Naik


---

\>x=[-3,-2,-1,0,1,2,3]; y=2^x; plot2d(x,y,"0-"); xlabel("X"); ...  
\>   ylabel("Y"); title("Grafik Eksponensial y=2^x"); ...  
\>   grid:=true:


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-338.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-338.png)

---



Contoh Grafik Monoton Turun


---

\>x=[-3,-2,-1,0,1,2,3]; y=(1/2)^x; plot2d(x,y,"0-",color(green)); xlabel("X"); ...  
\>   ylabel("Y"); title("Grafik Eksponensial y=(1/2)^x"); ...  
\>   grid:=true:


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-339.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-339.png)

---



Latihan


---



x=[-4,-2,0,2,4]


\>x=[-4,-2,0,2,4]; y=3^(-x)+1; plot2d(x,y,"0-",color(green)); xlabel("X"); ...  
\>   ylabel("Y"); title("Grafik Eksponensial y=3^(-x)+1"); ...  
\>   grid:=true:


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-340.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-340.png)

---

# Fungsi Logaritma

## Definisi Logaritma



atau




dengan




serta a disebut basis dan x disebut numerus.


---

## Definisi Fungsi Logaritma



dengan




serta a disebut basis dan x disebut numerus.


---

## Sifat-Sifat Logaritma

Jika a&gt;1 dan


Jika 0&lt;1 dan


---

## Sifat Grafik Fungsi Logaritma



Tidak memotong sumbu y


Memotong sumbu x di titik (1,0)


Jika 0&lt;a&lt;1 maka grafik fungsi turun dan




maka


Jika a&gt;1 maka grafik fungsi naik dan




maka


---



Latihan Membuat Grafik Logaritma


---

\>function k(x) := logbase(x, 7)

\>k(49)


    2

\>plot2d("k(x)"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-341.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-341.png)

## Komposisi Fungsi

Komposisi fungsi adalah susunan beberapa fungsi yang berkaitan dan
terhubung. Bahasa paling mudah untuk mendeskripsikan komposisi fungsi
ini adalah "fungsi di dalam fungsi". Sebagai contoh, jika




dan




maka


\>function f(x):= x^3+1

\>function g(x):= x^2+x;

\>f(g(5)) // komposisi fungsi


    27001

\>g(f(5))


    16002

\>function h(x) := f(g(x)) // definisi komposisi fungsi

\>h(5) // sama dengan f(g(5))


    27001

\>function u(x) := g(f(x))


Silakan Anda plot kurva fungsi komposisi fungsi f dan g:


dan


bersama-sama kurva fungsi f dan g dalam satu bidang koordinat.


\>plot2d(["h(x)", "u(x)"], -10,10,0,10):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-342.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-342.png)

\>f(0:10) // nilai-nilai f(0), f(1), f(2), ..., f(10)


    [1,  2,  9,  28,  65,  126,  217,  344,  513,  730,  1001]

\>fmap(0:10) // sama dengan f(0:10), berlaku untuk semua fungsi


    [1,  2,  9,  28,  65,  126,  217,  344,  513,  730,  1001]

\>gmap(200:210)


    [40200,  40602,  41006,  41412,  41820,  42230,  42642,  43056,  43472,
    43890,  44310]

Misalkan kita akan mendefinisikan fungsi


Fungsi tersebut tidak dapat didefinisikan sebagai fungsi numerik
secara "inline" menggunakan format :=, melainkan didefinisikan sebagai
program. Perhatikan, kata "map" digunakan agar fungsi dapat menerima
vektor sebagai input, dan hasilnya berupa vektor. Jika tanpa kata
"map" fungsinya hanya dapat menerima input satu nilai.


\>function map f(x)


    endfunction
</pre>
\>f(1)

\>f(-2)

\>f(-5:5)

\>aspect(1.5); plot2d("f(x)",-5,5):


    A function returned no value. Cannot assign this to a variable.
    %ploteval:
        y0=f$(x[1],args());
    adaptiveevalone:
        s=%ploteval(g$,t;args());
    Try "trace errors" to inspect local variables after errors.
    plot2d:
        dw/n,dw/n^2,dw/n,auto;args());

\>function f(x) &= 2\*E^x // fungsi simbolik


    
                                        x
                                     2 E
    

\>$f(a) // nilai fungsi secara simbolik


$$2\,e^{a}$$\>f(E) // nilai fungsi berupa bilangan desimal


    30.308524483

\>$f(E), $float(%)


$$2\,e^{e}$$$$30.30852448295852$$\>function g(x) &= 3\*x+1


    
                                   3 x + 1
    

\>function h(x) &= f(g(x)) // komposisi fungsi


    
                                     3 x + 1
                                  2 E
    

\>plot2d("h(x)",-1,1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-346.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-346.png)

# Latihan

Bukalah buku Kalkulus. Cari dan pilih beberapa (paling sedikit 5
fungsi berbeda tipe/bentuk/jenis) fungsi dari buku tersebut, kemudian
definisikan di EMT pada baris-baris perintah berikut (jika perlu
tambahkan lagi). Untuk setiap fungsi, hitung beberapa nilainya, baik
untuk satu nilai maupun vektor. Gambar grafik tersebut.


Juga, carilah fungsi beberapa (dua) variabel. Lakukan hal sama seperti
di atas.


1. Diberikan sebuah fungsi




tentukan nilai


a. a(-2)


b. a(-12)


\>function a(x) := x^2+x+11

\>a(-2), a(-12)


    13
    143

\>plot2d("a",-10,10):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-347.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-347.png)

2. Diberikan sebuah fungsi




hitunglah masing-masing nilai b(4) dan b(44)


\>function b(x) := (x^2+36)/(x-6)

\>b(4), b(44)


    -26
    51.8947368421

\>plot2d("b",-100,100,-100,100):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-348.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-348.png)

3. Diberikan sebuah fungsi




tentukan nilai p(4), p(-4), p(10)


\>function p(x) := x^3-12\*x^2+48\*x-64

\>p(4), p(-4), p(10)


    0
    -512
    216

\>plot2d("p",-1,8):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-349.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-349.png)

4. Tentukan nilai f(41) dari fungsi berikut


\>function f(x) := sqrt(x^2-81)

\>f(41)


    40

\>plot2d("f",-50,50):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-350.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-350.png)

5. Untuk fungsi




tentukan nilai (f o g)(0) dan (g o f)(10)


\>function f(x) := x^2-5\*x+6; $f(x)

\>function g(x) := x+7; $g(x)

\>f(g(-2)), g(f(0))


    6
    13

\>plot2d("f(g(x))",-5,5):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-351.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-351.png)

\>plot2d("g(f(x))",-5,5):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-352.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-352.png)

# Limit

Untuk sebuah fungsi f(x), dikatakan bahwa limit


(x) mendekati L saat x mendekati, ditulis sebagai:


Perhitungan limit pada EMT dapat dilakukan dengan menggunakan fungsi
Maxima, yakni "limit". Fungsi "limit" dapat digunakan untuk menghitung
limit fungsi dalam bentuk ekspresi maupun fungsi yang sudah
didefinisikan sebelumnya. Nilai limit dapat dihitung pada sebarang
nilai atau pada tak hingga (-inf, minf, dan inf).


Perhatikan!!!


\>$limit(sqrt(x^2-3\*x)/(x+1),x,inf)


$$1$$\>$showev('limit(sqrt(x^2-3\*x)/(x+1),x,inf))


$$\lim_{x\rightarrow \infty }{\frac{\sqrt{x^2-3\,x}}{x+1}}=1$$\>$showev('limit((3\*x+5)/(2\*x-4),x,minf))


$$\lim_{x\rightarrow  -\infty }{\frac{3\,x+5}{2\,x-4}}=\frac{3}{2}$$\>$showev('limit(1/(2\*x-1),x,0))


$$\lim_{x\rightarrow 0}{\frac{1}{2\,x-1}}=-1$$## Latihan soal

Contoh soal, hitung nilai limitnya


\>$showev('limit(1/(2\*x-1),x,0))


$$\lim_{x\rightarrow 0}{\frac{1}{2\,x-1}}=-1$$\>$showev('limit((4\*x+7)/(x-1),x,inf))


$$\lim_{x\rightarrow \infty }{\frac{4\,x+7}{x-1}}=4$$## limit kiri dan kanan

Limit Kiri :


menggunakan opsi "minus"


Limit Kanan :


menggunakan opsi "plus"


Jika,


maka,


contoh:


\>$showev('limit(abs(x-1)/(x-1),x,1,minus))


$$\lim_{x\uparrow 1}{\frac{\left| x-1\right| }{x-1}}=-1$$\>$showev('limit(abs(x-1)/(x-1),x,1,plus)) 


$$\lim_{x\downarrow 1}{\frac{\left| x-1\right| }{x-1}}=1$$karena limit dari kiri dan limit dari kirinya berbeda maka nilai limit
di x=1 tidak ada


## Latihan soal

1.


2.


hitunglah limit kanan dan kirinya dan berikan kesimpulan


\>$showev('limit(1/(x),x,0,minus))


$$\lim_{x\uparrow 0}{\frac{1}{x}}= -\infty $$\>$showev('limit(1/(x),x,0,plus))


$$\lim_{x\downarrow 0}{\frac{1}{x}}=\infty $$\>$showev('limit((x^2-4)/(x-4),x,2,minus))


$$\lim_{x\uparrow 2}{\frac{x^2-4}{x-4}}=0$$\>$showev('limit((x^2-4)/(x-4),x,2,plus))


$$\lim_{x\downarrow 2}{\frac{x^2-4}{x-4}}=0$$\>plot2d("(x^2-4)/(x-4)"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-365.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-365.png)

# Limit

limit dalam fungsi aljabar


hitunglah limit dari kanan, limit dari kiri, dan x mendekati 5


menggunakan perintah $showev dan jika dari kiri menggunakan opsi
"minus" dan jika dari kanan menggunakan opsi "plus"


\>$showev('limit((2\*x-8),x,5,minus))


$$\lim_{x\uparrow 5}{2\,x-8}=2$$\>$showev('limit((2\*x-8),x,5,plus))


$$\lim_{x\downarrow 5}{2\,x-8}=2$$\>$showev('limit((2\*x-8),x,5))


$$\lim_{x\rightarrow 5}{2\,x-8}=2$$\>$showev('limit((x^2/x),x,0,plus))


$$\lim_{x\downarrow 0}{x}=0$$\>$showev('limit((x^2/x),x,0,minus))


$$\lim_{x\uparrow 0}{x}=0$$# Limit dalam berbagai fungsi

Limit dalam fungsi aljabar


hitunglah nilai limit dari fungsi aljabar tersebut


\>$showev('limit((sqrt(x)-2)/(x-4),x,4))


$$\lim_{x\rightarrow 4}{\frac{\sqrt{x}-2}{x-4}}=\frac{1}{4}$$Latihan:


hitunglah nilai dari limit fungsi berikut


\>$showev('limit((sqrt(1-2\*x))/((3\*x+2)^3),x,-2))


$$\lim_{x\rightarrow -2}{\frac{\sqrt{1-2\,x}}{\left(3\,x+2\right)^3}}=
 -\frac{\sqrt{5}}{64}$$\>plot2d("(sqrt(1-2\*x))/((3\*x+2)^3)"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-373.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-373.png)

Limit dalam fungsi trigonometri


hitunglah nilai limit dari fungsi trigonometri tersebut


\>$showev('limit((sin(2\*x))/(x),x,0))


$$\lim_{x\rightarrow 0}{\frac{\sin \left(2\,x\right)}{x}}=2$$Latihan;


hitunglah nilai limit dari fungsi tersebut


\>$showev('limit((sin(x)),x,(pi/2)))


$$\lim_{x\rightarrow \frac{\pi}{2}}{\sin x}=1$$\>plot2d("(sin(x))"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-376.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-376.png)

\>$showev('limit(((1-(cos(5\*x)))/(x^2)),x,0))


$$\lim_{x\rightarrow 0}{\frac{1-\cos \left(5\,x\right)}{x^2}}=\frac{
 25}{2}$$\>plot2d("(1-(cos(5\*x)))/(x^2)"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-378.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-378.png)

Limit fungsi trigonometri




hitunglah nilai limit trigonometri tersebut


\>$showev('limit((log(x)/x^2),x,(pi/2)))


$$\lim_{x\rightarrow \frac{\pi}{2}}{\frac{\log x}{x^2}}=\frac{4\,
 \log \left(\frac{\pi}{2}\right)}{\pi^2}$$Latihan:


Hitunglah nilai limit dari fungsi berikut


baris tak tentu


\>$showev('limit(log(x)/(x-1),x,1))


$$\lim_{x\rightarrow 1}{\frac{\log x}{x-1}}=1$$\>plot2d("(log(x)/(x-1))"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-381.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-381.png)

# Turunan Fungsi

Definisi turunan:


Berikut adalah contoh-contoh menentukan turunan fungsi dengan
menggunakan definisi turunan (limit).


\>$showev('limit(((x+h)^2-x^2)/h,h,0)) // turunan x^2


$$\lim_{h\rightarrow 0}{\frac{\left(x+h\right)^2-x^2}{h}}=2\,x$$\>p &= expand((x+h)^2-x^2)|simplify; $p //pembilang dijabarkan dan disederhanakan


$$2\,h\,x+h^2$$\>q &=ratsimp(p/h); $q // ekspresi yang akan dihitung limitnya disederhanakan


$$2\,x+h$$\>$limit(q,h,0) // nilai limit sebagai turunan


$$2\,x$$\>$showev('limit(((x+h)^n-x^n)/h,h,0)) // turunan x^n


$$\lim_{h\rightarrow 0}{\frac{\left(x+h\right)^{n}-x^{n}}{h}}=n\,x^{n
 -1}$$Petunjuk: ekspansikan (x+h)^n dengan menggunakan teorema binomial.


\>$showev('limit((sin(x+h)-sin(x))/h,h,0)) // turunan sin(x)


$$\lim_{h\rightarrow 0}{\frac{\sin \left(x+h\right)-\sin x}{h}}=\cos 
 x$$Petunjuk: ekspansikan sin(x+h) dengan menggunakan rumus jumlah dua
sudut.


# Latihan

\>function f(x) := x^2

\>$showev('limit((((x+h)^2-x^2)/h),h,0)) // turunan x^2


$$\lim_{h\rightarrow 0}{\frac{\left(x+h\right)^2-x^2}{h}}=2\,x$$\>function df(x) &= limit((((x+h)^2-x^2)/h),h,0);  $df(x)// df(x) = f'(x)


$$2\,x$$\>plot2d(["f(x)","df(x)"],-pi,pi,color=[blue,red]), label("f(x)",2,0.6), label("df(x)",2,0.17):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-390.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-390.png)

2. 


\>function f(x) := x^2+3\*x

\>$showev('limit(((x+h)^2+3\*(x+h)-(x^2+3\*x))/h,h,0)) // turunan x^2+3\*x


$$\lim_{h\rightarrow 0}{\frac{\left(x+h\right)^2-x^2+3\,\left(x+h
 \right)-3\,x}{h}}=2\,x+3$$\>function df(x) &= limit(((x+h)^2+3\*(x+h)-(x^2+3\*x))/h,h,0);  $df(x)// df(x) = f'(x)


$$2\,x+3$$\>plot2d(["f(x)","df(x)"],-pi,pi,color=[blue,red]), label("f(x)",2,0.4), label("df(x)",1,-0.5):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-393.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-393.png)

\>function f(x) := log(x)

\>$showev('limit((log(x+h)-log(x))/h,h,0)) // turunan log(x)


$$\lim_{h\rightarrow 0}{\frac{\log \left(x+h\right)-\log x}{h}}=
 \frac{1}{x}$$\>function df(x) &= limit(((log(x+h)-log(x))/h) ,h,0);  $df(x)// df(x) = f'(x)


$$\frac{1}{x}$$\>plot2d(["f(x)","df(x)"],-pi,pi,color=[blue,red]), label("f(x)",2,0.6), label("df(x)",2,0.17):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-396.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-396.png)

## Turunan Eksponensial

\>function f(x) := E^x

\>$showev('limit(factor((E^(x+h)-E^x)/h),h,0)) // turunan f(x)=e^x


$$\left(\lim_{h\rightarrow 0}{\frac{e^{h}-1}{h}}\right)\,e^{x}=e^{x}$$Menggunakan factor atau pemfactoran pada




dikarenakan untuk menyederhanakan limit, sehingga kita bisa memisahkan
komponen yang bergantung pada h dan yang tidak bergantung pada h.


karena turunan dari




adalah




maka,


\>function df(x) &= E^x


    
                                       x
                                      E
    

\>plot2d(["f(x)","df(x)"],-pi,pi,color=[blue,red]), label("f(x)",2,0.3), label("df(x)",1,-0.5):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-398.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-398.png)

\>function f(x) &= x^x


    
                                       x
                                      x
    

\>$showev('limit(f(x),x,0))


$$\lim_{x\rightarrow 0}{x^{x}}=1$$\>plot2d("x^x"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-400.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-400.png)

\>$showev('limit((f(x+h)-f(x))/h,h,0)) // turunan f(x)=x^x


$$\lim_{h\rightarrow 0}{\frac{\left(x+h\right)^{x+h}-x^{x}}{h}}=
 {\it infinity}$$Dapat dilihat bahwa dari yang kita cari pertama nilai limit dari


itu ada yaitu 1.


Sementara pada yang kita cari menggunakan definisi turunan nilai
limitnya infinity.


Begitu juga pada grafik, nilai dari x hanya terdefinisi di zona
positif, jadi untuk mencari turunannya perlu diasumsikan dulu bahwa
nilai x nya itu berjalan dengan x yang positif karena nilai dari yang
negatifnya tidak terdefinisi.


\>&assume(x\>0); $showev('limit((f(x+h)-f(x))/h,h,0)) // turunan f(x)=x^x


$$\lim_{h\rightarrow 0}{\frac{\left(x+h\right)^{x+h}-x^{x}}{h}}=x^{x}
 \,\left(\log x+1\right)$$\>&forget(x\>0) // jangan lupa, lupakan asumsi untuk kembali ke semula


    
                                   [x &gt; 0]
    

\>&forget(x<0)


    
                                   [x &lt; 0]
    

\>&facts()


    
            [kind(sinh, one_to_one), kind(log, one_to_one), 
                            kind(tanh, one_to_one), kind(log, increasing)]
    

# Latihan

\>function f(x) &= E^(3\*x)+4\*x\*E^x


    
                                 3 x        x
                                E    + 4 x E
    

\>$showev('limit(factor((E^(3\*x+h)+4\*(x+h)\*E^(x+h)-E^(3\*x)-4\*x\*E^x)/h),h,0))


$$e^{x}\,\left(\lim_{h\rightarrow 0}{\frac{e^{2\,x+h}-e^{2\,x}+4\,e^{
 h}\,x-4\,x+4\,h\,e^{h}}{h}}\right)=e^{x}\,\left(e^{2\,x}+4\,x+4
 \right)$$\>function df(x) &= E^x\*(E^(2\*x)+4\*x+4)


    
                              x   2 x
                             E  (E    + 4 x + 4)
    

\>plot2d(["f(x)","df(x)"],-pi,pi,color=[blue,red]), label("f(x)",2,0.6), label("df(x)",1,-0.5):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-404.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-404.png)

2. 


\>function f(x) &= log(3\*x+1)


    
                                 log(3 x + 1)
    

\>$showev('limit((log(3\*x+h+1)-log(3\*x+1))/h,h,0))


$$\lim_{h\rightarrow 0}{\frac{\log \left(3\,x+h+1\right)-\log \left(3
 \,x+1\right)}{h}}=\frac{1}{3\,x+1}$$\>function df(x) &= limit(((log(3\*x+h+1)-log(3\*x+1))/h) ,h,0);  $df(x)// df(x) = f'(x)


$$\frac{1}{3\,x+1}$$\>plot2d(["f(x)","df(x)"],-pi,pi,color=[blue,red]), label("f(x)",2,0.6), label("df(x)",1,-0.2):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-407.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-407.png)

\>$showev('limit((asin(x+h)-asin(x))/h,h,0)) // turunan arcsin(x)


$$\lim_{h\rightarrow 0}{\frac{\arcsin \left(x+h\right)-\arcsin x}{h}}=
 \frac{1}{\sqrt{1-x^2}}$$Mengapa hasilnya seperti itu? Tuliskan atau tunjukkan bahwa hasil
limit tersebut benar, sehingga benar turunan fungsinya benar. Tulis
penjelasan Anda di komentar ini.


\>$showev('limit((tan(x+h)-tan(x))/h,h,0)) // turunan tan(x)


$$\lim_{h\rightarrow 0}{\frac{\tan \left(x+h\right)-\tan x}{h}}=
 \frac{1}{\cos ^2x}$$Mengapa hasilnya seperti itu? Tuliskan atau tunjukkan bahwa hasil
limit tersebut benar, sehingga benar turunan fungsinya benar. Tulis
penjelasan Anda di komentar ini.


Jadi, terbukti benar bahwa


\>function f(x) &= sinh(x) // definisikan f(x)=sinh(x)


    
                                   sinh(x)
    

\>function df(x) &= limit((f(x+h)-f(x))/h,h,0); $df(x) // df(x) = f'(x)


$$\frac{e^ {- x }\,\left(e^{2\,x}+1\right)}{2}$$Hasilnya adalah cosh(x), karena


\>plot2d(["f(x)","df(x)"],-pi,pi,color=[blue,red]):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-411.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-411.png)

\>function f(x) &= sin(3\*x^5+7)^2


    
                                   2    5
                                sin (3 x  + 7)
    

\>diff(f,3), diffc(f,3)


    1198.32948904
    1198.72863721

Apakah perbedaan diff dan diffc?


diff untuk menghitung turunan numerik ke-n dari fungsi f menggunakan
metode perbedaan terbatas (finite difference). Sedangkan diffc mungkin
merujuk pada metode yang lebih canggih atau terkompensasi untuk
menghitung turunan numerik ke-n dari fungsi f.


\>$showev('diff(f(x),x))


$$\frac{d}{d\,x}\,\sin ^2\left(3\,x^5+7\right)=30\,x^4\,\cos \left(3
 \,x^5+7\right)\,\sin \left(3\,x^5+7\right)$$\>$% with x=3


$${\it \%at}\left(\frac{d}{d\,x}\,\sin ^2\left(3\,x^5+7\right) , x=3
 \right)=2430\,\cos 736\,\sin 736$$\>$float(%)


$${\it \%at}\left(\frac{d^{1.0}}{d\,x^{1.0}}\,\sin ^2\left(3.0\,x^5+
 7.0\right) , x=3.0\right)=1198.728637211748$$\>plot2d(f,0,3.1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-415.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-415.png)

\>function f(x) &=5\*cos(2\*x)-2\*x\*sin(2\*x) // mendifinisikan fungsi f


    
                          5 cos(2 x) - 2 x sin(2 x)
    

\>function df(x) &=diff(f(x),x) // fd(x) = f'(x)


    
                         - 12 sin(2 x) - 4 x cos(2 x)
    

\>$'f(1)=f(1), $float(f(1)), $'f(2)=f(2), $float(f(2)) // nilai f(1) dan f(2)


$$f\left(1\right)=5\,\cos 2-2\,\sin 2$$$$-3.899329036387075$$$$f\left(2\right)=5\,\cos 4-4\,\sin 4$$$$-0.2410081230863468$$\>xp=solve("df(x)",1,2,0) // solusi f'(x)=0 pada interval [1, 2]


    1.35822987384

\>df(xp), f(xp) // cek bahwa f'(xp)=0 dan nilai ekstrim di titik tersebut


    0
    -5.67530133759

\>plot2d(["f(x)","df(x)"],0,2\*pi,color=[blue,red]): //grafik fungsi dan turunannya


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-420.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-420.png)

Perhatikan titik-titik "puncak" grafik y=f(x) dan nilai turunan pada
saat grafik fungsinya mencapai titik "puncak" tersebut.


# Integral

## Integral Tak Tentu

## DEFINISI

 Integral Tak Tentu (undefinite integral) adalah bentuk integral yang  

tidak memiliki batas tertentu, sehingga hasilnya adalah fungsi umum
yang disertai konstanta integrasi (C). Integral tak tentu merupakan
kebalikan dari turunan, sehingga disebut antiturunan atau
antiderivatif.


 Integral tak tentu dari suatu fungsi f(x) adalah fungsi F(x) yang  

mempunyai turunan f(x), maka integral tak tentu merupakan himpunan
anti turunan F(x) dari f(x) pada interval negatif tak hingga sampai
tak hingga yang dinotasikan :


dimana F'(x)=f(x) dan C adalah konstanta integrasi


---

## KURVA FUNGSI ANTIDERIVATIF

 Kurva fungsi antiderivatif adalah kurva yang menggambarkan semua  

fungsi yang memiliki turunan sama. Setiap fungsi antiderivatif dari
suatu fngsi f(x) berbeda hanya dalam konstanta integrasi (C)


 1. kurva antiderivatif dari fungsi aljabar dengan  

\>$showev('integrate(3\*x^2,x)+c)


$$3\,\int {x^2}{\;dx}+c=x^3+c$$\>plot2d(["3\*x^2","x^3","x^3+1","x^3+2","x^3+3"]):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-422.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-422.png)

2. kurva antiderivatif dari fungsi trigonometri dengan


\>$showev('integrate(sin(x),x)+c)


$$\int {\sin x}{\;dx}+c=c-\cos x$$\>plot2d(["-cos(x)","-cos(x)+1","-cos(x)+2","-cos(x)+3","-cos(x)+4"]):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-424.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-424.png)

 3. kurva antiderivatif dari fungsi eksponensial dengan  

\>$showev('integrate(x\*E^x,x)+c)


$$\int {x\,e^{x}}{\;dx}+c=\left(x-1\right)\,e^{x}+c$$\>plot2d(["x\*E^x","(x-1)E^x+1","(x-1)E^x+2","(x-1)E^x+3","(x-1)E^x+4"]):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-426.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-426.png)

4. kurva antiderivatif dari fungsi logaritma dengan


\>$showev('integrate(log(8\*x),x)+c)


$$\int {\log \left(8\,x\right)}{\;dx}+c=\frac{8\,x\,\log \left(8\,x
 \right)-8\,x}{8}+c$$\>plot2d(["log(8\*x)","(8\*x)log(8\*x)-8\*x/8 +1","(8\*x)log(8\*x)-8\*x/8 +2","(8\*x)log(8\*x)-8\*x/8 +3"]):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-428.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-428.png)

5. kurva antiderivatif dari fungsi komposisi dengan




dengan


\>function f(x) &&= x+2


    
                                    x + 2
    

\>function g(x) &&= 2\*x-1


    
                                   2 x - 1
    

\>$showev('integrate(f(g(x)),x)+c)


$$\int {2\,x+1}{\;dx}+c=x^2+x+c$$\>plot2d(["2\*x+1","x^2+x+1","x^2+x+2","x^2+x+3","x^2+x+4"]):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-430.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-430.png)

---

## SIFAT-SIFAT INTEGRAL TAK TENTU

Integral tak tentu adalah LINEAR. Perlu diingat pada Aturan Kelipatan
Konstanta, bahwa




adalah suatu operator linear. Ini berarti dua hal.


Dari dua sifat ini, sifat ketiga mengikuti secara otomatis.


Apa yang benar untuk anti turunan adalah benar juga untuk integral tak
tentu (anti-turunan).


(Kelinearan dari




Andaikan f dan k mempunyai anti turunan (integral tak tentu) dan
andaikan k suatu konstanta, maka:


\>   


Bukti: Untuk memperlihatkan sifat (i) dan (ii), kita cukup
mendiferensikan ruas kanan dan amati bahwa kita akan memperolah
integran dari ruas kiri.


---



Contoh Soal


---

\>$showev('integrate(3\*x^2,x)+c)


$$3\,\int {x^2}{\;dx}+c=x^3+c$$\>$showev('integrate(4\*x,x)+c)


$$4\,\int {x}{\;dx}+c=2\,x^2+c$$\>$showev('integrate(3\*x^2+4\*x,x)+c)


$$\int {3\,x^2+4\,x}{\;dx}+c=x^3+2\,x^2+c$$Apabila perhitungan secara manual:


image: contoh1.jpg


---



Latihan


---

\>$showev('integrate(3\*sin(t),t)+c)


$$3\,\int {\sin t}{\;dt}+c=c-3\,\cos t$$\>$showev('integrate(-2\*cos(t),t)+c)


$$c-2\,\int {\cos t}{\;dt}=c-2\,\sin t$$\>$showev('integrate(3\*sin(t)-2\*cos(t),t)+c)


$$\int {3\,\sin t-2\,\cos t}{\;dt}+c=-2\,\sin t-3\,\cos t+c$$---

## RUMUS-RUMUS INTEGRAL TAK TENTU



dimana a adalah konstanta dan C juga merupakan konstanta.




dimana a adalah konstanta dan C juga merupakan konstanta.


---



Contoh Soal


---

\>$showev('integrate(1/(1+x^2),x)+c)


$$\int {\frac{1}{x^2+1}}{\;dx}+c=\arctan x+c$$Mengapa arctan(x)+c?


Jadi, antara




dengan arctan(x) ini saling berhubungan dengan definisi invers
trigonometri.


Fungsi arctan(x) adalah fungsi invers dari tan(x). Secara matematis,
turunan dari arctan(x) adalah:




Ini berarti bahwa arctan(x) adalah fungsi yang jika diturunkan
menghasilkan




Oleh karena itu, ketika kita melakukan integral terhadap




kita mendapatkan kebalikan dari turunan tersebut, yaitu fungsi
arctan(x).


# Integral tentu

Integral tentu adalah integral yang memiliki batasan atas dan bawah
yang jelas, sehingga menghasilkan sebuah nilai. Batasan dari integral
tentu adalah a sampai b atau batas atas sampai batas bawah.


Integral tentu dapat dihitung dengan menggunakan Teorema Dasar
Kalkulus


Misalnya mencari hasil dari fungsi integral:


dengan menggunakan rumus kita peroleh:


\>$showev('integrate(6\*x+2,x,2,3))


$$\int_{2}^{3}{6\,x+2\;dx}=17$$## Latihan:

a.




b.


Integral dapat diselesaikan dengan EMT yaitu dengan fungsi
"integrate". EMT juga dapat digunakan untuk menghitung integral tentu
dengan beberapa fungsi yang mengimplementasikan algoritma
kuadratur(perhitungan integral tentu menggunakan metode numerik).


Fungsi "showev" digunakan untuk menampilkan atau melihat hasil
perhitungan. Setelah fungsi integrate, diikuti fungsi, terhadap
variabel apa, batas bawah, dan batas atas.


\>$showev('integrate(x^2-4\*x+3,x,0,1))


$$\int_{0}^{1}{x^2-4\,x+3\;dx}=\frac{4}{3}$$\>$showev('integrate(1+cos(t),t,2,6))


$$\int_{2}^{6}{\cos t+1\;dt}=\sin 6-\sin 2+4$$* 
fx &amp;=: Ini adalah operasi penugasan gabungan. Artinya, hasil dari
* perhitungan di sebelah kanan akan ditambahkan ke variabel fx. Jika fx
* belum didefinisikan sebelumnya, maka fx akan dibuat sebagai sebuah
* list.
* -makelist(...,i,1,length(t)): Fungsi ini digunakan untuk membuat
* sebuah list.


Parameter-parameternya adalah:


- f(t[i]+0.1): Ini adalah ekspresi yang akan dihitung untuk setiap
nilai i. Fungsi f akan dievaluasi pada nilai t[i] ditambah 0.1.


- i: Adalah indeks yang akan digunakan untuk mengakses elemen-elemen
dalam list t.


- 1: Adalah nilai awal untuk indeks i.


- length(t): Adalah nilai akhir untuk indeks i, yaitu panjang dari
list t.


\>function map f(x) &= E^(-x^2)


    
                                        2
                                     - x
                                    E
    

\>$showev('integrate(f(x),x))


$$\int {e^ {- x^2 }}{\;dx}=\frac{\sqrt{\pi}\,\mathrm{erf}\left(x
 \right)}{2}$$Fungsi f diatas tidak memiliki antiturunan yang dapat diungkapkan
dalam bentuk tertutup, sehingga kita tidak dapat menghitungnya dengan
Teorema Dasar Kalkulus. KIta dapat menghitung integral tentu fungsi
tersebut dengan menggunakan metode numerik(rumus kuadratur).


\>x=0:0.1:pi-0.1; plot2d(x,f(x+0.1),\>bar); plot2d("f(x)",0,pi,\>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-442.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-442.png)

Integral tentu erat kaitannya dengan luas daerah dibawah kurva,
sehingga menghitung fungsi diatas dapat dihampiri dengan jumlah luas
persegi panjang-persegi panjang di bawah kurva tersebut. Cara
menghitungnya adalah dengan langkah-langkah sebagai berikut:


Langkah pertama, yaitu kita dapat menyimpan nilai-nilai x ke dalam
variabel misalkan t.


\>t &= makelist(a,a,0,pi-0.1,0.1);


Selanjutnya kita dapat menyimpan nilai dari masing-masing f(x).


\>fx &= makelist(f(t[i]+0.1),i,1,length(t));

\>0.1\*sum(f(x+0.1))


    0.836219610253

jadi hasilnya adalah:


maxima: 'integrate(f(x),x,0,pi) = 0.1*sum(fx[i],i,1,length(fx))


Jumlah tersebut diperoleh dari hasil kali lebar sub-subinterval (=0.1)
dan jumlah nilai-nilai f(x) untuk x = 0.1, 0.2, 0.3, ..., 3.2.


Jika kita memperbanyak jumlah persegi panjang dibawah kurva, maka
lebar sub-intervalnya akan semakin kecil dan persegi panjangnya akan
menutup daerah dibawah kurva dengan sempurna.Untuk mendapatkan hasil
yang mendekati nilai sebenarnya kita dapat gunakan misalnya lebar
sub-interval misalnya 0.01, atau jika ingin lebih presisi lagi bisa
0.001 dan seterusnya. Kita akan mencoba menghitung integral fungsi
diatas dengan dengan t yang diperkecil lagi menjadi 0.01.


\>x=0:0.01:pi-0.01; plot2d(x,f(x+0.01),\>bar); plot2d("f(x)",0,pi,\>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-443.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-443.png)

Gambar diatas jika dibandingkan dengan gambar sebelumnya, terlihat
perbedannya dimana jika gambar pertama daerah dibawah kurva masih
belum tertutup sempurna, tetapi pada gambar diatas terlihat bahwa
daerah dibawah kurva lebih tertutup sempurna dan tidak terlihat daerah
yang masih berlubang.


Jika kita hitung integral fungsinya maka akan diperoleh hasil yang
mendekati sebenarnya.


\>t &= makelist(a,a,0,pi-0.01,0.01);

\>fx &= makelist(f(t[i]+0.01),i,1,length(t));

\>0.01\*sum(f(x+0.01))


    0.881219234865

Integral fungsi diatas yang memiliki batas tidak dapat kita hitung
langsung secara eksak, tetapi ternyata jika kita mengubah batasnya
menjadi tak hingga kita dapat menghitungnya secara eksak. Berikut akan
ditunjukkan contohnya.


\>$showev('integrate(f(x),x,0,inf))


$$\int_{0}^{\infty }{e^ {- x^2 }\;dx}=\frac{\sqrt{\pi}}{2}$$Contoh lain fungsi tidak memiliki antiderivatif yang hanya dapat
dihitung dengan metode numerik adalah sebagai berikut.


\>function f(x) &= x^(2\*x)


    
                                      2 x
                                     x
    

\>$showev('integrate(f(x),x,0,2))


$$\int_{0}^{2}{x^{2\,x}\;dx}=\int_{0}^{2}{x^{2\,x}\;dx}$$\>x=0:0.002:2-0.002; plot2d(x,f(x+0.002),\>bar); plot2d("f(x)",0,2,\>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-446.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-446.png)

\>k &= makelist(a,a,0,pi-0.002,0.002);

\>fx &= makelist(f(k[i]+0.002),i,1,length(k));

\>0.002\*sum(f(x+0.002))


    5.54658986236

\>function f(x) &= sin(3\*x^5+7)^2


    
                                   2    5
                                sin (3 x  + 7)
    

\>integrate(f,0,1)


    0.542581176074

\>function f(x) &= sin(3\*x^5+7)^2


    
                                   2    5
                                sin (3 x  + 7)
    

\>integrate(f,0,1)


    0.542581176074

Berikut adalah contoh integral fungsi eksponensial yang dapat dihitung
secara eksak.


\>$showev('integrate(x\*exp(-x),x,0,1))


$$\int_{0}^{1}{x\,e^ {- x }\;dx}=1-2\,e^ {- 1 }$$## Latihan:

tentukan integral dari


a.




b.


\>$showev('integrate (3\*x^2+4\*x+2,x,1,2))


$$\int_{1}^{2}{3\,x^2+4\,x+2\;dx}=15$$\>$showev('integrate (sin(x),x,0,pi))


$$\int_{0}^{\pi}{\sin x\;dx}=2$$# Aplikasi Integral Tentu

\>plot2d("x^3-x",-0.1,1.1); plot2d("-x^2",\>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-450.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-450.png)

\>b=solve("x^3-x+x^2",0.5); x=linspace(0,b,200); xi=flipx(x):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-451.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-451.png)

Menggunakan perintah diatas kita mendapatkan penyelesaian dari
gabungan kedua fungsi diatas yang kemudian disimpan dalam variabel b.
Kemudian dibuat baris array x yang berisi 200 nilai dengan interval
dari 0 sampai b untuk kemudian dibali urutan nilai-nilainya menjdai
baris baru yaitu xi.


\>plot2d(x|xi,x^3-x|-xi^2,\>filled,style="|",fillcolor=1,\>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-452.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-452.png)

\>a=solve("x^3-x+x^2",0), b=solve("x^3-x+x^2",1) // absis titik-titik potong kedua kurva


    0
    0.61803398875

Hasil diatas merupakan absis dari kedua titik potong kurva.


\>integrate("(-x^2)-(x^3-x)",a,b) // luas daerah yang diarsir


    0.0758191713542

Hasil perhitungan tadi jika dibandingkan dengan hasil perhitungan
analitik akan menghasilkan nilai perhitungan yang sama. Kita coba
dengan perhitungan analitik sebagai berikut.


\>a &= solve((-x^2)-(x^3-x),x); $a // menentukan absis titik potong kedua kurva secara eksak


$$\left[ x=\frac{-\sqrt{5}-1}{2} , x=\frac{\sqrt{5}-1}{2} , x=0
  \right] $$\>$showev('integrate(-x^2-x^3+x,x,0,(sqrt(5)-1)/2))


$$\int_{0}^{\frac{\sqrt{5}-1}{2}}{-x^3-x^2+x\;dx}=\frac{13-5^{\frac{3
 }{2}}}{24}$$\>$float(%)


$$\int_{0.0}^{0.6180339887498949}{-1.0\,x^3-1.0\,x^2+x\;dx}=
 0.07581917135421037$$Hasil perhitungan analitik menunjukkan hasil yang sama dengan
perhitungan sebelumnya.


## Panjang Kurva

Hitunglah panjang kurva berikut ini dan luas daerah di dalam kurva
tersebut.


dengan


\>t=linspace(0,2pi,1000); r=1+sin(3\*t)/2; x=r\*cos(t); y=r\*sin(t);

\>plot2d(x,y,\>filled,fillcolor=red,style="/",r=1.5):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-456.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-456.png)

Perintah diatas akan menghasilkan larik array t yang berjumlah 1000
nilai terdistribusi dari 0 sampai 2pi. Selajutnya dibuat plot dari
korrdinat x dan y dengan skala yang diperbesar 1.5 kali.


\>function r(t) &= 1+sin(3\*t)/2; $'r(t)=r(t)


$$r\left(\left[ 0 , 0.01 , 0.02 , 0.03 , 0.04 , 0.05 , 0.06 , 0.07 , 
 0.08 , 0.09 , 0.1 , 0.11 , 0.12 , 0.13 , 0.14 , 0.15 , 0.16 , 0.17
  , 0.18 , 0.19 , 0.2 , 0.21 , 0.2200000000000001 , 
 0.2300000000000001 , 0.2400000000000001 , 0.2500000000000001 , 
 0.2600000000000001 , 0.2700000000000001 , 0.2800000000000001 , 
 0.2900000000000001 , 0.3000000000000001 , 0.3100000000000001 , 
 0.3200000000000001 , 0.3300000000000001 , 0.3400000000000001 , 
 0.3500000000000001 , 0.3600000000000002 , 0.3700000000000002 , 
 0.3800000000000002 , 0.3900000000000002 , 0.4000000000000002 , 
 0.4100000000000002 , 0.4200000000000002 , 0.4300000000000002 , 
 0.4400000000000002 , 0.4500000000000002 , 0.4600000000000002 , 
 0.4700000000000003 , 0.4800000000000003 , 0.4900000000000003 , 
 0.5000000000000002 , 0.5100000000000002 , 0.5200000000000002 , 
 0.5300000000000002 , 0.5400000000000003 , 0.5500000000000003 , 
 0.5600000000000003 , 0.5700000000000003 , 0.5800000000000003 , 
 0.5900000000000003 , 0.6000000000000003 , 0.6100000000000003 , 
 0.6200000000000003 , 0.6300000000000003 , 0.6400000000000003 , 
 0.6500000000000004 , 0.6600000000000004 , 0.6700000000000004 , 
 0.6800000000000004 , 0.6900000000000004 , 0.7000000000000004 , 
 0.7100000000000004 , 0.7200000000000004 , 0.7300000000000004 , 
 0.7400000000000004 , 0.7500000000000004 , 0.7600000000000005 , 
 0.7700000000000005 , 0.7800000000000005 , 0.7900000000000005 , 
 0.8000000000000005 , 0.8100000000000005 , 0.8200000000000005 , 
 0.8300000000000005 , 0.8400000000000005 , 0.8500000000000005 , 
 0.8600000000000005 , 0.8700000000000006 , 0.8800000000000006 , 
 0.8900000000000006 , 0.9000000000000006 , 0.9100000000000006 , 
 0.9200000000000006 , 0.9300000000000006 , 0.9400000000000006 , 
 0.9500000000000006 , 0.9600000000000006 , 0.9700000000000006 , 
 0.9800000000000006 , 0.9900000000000007 , 1.000000000000001 , 
 1.010000000000001 , 1.020000000000001 , 1.030000000000001 , 
 1.040000000000001 , 1.050000000000001 , 1.060000000000001 , 
 1.070000000000001 , 1.080000000000001 , 1.090000000000001 , 
 1.100000000000001 , 1.110000000000001 , 1.120000000000001 , 
 1.130000000000001 , 1.140000000000001 , 1.150000000000001 , 
 1.160000000000001 , 1.170000000000001 , 1.180000000000001 , 
 1.190000000000001 , 1.200000000000001 , 1.210000000000001 , 
 1.220000000000001 , 1.230000000000001 , 1.240000000000001 , 
 1.250000000000001 , 1.260000000000001 , 1.270000000000001 , 
 1.280000000000001 , 1.290000000000001 , 1.300000000000001 , 
 1.310000000000001 , 1.320000000000001 , 1.330000000000001 , 
 1.340000000000001 , 1.350000000000001 , 1.360000000000001 , 
 1.370000000000001 , 1.380000000000001 , 1.390000000000001 , 
 1.400000000000001 , 1.410000000000001 , 1.420000000000001 , 
 1.430000000000001 , 1.440000000000001 , 1.450000000000001 , 
 1.460000000000001 , 1.470000000000001 , 1.480000000000001 , 
 1.490000000000001 , 1.500000000000001 , 1.510000000000001 , 
 1.520000000000001 , 1.530000000000001 , 1.540000000000001 , 
 1.550000000000001 , 1.560000000000001 , 1.570000000000001 , 
 1.580000000000001 , 1.590000000000001 , 1.600000000000001 , 
 1.610000000000001 , 1.620000000000001 , 1.630000000000001 , 
 1.640000000000001 , 1.650000000000001 , 1.660000000000001 , 
 1.670000000000001 , 1.680000000000001 , 1.690000000000001 , 
 1.700000000000001 , 1.710000000000001 , 1.720000000000001 , 
 1.730000000000001 , 1.740000000000001 , 1.750000000000001 , 
 1.760000000000001 , 1.770000000000001 , 1.780000000000001 , 
 1.790000000000001 , 1.800000000000001 , 1.810000000000001 , 
 1.820000000000001 , 1.830000000000001 , 1.840000000000001 , 
 1.850000000000001 , 1.860000000000001 , 1.870000000000001 , 
 1.880000000000001 , 1.890000000000001 , 1.900000000000001 , 
 1.910000000000001 , 1.920000000000001 , 1.930000000000001 , 
 1.940000000000002 , 1.950000000000002 , 1.960000000000002 , 
 1.970000000000002 , 1.980000000000002 , 1.990000000000002 , 
 2.000000000000001 , 2.010000000000001 , 2.020000000000001 , 
 2.030000000000001 , 2.04 , 2.05 , 2.06 , 2.07 , 2.08 , 
 2.089999999999999 , 2.099999999999999 , 2.109999999999999 , 
 2.119999999999999 , 2.129999999999999 , 2.139999999999998 , 
 2.149999999999998 , 2.159999999999998 , 2.169999999999998 , 
 2.179999999999997 , 2.189999999999997 , 2.199999999999997 , 
 2.209999999999997 , 2.219999999999997 , 2.229999999999996 , 
 2.239999999999996 , 2.249999999999996 , 2.259999999999996 , 
 2.269999999999996 , 2.279999999999995 , 2.289999999999995 , 
 2.299999999999995 , 2.309999999999995 , 2.319999999999995 , 
 2.329999999999994 , 2.339999999999994 , 2.349999999999994 , 
 2.359999999999994 , 2.369999999999993 , 2.379999999999993 , 
 2.389999999999993 , 2.399999999999993 , 2.409999999999993 , 
 2.419999999999992 , 2.429999999999992 , 2.439999999999992 , 
 2.449999999999992 , 2.459999999999992 , 2.469999999999991 , 
 2.479999999999991 , 2.489999999999991 , 2.499999999999991 , 
 2.50999999999999 , 2.51999999999999 , 2.52999999999999 , 
 2.53999999999999 , 2.54999999999999 , 2.559999999999989 , 
 2.569999999999989 , 2.579999999999989 , 2.589999999999989 , 
 2.599999999999989 , 2.609999999999988 , 2.619999999999988 , 
 2.629999999999988 , 2.639999999999988 , 2.649999999999987 , 
 2.659999999999987 , 2.669999999999987 , 2.679999999999987 , 
 2.689999999999987 , 2.699999999999986 , 2.709999999999986 , 
 2.719999999999986 , 2.729999999999986 , 2.739999999999986 , 
 2.749999999999985 , 2.759999999999985 , 2.769999999999985 , 
 2.779999999999985 , 2.789999999999984 , 2.799999999999984 , 
 2.809999999999984 , 2.819999999999984 , 2.829999999999984 , 
 2.839999999999983 , 2.849999999999983 , 2.859999999999983 , 
 2.869999999999983 , 2.879999999999983 , 2.889999999999982 , 
 2.899999999999982 , 2.909999999999982 , 2.919999999999982 , 
 2.929999999999982 , 2.939999999999981 , 2.949999999999981 , 
 2.959999999999981 , 2.969999999999981 , 2.97999999999998 , 
 2.98999999999998 , 2.99999999999998 , 3.00999999999998 , 
 3.01999999999998 , 3.029999999999979 , 3.039999999999979 , 
 3.049999999999979 , 3.059999999999979 , 3.069999999999979 , 
 3.079999999999978 , 3.089999999999978 , 3.099999999999978 , 
 3.109999999999978 , 3.119999999999977 , 3.129999999999977 \right] 
 \right)=\left[ 1 , 1.014997750101248 , 1.029982003239722 , 
 1.044939274599006 , 1.05985610364446 , 1.0747190662368 , 
 1.089514786712912 , 1.10422994992305 , 1.118851313213567 , 
 1.133365718344415 , 1.14776010333067 , 1.162021514197434 , 
 1.176137116637545 , 1.190094207561581 , 1.203880226529785 , 
 1.217482767055615 , 1.230889587770742 , 1.244088623441454 , 
 1.257067995826556 , 1.269816024366985 , 1.282321236697518 , 
 1.294572378971135 , 1.306558425986717 , 1.318268591110984 , 
 1.329692335985737 , 1.340819380011667 , 1.351639709600205 , 
 1.362143587185071 , 1.37232155998543 , 1.382164468512753 , 
 1.391663454813742 , 1.400809970441889 , 1.409595784150499 , 
 1.41801298930026 , 1.426054010974682 , 1.433711612797009 , 
 1.440978903442474 , 1.447849342840024 , 1.454316748057942 , 
 1.460375298868068 , 1.466019542983613 , 1.471244400965849 , 
 1.476045170795258 , 1.480417532103036 , 1.484357550059133 , 
 1.48786167891333 , 1.49092676518618 , 1.493550050506925 , 
 1.495729174095843 , 1.49746217488879 , 1.498747493302027 , 
 1.499583972635738 , 1.499970860114983 , 1.499907807567145 , 
 1.499394871735262 , 1.498432514226959 , 1.497021601099038 , 
 1.495163402078079 , 1.492859589417777 , 1.490112236394023 , 
 1.486923815439098 , 1.483297195916649 , 1.479235641539457 , 
 1.474742807432315 , 1.469822736842662 , 1.464479857501934 , 
 1.458718977640905 , 1.4525452816626 , 1.44596432547669 , 
 1.438982031499539 , 1.431604683324436 , 1.423838920066784 , 
 1.415691730389341 , 1.407170446212898 , 1.398282736118043 , 
 1.38903659844396 , 1.379440354090461 , 1.369502639029735 , 
 1.359232396534563 , 1.348638869129968 , 1.337731590275575 , 
 1.326520375786132 , 1.315015314997945 , 1.303226761689157 , 
 1.29116532476204 , 1.278841858695708 , 1.26626745377781 , 
 1.253453426124026 , 1.240411307494323 , 1.227152834915152 , 
 1.213689940116914 , 1.200034738796209 , 1.186199519712527 , 
 1.172196733629194 , 1.158038982108526 , 1.143739006171271 , 
 1.129309674830555 , 1.114763973510631 , 1.100114992360884 , 
 1.085375914475572 , 1.070560004029933 , 1.055680594343324 , 
 1.040751075880133 , 1.025784884199266 , 1.010795487863047 , 
 0.9957963763164246 , 0.9808010477473812 , 0.965822996939475 , 
 0.9508757031274447 , 0.9359726178668091 , 0.9211271529283745 , 
 0.9063526682285473 , 0.8916624598063091 , 0.8770697478576804 , 
 0.8625876648384367 , 0.8482292436457843 , 0.8340074058896318 , 
 0.8199349502640146 , 0.8060245410291336 , 0.7922886966143758 , 
 0.7787397783525728 , 0.7653899793556352 , 0.7522513135415764 , 
 0.7393356048227956 , 0.7266544764653555 , 0.7142193406288271 , 
 0.7020413880961168 , 0.6901315782025174 , 0.6785006289730446 , 
 0.6671590074769393 , 0.656116920408012 , 0.645384304899306 , 
 0.6349708195803493 , 0.6248858358850397 , 0.6151384296179869 , 
 0.6057373727869018 , 0.5966911257083789 , 0.5880078293941864 , 
 0.5796952982249017 , 0.5717610129174986 , 0.5642121137932052 , 
 0.557055394351698 , 0.5502972951574103 , 0.5439438980434592 , 
 0.5380009206384055 , 0.5324737112207749 , 0.5273672439059678 , 
 0.5226861141698913 , 0.5184345347133413 , 0.5146163316708554 , 
 0.511234941167451 , 0.5082934062263444 , 0.5057943740304345 , 
 0.5037400935400183 , 0.5021324134688772 , 0.5009727806205602 , 
 0.500262238586358 , 0.500001426806141 , 0.5001905799929074 , 
 0.5008295279215563 , 0.5019176955820799 , 0.5034541036970326 , 
 0.5054373696028154 , 0.5078657084939796 , 0.5107369350294311 , 
 0.51404846529909 , 0.5177973191492352 , 0.5219801228644414 , 
 0.5265931122036962 , 0.5316321357879612 , 0.5370926588361347 , 
 0.5429697672460474 , 0.5492581720168234 , 0.5559522140086237 , 
 0.5630458690354898 , 0.5705327532867048 , 0.5784061290717926 , 
 0.5866589108839831 , 0.5952836717766916 , 0.6042726500472684 , 
 0.6136177562220075 , 0.6233105803361282 , 0.6333423995021732 , 
 0.6437041857600205 , 0.6543866142014381 , 0.6653800713618707 , 
 0.6766746638719099 , 0.6882602273606591 , 0.7001263356029799 , 
 0.7122623099023933 , 0.724657228701183 , 0.7372999374090619 , 
 0.7501790584415506 , 0.7632830014590344 , 0.776599973797287 , 
 0.7901179910800726 , 0.8038248880042751 , 0.8177083292878514 , 
 0.8317558207707499 , 0.845954720658813 , 0.8602922509005387 , 
 0.8747555086864638 , 0.8893314780608216 , 0.9040070416350233 , 
 0.9187689923924234 , 0.9336040455737417 , 0.9484988506324511 , 
 0.963440003249368 , 0.9784140573956348 , 0.9934075374332381 , 
 1.008406950242174 , 1.023398797363343 , 1.038369587146257 , 
 1.053305846890609 , 1.068194134970796 , 1.083021052932476 , 
 1.097773257550269 , 1.112437472835763 , 1.127000501985008 , 
 1.141449239254742 , 1.155770681756685 , 1.169951941159252 , 
 1.183980255286187 , 1.19784299960166 , 1.211527698571493 , 
 1.225022036890303 , 1.238313870564444 , 1.25139123784078 , 
 1.264242369971459 , 1.276855701804989 , 1.289219882194093 , 
 1.30132378421098 , 1.313156515160821 , 1.324707426384449 , 
 1.335966122841424 , 1.346922472464875 , 1.357566615279672 , 
 1.36788897227574 , 1.37788025402852 , 1.387531469058827 , 
 1.39683393192457 , 1.405779271037068 , 1.414359436194911 , 
 1.422566705828602 , 1.430393693949445 , 1.437833356796435 , 
 1.444878999175174 , 1.451524280483087 , 1.457763220415539 , 
 1.463590204347708 , 1.468999988387365 , 1.473987704094021 , 
 1.478548862860204 , 1.482679359950892 , 1.486375478197503 , 
 1.489633891343097 , 1.492451667035778 , 1.494826269467617 , 
 1.496755561656706 , 1.498237807370299 , 1.499271672687302 , 
 1.499856227198713 , 1.499990944844928 , 1.499675704389159 , 
 1.498910789526538 , 1.497696888628812 , 1.496035094124851 , 
 1.493926901517543 , 1.491374208037935 , 1.488379310937856 , 
 1.484944905422548 , 1.481074082225159 , 1.476770324825293 , 
 1.472037506314117 , 1.466879885908833 , 1.461302105119679 , 
 1.455309183572874 , 1.448906514493302 , 1.442099859850967 , 
 1.434895345175611 , 1.427299454044153 , 1.419319022245902 , 
 1.410961231630815 , 1.402233603646312 , 1.39314399256848 , 
 1.38370057843376 , 1.373911859677462 , 1.363786645485748 , 
 1.353334047867958 , 1.34256347345642 , 1.331484615041111 , 
 1.320107442846807 , 1.308442195560544 , 1.2964993711175 , 
 1.284289717253558 , 1.271824221833068 , 1.259114102960513 , 
 1.24617079888497 , 1.233005957706462 , 1.219631426893447 , 
 1.206059242620906 , 1.192301618938587 , 1.178370936779193 , 
 1.164279732816375 , 1.150040688182572 , 1.135666617056847 , 
 1.121170455132993 , 1.106565247978279 , 1.091864139293324 , 
 1.077080359083648 , 1.062227211753564 , 1.047318064133114 , 
 1.032366333448817 , 1.017385475249078 \right] $$\>function fx(t) &= r(t)\*cos(t); $'fx(t)=fx(t)


$${\it fx}\left(\left[ 0 , 0.01 , 0.02 , 0.03 , 0.04 , 0.05 , 0.06 , 
 0.07 , 0.08 , 0.09 , 0.1 , 0.11 , 0.12 , 0.13 , 0.14 , 0.15 , 0.16
  , 0.17 , 0.18 , 0.19 , 0.2 , 0.21 , 0.2200000000000001 , 
 0.2300000000000001 , 0.2400000000000001 , 0.2500000000000001 , 
 0.2600000000000001 , 0.2700000000000001 , 0.2800000000000001 , 
 0.2900000000000001 , 0.3000000000000001 , 0.3100000000000001 , 
 0.3200000000000001 , 0.3300000000000001 , 0.3400000000000001 , 
 0.3500000000000001 , 0.3600000000000002 , 0.3700000000000002 , 
 0.3800000000000002 , 0.3900000000000002 , 0.4000000000000002 , 
 0.4100000000000002 , 0.4200000000000002 , 0.4300000000000002 , 
 0.4400000000000002 , 0.4500000000000002 , 0.4600000000000002 , 
 0.4700000000000003 , 0.4800000000000003 , 0.4900000000000003 , 
 0.5000000000000002 , 0.5100000000000002 , 0.5200000000000002 , 
 0.5300000000000002 , 0.5400000000000003 , 0.5500000000000003 , 
 0.5600000000000003 , 0.5700000000000003 , 0.5800000000000003 , 
 0.5900000000000003 , 0.6000000000000003 , 0.6100000000000003 , 
 0.6200000000000003 , 0.6300000000000003 , 0.6400000000000003 , 
 0.6500000000000004 , 0.6600000000000004 , 0.6700000000000004 , 
 0.6800000000000004 , 0.6900000000000004 , 0.7000000000000004 , 
 0.7100000000000004 , 0.7200000000000004 , 0.7300000000000004 , 
 0.7400000000000004 , 0.7500000000000004 , 0.7600000000000005 , 
 0.7700000000000005 , 0.7800000000000005 , 0.7900000000000005 , 
 0.8000000000000005 , 0.8100000000000005 , 0.8200000000000005 , 
 0.8300000000000005 , 0.8400000000000005 , 0.8500000000000005 , 
 0.8600000000000005 , 0.8700000000000006 , 0.8800000000000006 , 
 0.8900000000000006 , 0.9000000000000006 , 0.9100000000000006 , 
 0.9200000000000006 , 0.9300000000000006 , 0.9400000000000006 , 
 0.9500000000000006 , 0.9600000000000006 , 0.9700000000000006 , 
 0.9800000000000006 , 0.9900000000000007 , 1.000000000000001 , 
 1.010000000000001 , 1.020000000000001 , 1.030000000000001 , 
 1.040000000000001 , 1.050000000000001 , 1.060000000000001 , 
 1.070000000000001 , 1.080000000000001 , 1.090000000000001 , 
 1.100000000000001 , 1.110000000000001 , 1.120000000000001 , 
 1.130000000000001 , 1.140000000000001 , 1.150000000000001 , 
 1.160000000000001 , 1.170000000000001 , 1.180000000000001 , 
 1.190000000000001 , 1.200000000000001 , 1.210000000000001 , 
 1.220000000000001 , 1.230000000000001 , 1.240000000000001 , 
 1.250000000000001 , 1.260000000000001 , 1.270000000000001 , 
 1.280000000000001 , 1.290000000000001 , 1.300000000000001 , 
 1.310000000000001 , 1.320000000000001 , 1.330000000000001 , 
 1.340000000000001 , 1.350000000000001 , 1.360000000000001 , 
 1.370000000000001 , 1.380000000000001 , 1.390000000000001 , 
 1.400000000000001 , 1.410000000000001 , 1.420000000000001 , 
 1.430000000000001 , 1.440000000000001 , 1.450000000000001 , 
 1.460000000000001 , 1.470000000000001 , 1.480000000000001 , 
 1.490000000000001 , 1.500000000000001 , 1.510000000000001 , 
 1.520000000000001 , 1.530000000000001 , 1.540000000000001 , 
 1.550000000000001 , 1.560000000000001 , 1.570000000000001 , 
 1.580000000000001 , 1.590000000000001 , 1.600000000000001 , 
 1.610000000000001 , 1.620000000000001 , 1.630000000000001 , 
 1.640000000000001 , 1.650000000000001 , 1.660000000000001 , 
 1.670000000000001 , 1.680000000000001 , 1.690000000000001 , 
 1.700000000000001 , 1.710000000000001 , 1.720000000000001 , 
 1.730000000000001 , 1.740000000000001 , 1.750000000000001 , 
 1.760000000000001 , 1.770000000000001 , 1.780000000000001 , 
 1.790000000000001 , 1.800000000000001 , 1.810000000000001 , 
 1.820000000000001 , 1.830000000000001 , 1.840000000000001 , 
 1.850000000000001 , 1.860000000000001 , 1.870000000000001 , 
 1.880000000000001 , 1.890000000000001 , 1.900000000000001 , 
 1.910000000000001 , 1.920000000000001 , 1.930000000000001 , 
 1.940000000000002 , 1.950000000000002 , 1.960000000000002 , 
 1.970000000000002 , 1.980000000000002 , 1.990000000000002 , 
 2.000000000000001 , 2.010000000000001 , 2.020000000000001 , 
 2.030000000000001 , 2.04 , 2.05 , 2.06 , 2.07 , 2.08 , 
 2.089999999999999 , 2.099999999999999 , 2.109999999999999 , 
 2.119999999999999 , 2.129999999999999 , 2.139999999999998 , 
 2.149999999999998 , 2.159999999999998 , 2.169999999999998 , 
 2.179999999999997 , 2.189999999999997 , 2.199999999999997 , 
 2.209999999999997 , 2.219999999999997 , 2.229999999999996 , 
 2.239999999999996 , 2.249999999999996 , 2.259999999999996 , 
 2.269999999999996 , 2.279999999999995 , 2.289999999999995 , 
 2.299999999999995 , 2.309999999999995 , 2.319999999999995 , 
 2.329999999999994 , 2.339999999999994 , 2.349999999999994 , 
 2.359999999999994 , 2.369999999999993 , 2.379999999999993 , 
 2.389999999999993 , 2.399999999999993 , 2.409999999999993 , 
 2.419999999999992 , 2.429999999999992 , 2.439999999999992 , 
 2.449999999999992 , 2.459999999999992 , 2.469999999999991 , 
 2.479999999999991 , 2.489999999999991 , 2.499999999999991 , 
 2.50999999999999 , 2.51999999999999 , 2.52999999999999 , 
 2.53999999999999 , 2.54999999999999 , 2.559999999999989 , 
 2.569999999999989 , 2.579999999999989 , 2.589999999999989 , 
 2.599999999999989 , 2.609999999999988 , 2.619999999999988 , 
 2.629999999999988 , 2.639999999999988 , 2.649999999999987 , 
 2.659999999999987 , 2.669999999999987 , 2.679999999999987 , 
 2.689999999999987 , 2.699999999999986 , 2.709999999999986 , 
 2.719999999999986 , 2.729999999999986 , 2.739999999999986 , 
 2.749999999999985 , 2.759999999999985 , 2.769999999999985 , 
 2.779999999999985 , 2.789999999999984 , 2.799999999999984 , 
 2.809999999999984 , 2.819999999999984 , 2.829999999999984 , 
 2.839999999999983 , 2.849999999999983 , 2.859999999999983 , 
 2.869999999999983 , 2.879999999999983 , 2.889999999999982 , 
 2.899999999999982 , 2.909999999999982 , 2.919999999999982 , 
 2.929999999999982 , 2.939999999999981 , 2.949999999999981 , 
 2.959999999999981 , 2.969999999999981 , 2.97999999999998 , 
 2.98999999999998 , 2.99999999999998 , 3.00999999999998 , 
 3.01999999999998 , 3.029999999999979 , 3.039999999999979 , 
 3.049999999999979 , 3.059999999999979 , 3.069999999999979 , 
 3.079999999999978 , 3.089999999999978 , 3.099999999999978 , 
 3.109999999999978 , 3.119999999999977 , 3.129999999999977 \right] 
 \right)=\left[ 1 , 1.014947000636657 , 1.029776013705529 , 
 1.044469087191079 , 1.059008331806833 , 1.073375947255439 , 
 1.087554248364218 , 1.101525691055367 , 1.11527289811021 , 
 1.128778684687222 , 1.142026083553954 , 1.154998369993414 , 
 1.16767908634602 , 1.180052066148761 , 1.192101457833886 , 
 1.203811747950136 , 1.215167783870255 , 1.226154795949382 , 
 1.236758419099762 , 1.246964713748154 , 1.256760186143285 , 
 1.266131807981756 , 1.275067035321848 , 1.283553826755846 , 
 1.29158066081265 , 1.29913655256367 , 1.306211069406282 , 
 1.312794346000405 , 1.318877098335118 , 1.324450636903608 , 
 1.329506878966172 , 1.334038359882425 , 1.338038243495345 , 
 1.341500331551311 , 1.344419072141793 , 1.346789567153917 , 
 1.348607578718725 , 1.349869534647481 , 1.350572532848044 , 
 1.350714344714907 , 1.350293417488142 , 1.349308875578123 , 
 1.347760520854542 , 1.345648831899879 , 1.342974962229111 , 
 1.339740737479097 , 1.335948651572729 , 1.331601861864506 , 
 1.326704183275865 , 1.321260081430156 , 1.315274664798767 , 
 1.308753675871437 , 1.301703481365363 , 1.294131061489226 , 
 1.286043998279732 , 1.277450463029762 , 1.268359202828647 , 
 1.25877952623647 , 1.248721288115691 , 1.238194873644713 , 
 1.227211181539273 , 1.215781606508839 , 1.203918020976346 , 
 1.191632756090801 , 1.17893858206338 , 1.165848687858719 , 
 1.152376660274093 , 1.138536462440146 , 1.124342411777761 , 
 1.10980915744646 , 1.094951657320579 , 1.079785154530145 , 
 1.064325153604093 , 1.04858739625406 , 1.032587836837555 , 
 1.0163426175398 , 0.999868043313951 , 0.9831805566197906 , 
 0.9662967120012925 , 0.9492331505436565 , 0.932006574250646 , 
 0.9146337203831 , 0.897131335799599 , 0.8795161513401855 , 
 0.8618048562939812 , 0.8440140729913906 , 0.8261603315613344 , 
 0.8082600448937051 , 0.7903294838468643 , 0.7723847527396025 , 
 0.754441765166499 , 0.7365162201750889 , 0.7186235788426429 , 
 0.7007790412897039 , 0.6829975241668103 , 0.6652936386500562 , 
 0.6476816689803099 , 0.6301755515800127 , 0.6127888547805567 , 
 0.595534759192214 , 0.5784260387475773 , 0.5614750424483481 , 
 0.5446936768441829 , 0.5280933892711049 , 0.5116851518757627 , 
 0.4954794464505473 , 0.4794862501032484 , 0.4637150217835931 , 
 0.4481746896876128 , 0.4328736395593664 , 0.4178197039080948 , 
 0.4030201521573983 , 0.3884816817415227 , 0.3742104101623088 , 
 0.3602118680188048 , 0.3464909930199702 , 0.3330521249893116 , 
 0.3198990018686896 , 0.3070347567269186 , 0.2944619157771625 , 
 0.2821823974055002 , 0.2701975122114014 , 0.2585079640592211 , 
 0.24711385213819 , 0.236014674026751 , 0.2252093297554723 , 
 0.2146961268611566 , 0.2044727864231691 , 0.1945364500714196 , 
 0.1848836879538733 , 0.1755105076499143 , 0.1664123640143599 , 
 0.15758416993543 , 0.1490203079884969 , 0.1407146429660004 , 
 0.1326605352625015 , 0.1248508550924698 , 0.1172779975170584 , 
 0.1099338982548158 , 0.1028100502500252 , 0.09589752097113614 , 
 0.08918697041058306 , 0.08266866975615104 , 0.07633252070297167 , 
 0.07016807537419696 , 0.06416455681742222 , 0.05831088004299921 , 
 0.05259567356951026 , 0.04700730144085663 , 0.04153388567865525 , 
 0.03616332913293765 , 0.03088333869350296 , 0.02568144882369685 , 
 0.02054504537786921 , 0.01546138966330633 , 0.01041764270704039 , 
 0.005400889687608656 , 3.981644915699177 \times 10^{-4} , -
 0.004603525645615616 , -0.009617175454872322 , -0.01465575694556099
  , -0.01973219475490163 , -0.02485934157531223 , -
 0.03004995370008319 , -0.03531666672761627 , -0.04067197146420217 , 
 -0.04612819006499101 , -0.05169745245242638 , -0.05739167305096758
  , -0.06322252787641469 , -0.06920143201758122 , -
 0.07533951754742671 , -0.08164761190007062 , -0.08813621674935902 , 
 -0.09481548742384746 , -0.1016952128922007 , -0.1087847963520907 , -
 0.1160932364547031 , -0.1236291091959386 , -0.1314005505043224 , -
 0.139415239554513 , -0.1476803828341322 , -0.1562026989904259 , -
 0.1649884044820097 , -0.174043200059654 , -0.1833722580987308 , -
 0.1929802108045716 , -0.2028711393105765 , -0.213048563687482 , -
 0.2235154338807206 , -0.2342741215913132 , -0.2453264131142145 , -
 0.2566735031464869 , -0.2683159895761154 , -0.2802538692606958 , -
 0.2924865348036311 , -0.3050127723338639 , -0.3178307602935531 , -
 0.3309380692364743 , -0.3443316626383011 , -0.3580078987182807 , -
 0.3719625332701944 , -0.3861907234988561 , -0.4006870328567865 , -
 0.4154454368740791 , -0.4304593299728726 , -0.4457215332562533 , -
 0.4612243032598357 , -0.4769593416527143 , -0.4929178058729419 , -
 0.5090903206811831 , -0.5254669906146977 , -0.5420374133223633 , -
 0.5587906937600045 , -0.5757154592239161 , -0.5927998751991035 , -
 0.6100316619974365 , -0.6273981121596448 , -0.6448861085938298 , -
 0.6624821434219715 , -0.6801723375047791 , -0.697942460614089 , -
 0.7157779522210085 , -0.7336639428669554 , -0.7515852760838196 , -
 0.7695265308285668 , -0.7874720443967583 , -0.8054059357786804 , -
 0.8233121294210486 , -0.84117437935658 , -0.8589762936631191 , -
 0.8767013592134671 , -0.8943329666765518 , -0.9118544357301941 , -
 0.9292490404453213 , -0.9465000348012289 , -0.9635906782912238 , -
 0.9805042615778466 , -0.9972241321567511 , -1.013733719988298 , -
 1.030016563055939 , -1.046056332810583 , -1.061836859460272 , -
 1.077342157064746 , -1.092556448394762 , -1.10746418951636 , -
 1.122050094060758 , -1.136299157140943 , -1.150196678876666 , -
 1.163728287490093 , -1.176879961935049 , -1.189638054023528 , -
 1.20198931001392 , -1.21392089162623 , -1.225420396450494 , -
 1.23647587771553 , -1.247075863386148 , -1.257209374558044 , -
 1.266865943120662 , -1.276035628659481 , -1.28470903457039 , -
 1.292877323360026 , -1.30053223110728 , -1.307666081062444 , -
 1.314271796361877 , -1.320342911837456 , -1.32587358490148 , -
 1.330858605489208 , -1.335293405042638 , -1.339174064520721 , -
 1.342497321422677 , -1.345260575812696 , -1.347461895335851 , -
 1.349100019216673 , -1.350174361233419 , -1.350685011662737 , -
 1.350632738191 , -1.350018985790271 , -1.348845875558472 , -
 1.347116202524988 , -1.344833432424572 , -1.342001697444045 , -
 1.338625790947931 , -1.334711161190771 , -1.330263904025476 , -
 1.325290754618677 , -1.319799078185586 , -1.313796859758453 , -
 1.307292693004252 , -1.3002957681087 , -1.29281585874522 , -
 1.284863308148933 , -1.276449014317106 , -1.267584414358992 , -
 1.258281468019224 , -1.248552640400313 , -1.238410883911061 , -
 1.227869619468906 , -1.216942716985417 , -1.205644475165291 , -
 1.19398960065031 , -1.181993186540708 , -1.169670690327459 , -
 1.157037911269867 , -1.144110967253747 , -1.13090627116632 , -
 1.117440506824699 , -1.103730604495534 , -1.089793716044085 , -
 1.075647189751512 , -1.061308544839763 , -1.046795445743849 , -
 1.03212567617173 , -1.017317112992372 \right] $$\>function fy(t) &= r(t)\*sin(t); $'fy(t)=fy(t)


$${\it fy}\left(\left[ 0 , 0.01 , 0.02 , 0.03 , 0.04 , 0.05 , 0.06 , 
 0.07 , 0.08 , 0.09 , 0.1 , 0.11 , 0.12 , 0.13 , 0.14 , 0.15 , 0.16
  , 0.17 , 0.18 , 0.19 , 0.2 , 0.21 , 0.2200000000000001 , 
 0.2300000000000001 , 0.2400000000000001 , 0.2500000000000001 , 
 0.2600000000000001 , 0.2700000000000001 , 0.2800000000000001 , 
 0.2900000000000001 , 0.3000000000000001 , 0.3100000000000001 , 
 0.3200000000000001 , 0.3300000000000001 , 0.3400000000000001 , 
 0.3500000000000001 , 0.3600000000000002 , 0.3700000000000002 , 
 0.3800000000000002 , 0.3900000000000002 , 0.4000000000000002 , 
 0.4100000000000002 , 0.4200000000000002 , 0.4300000000000002 , 
 0.4400000000000002 , 0.4500000000000002 , 0.4600000000000002 , 
 0.4700000000000003 , 0.4800000000000003 , 0.4900000000000003 , 
 0.5000000000000002 , 0.5100000000000002 , 0.5200000000000002 , 
 0.5300000000000002 , 0.5400000000000003 , 0.5500000000000003 , 
 0.5600000000000003 , 0.5700000000000003 , 0.5800000000000003 , 
 0.5900000000000003 , 0.6000000000000003 , 0.6100000000000003 , 
 0.6200000000000003 , 0.6300000000000003 , 0.6400000000000003 , 
 0.6500000000000004 , 0.6600000000000004 , 0.6700000000000004 , 
 0.6800000000000004 , 0.6900000000000004 , 0.7000000000000004 , 
 0.7100000000000004 , 0.7200000000000004 , 0.7300000000000004 , 
 0.7400000000000004 , 0.7500000000000004 , 0.7600000000000005 , 
 0.7700000000000005 , 0.7800000000000005 , 0.7900000000000005 , 
 0.8000000000000005 , 0.8100000000000005 , 0.8200000000000005 , 
 0.8300000000000005 , 0.8400000000000005 , 0.8500000000000005 , 
 0.8600000000000005 , 0.8700000000000006 , 0.8800000000000006 , 
 0.8900000000000006 , 0.9000000000000006 , 0.9100000000000006 , 
 0.9200000000000006 , 0.9300000000000006 , 0.9400000000000006 , 
 0.9500000000000006 , 0.9600000000000006 , 0.9700000000000006 , 
 0.9800000000000006 , 0.9900000000000007 , 1.000000000000001 , 
 1.010000000000001 , 1.020000000000001 , 1.030000000000001 , 
 1.040000000000001 , 1.050000000000001 , 1.060000000000001 , 
 1.070000000000001 , 1.080000000000001 , 1.090000000000001 , 
 1.100000000000001 , 1.110000000000001 , 1.120000000000001 , 
 1.130000000000001 , 1.140000000000001 , 1.150000000000001 , 
 1.160000000000001 , 1.170000000000001 , 1.180000000000001 , 
 1.190000000000001 , 1.200000000000001 , 1.210000000000001 , 
 1.220000000000001 , 1.230000000000001 , 1.240000000000001 , 
 1.250000000000001 , 1.260000000000001 , 1.270000000000001 , 
 1.280000000000001 , 1.290000000000001 , 1.300000000000001 , 
 1.310000000000001 , 1.320000000000001 , 1.330000000000001 , 
 1.340000000000001 , 1.350000000000001 , 1.360000000000001 , 
 1.370000000000001 , 1.380000000000001 , 1.390000000000001 , 
 1.400000000000001 , 1.410000000000001 , 1.420000000000001 , 
 1.430000000000001 , 1.440000000000001 , 1.450000000000001 , 
 1.460000000000001 , 1.470000000000001 , 1.480000000000001 , 
 1.490000000000001 , 1.500000000000001 , 1.510000000000001 , 
 1.520000000000001 , 1.530000000000001 , 1.540000000000001 , 
 1.550000000000001 , 1.560000000000001 , 1.570000000000001 , 
 1.580000000000001 , 1.590000000000001 , 1.600000000000001 , 
 1.610000000000001 , 1.620000000000001 , 1.630000000000001 , 
 1.640000000000001 , 1.650000000000001 , 1.660000000000001 , 
 1.670000000000001 , 1.680000000000001 , 1.690000000000001 , 
 1.700000000000001 , 1.710000000000001 , 1.720000000000001 , 
 1.730000000000001 , 1.740000000000001 , 1.750000000000001 , 
 1.760000000000001 , 1.770000000000001 , 1.780000000000001 , 
 1.790000000000001 , 1.800000000000001 , 1.810000000000001 , 
 1.820000000000001 , 1.830000000000001 , 1.840000000000001 , 
 1.850000000000001 , 1.860000000000001 , 1.870000000000001 , 
 1.880000000000001 , 1.890000000000001 , 1.900000000000001 , 
 1.910000000000001 , 1.920000000000001 , 1.930000000000001 , 
 1.940000000000002 , 1.950000000000002 , 1.960000000000002 , 
 1.970000000000002 , 1.980000000000002 , 1.990000000000002 , 
 2.000000000000001 , 2.010000000000001 , 2.020000000000001 , 
 2.030000000000001 , 2.04 , 2.05 , 2.06 , 2.07 , 2.08 , 
 2.089999999999999 , 2.099999999999999 , 2.109999999999999 , 
 2.119999999999999 , 2.129999999999999 , 2.139999999999998 , 
 2.149999999999998 , 2.159999999999998 , 2.169999999999998 , 
 2.179999999999997 , 2.189999999999997 , 2.199999999999997 , 
 2.209999999999997 , 2.219999999999997 , 2.229999999999996 , 
 2.239999999999996 , 2.249999999999996 , 2.259999999999996 , 
 2.269999999999996 , 2.279999999999995 , 2.289999999999995 , 
 2.299999999999995 , 2.309999999999995 , 2.319999999999995 , 
 2.329999999999994 , 2.339999999999994 , 2.349999999999994 , 
 2.359999999999994 , 2.369999999999993 , 2.379999999999993 , 
 2.389999999999993 , 2.399999999999993 , 2.409999999999993 , 
 2.419999999999992 , 2.429999999999992 , 2.439999999999992 , 
 2.449999999999992 , 2.459999999999992 , 2.469999999999991 , 
 2.479999999999991 , 2.489999999999991 , 2.499999999999991 , 
 2.50999999999999 , 2.51999999999999 , 2.52999999999999 , 
 2.53999999999999 , 2.54999999999999 , 2.559999999999989 , 
 2.569999999999989 , 2.579999999999989 , 2.589999999999989 , 
 2.599999999999989 , 2.609999999999988 , 2.619999999999988 , 
 2.629999999999988 , 2.639999999999988 , 2.649999999999987 , 
 2.659999999999987 , 2.669999999999987 , 2.679999999999987 , 
 2.689999999999987 , 2.699999999999986 , 2.709999999999986 , 
 2.719999999999986 , 2.729999999999986 , 2.739999999999986 , 
 2.749999999999985 , 2.759999999999985 , 2.769999999999985 , 
 2.779999999999985 , 2.789999999999984 , 2.799999999999984 , 
 2.809999999999984 , 2.819999999999984 , 2.829999999999984 , 
 2.839999999999983 , 2.849999999999983 , 2.859999999999983 , 
 2.869999999999983 , 2.879999999999983 , 2.889999999999982 , 
 2.899999999999982 , 2.909999999999982 , 2.919999999999982 , 
 2.929999999999982 , 2.939999999999981 , 2.949999999999981 , 
 2.959999999999981 , 2.969999999999981 , 2.97999999999998 , 
 2.98999999999998 , 2.99999999999998 , 3.00999999999998 , 
 3.01999999999998 , 3.029999999999979 , 3.039999999999979 , 
 3.049999999999979 , 3.059999999999979 , 3.069999999999979 , 
 3.079999999999978 , 3.089999999999978 , 3.099999999999978 , 
 3.109999999999978 , 3.119999999999977 , 3.129999999999977 \right] 
 \right)=\left[ 0 , 0.01014980833556662 , 0.02059826678292271 , 
 0.03134347622283015 , 0.04238293991838228 , 0.05371356612987439 , 
 0.06533167172990376 , 0.07723298681299934 , 0.08941266029246918 , 
 0.1018652664755576 , 0.1145848126064173 , 0.1275647473648353 , 
 0.1407979703071057 , 0.1542768422339107 , 0.1679931964685752 , 
 0.1819383510275811 , 0.1961031216637831 , 0.2104778357613507 , 
 0.2250523470600841 , 0.2398160511854019 , 0.2547579019589912 , 
 0.2698664284638497 , 0.2851297528362152 , 0.3005356087557041 , 
 0.3160713606038417 , 0.3317240232600813 , 0.3474802825033731 , 
 0.3633265159863522 , 0.3792488147482899 , 0.3952330052320643 , 
 0.411264671769591 , 0.4273291794993832 , 0.4434116976792021 , 
 0.4594972233561165 , 0.4755706053556919 , 0.4916165685515136 , 
 0.5076197383757777 , 0.5235646655312819 , 0.5394358508648145 , 
 0.5552177703616642 , 0.5708949002207642 , 0.5864517419698421 , 
 0.6018728475798654 , 0.6171428445380648 , 0.6322464608388652 , 
 0.6471685498521687 , 0.6618941150286309 , 0.6764083344018014 , 
 0.6906965848473219 , 0.704744466059751 , 0.7185378242080237 , 
 0.7320627752310482 , 0.7453057277355214 , 0.7582534054586558 , 
 0.7708928692592016 , 0.7832115386008901 , 0.7951972124932317 , 
 0.8068380898554457 , 0.8181227892702304 , 0.8290403680950348 , 
 0.8395803408995157 , 0.8497326971989371 , 0.8594879184543822 , 
 0.8688369943118147 , 0.877771438053233 , 0.8862833012344233 , 
 0.894365187485098 , 0.9020102654485477 , 0.9092122808393135 , 
 0.91596556759876 , 0.9222650581299157 , 0.9281062925943645 , 
 0.9334854272555032 , 0.9383992418539865 , 0.9428451460027243 , 
 0.9468211845903713 , 0.9503260421838114 , 0.9533590464217597 , 
 0.9559201703932094 , 0.9580100339960551 , 0.9596299042728891 , 
 0.9607816947225576 , 0.9614679635877484 , 0.9616919111204768 , 
 0.9614573758289937 , 0.9607688297112769 , 0.9596313724818526 , 
 0.9580507248003547 , 0.9560332205117796 , 0.9535857979100135 , 
 0.950715990037748 , 0.9474319140374602 , 0.9437422595696462 , 
 0.9396562763159917 , 0.9351837605866338 , 0.9303350410521015 , 
 0.9251209636219332 , 0.9195528754933222 , 0.9136426083945087 , 
 0.9074024610488752 , 0.9008451808870137 , 0.8939839450352001 , 
 0.8868323406098919 , 0.8794043443489797 , 0.8717143016115846 , 
 0.8637769047792269 , 0.8556071710921349 , 0.8472204199553921 , 
 0.8386322497504639 , 0.8298585141884582 , 0.820915298242203 , 
 0.8118188936949144 , 0.8025857743438493 , 0.7932325708978999 , 
 0.7837760456085848 , 0.774233066674328 , 0.7646205824582917 , 
 0.7549555955603404 , 0.7452551367839522 , 0.7355362390390766 , 
 0.7258159112220526 , 0.7161111121137482 , 0.7064387243370677 , 
 0.6968155284148838 , 0.687258176969315 , 0.6777831691030455 , 
 0.668406825003112 , 0.6591452608072385 , 0.6500143637723917 , 
 0.6410297677847648 , 0.6322068292498609 , 0.6235606034007541 , 
 0.6151058210619551 , 0.6068568659055925 , 0.5988277522358446 , 
 0.5910321033367347 , 0.5834831304175053 , 0.5761936121888643 , 
 0.5691758751023778 , 0.5624417742842642 , 0.5560026751937326 , 
 0.5498694360348715 , 0.544052390949907 , 0.53856133402041 , 
 0.5334055041017602 , 0.5285935705148607 , 0.524133619617734 , 
 0.5200331422782496 , 0.5162990222678009 , 0.5129375255942972 , 
 0.5099542907913512 , 0.5073543201790264 , 0.5051419721099751 , 
 0.5033209542132412 , 0.5018943176464132 , 0.5008644523652326 , 
 0.5002330834181367 , 0.500001268271606 , 0.5001693951705475 , 
 0.5007371825363073 , 0.5017036794032689 , 0.5030672668933421 , 
 0.5048256607260124 , 0.5069759147599763 , 0.5095144255607565 , 
 0.5124369379870706 , 0.5157385517871076 , 0.5194137291942778 , 
 0.5234563035104128 , 0.5278594886628308 , 0.5326158897201478 , 
 0.537717514350191 , 0.5431557852018865 , 0.5489215531915289 , 
 0.5550051116724135 , 0.5613962114654124 , 0.5680840767267195 , 
 0.5750574216276612 , 0.5823044678201934 , 0.5898129626604602 , 
 0.5975701981615958 , 0.6055630306457991 , 0.6137779010646088 , 
 0.6222008559552548 , 0.6308175689999582 , 0.6396133631541016 , 
 0.6485732333083022 , 0.6576818694485768 , 0.666923680278004 , 
 0.6762828172625756 , 0.6857431990632479 , 0.6952885363156223 , 
 0.7049023567181215 , 0.7145680303890611 , 0.7242687954525969 , 
 0.7339877838131736 , 0.7437080470778139 , 0.7534125825853661 , 
 0.7630843595016599 , 0.772706344939443 , 0.7822615300619331 , 
 0.7917329561288537 , 0.8011037404439425 , 0.8103571021630719 , 
 0.8194763879223699 , 0.828445097246017 , 0.8372469076937672 , 
 0.8458656997086601 , 0.854285581125889 , 0.8624909113043309 , 
 0.8704663248428698 , 0.8781967548443059 , 0.8856674556903905 , 
 0.8928640252922927 , 0.8997724267816849 , 0.906379009608506 , 
 0.9126705300124326 , 0.9186341708361021 , 0.9242575606491771 , 
 0.9295287921534543 , 0.9344364398403978 , 0.9389695768736348 , 
 0.9431177911702464 , 0.9468712006559368 , 0.9502204676705017 , 
 0.9531568125013942 , 0.9556720260245586 , 0.9577584814331576 , 
 0.9594091450362716 , 0.9606175861111349 , 0.9613779857939967 , 
 0.9616851449962428 , 0.9615344913339456 , 0.9609220850606357 , 
 0.9598446239946319 , 0.9582994474339243 , 0.9562845390531859 , 
 0.9537985287791452 , 0.9508406936421651 , 0.947410957603528 , 
 0.9435098903595474 , 0.9391387051252784 , 0.9342992554022154 , 
 0.9289940307359997 , 0.9232261514717631 , 0.9169993625163411 , 
 0.9103180261181786 , 0.9031871136772969 , 0.8956121965992712 , 
 0.887599436208666 , 0.8791555727388846 , 0.8702879134168627 , 
 0.861004319662487 , 0.8513131934239982 , 0.8412234626720594 , 
 0.8307445660764733 , 0.8198864368908458 , 0.8086594860717609 , 
 0.7970745846602297 , 0.7851430454543705 , 0.7728766040033802 , 
 0.7602873989539559 , 0.747387951781335 , 0.7341911459381067 , 
 0.7207102054548656 , 0.7069586730276477 , 0.6929503876278947 , 
 0.6786994616714588 , 0.6642202577838278 , 0.6495273651994194 , 
 0.6346355758333427 , 0.6195598600645386 , 0.6043153422696768 , 
 0.5889172761475558 , 0.5733810198740807 , 0.5577220111281572 , 
 0.5419557420290201 , 0.5260977340256624 , 0.5101635127790679 , 
 0.494168583077974 , 0.4781284038288049 , 0.4620583631602888 , 
 0.4459737536830763 , 0.4298897479444084 , 0.4138213741175589 , 
 0.3977834919653886 , 0.3817907691168823 , 0.3658576576950352 , 
 0.3499983713338726 , 0.3342268626217452 , 0.3185568010073464 , 
 0.3030015512041419 , 0.2875741521280825 , 0.2722872964026102 , 
 0.2571533104640303 , 0.2421841352993548 , 0.2273913078476872 , 
 0.2127859430951425 , 0.1983787168921659 , 0.1841798495209409 , 
 0.1701990900393635 , 0.1564457014267882 , 0.1429284465554646 , 
 0.1296555750102305 , 0.1166348107776594 , 0.1038733408244504 , 
 0.09137780458340303 , 0.07915428436385227 , 0.0672082967019403 , 
 0.05554478466457765 , 0.04416811111940389 , 0.03308205298149149 , 
 0.02228979644595547 , 0.01179393321403596 \right] $$\>function ds(t) &= trigreduce(radcan(sqrt(diff(fx(t),t)^2+diff(fy(t),t)^2))); $'ds(t)=ds(t)


    Maxima said:
    diff: second argument must be a variable; found errexp1
     -- an error. To debug this try: debugmode(true);
    
    Error in:
    ... e(radcan(sqrt(diff(fx(t),t)^2+diff(fy(t),t)^2))); $'ds(t)=ds(t ...
                                                         ^

Sintaks diatas digunakan untuk menghitung panjang elemen diferensial
pada kurva yaitu menghitung turunan pertama fungsi fx dan fy. Perintah
"trigeduce" berfungsi untuk menyederhanakan ekspresi trigonometri dan
perintah "radcan" untuk menyederhanakan ekspresi akar kuadrat.


\>$integrate(ds(x),x,0,2\*pi)


$$\int_{0}^{2\,\pi}{{\it ds}\left(x\right)\;dx}$$Pada pengintegralan fungsi diatas tidak bisa diselesaikan secara eksak
oleh maxima sehingga kita harus menghitungnya secara numerik dengan
perintah EMT.


\>integrate("ds(x)",0,2\*pi)


    Function ds not found.
    Try list ... to find functions!
    Error in expression: ds(x)
    %mapexpression1:
        return expr(x,args());
    Error in map.
    %evalexpression:
        if maps then return %mapexpression1(x,f$;args());
    gauss:
        if maps then y=%evalexpression(f$,a+h-(h*xn)',maps;args());
    adaptivegauss:
        t1=gauss(f$,c,c+h;args(),=maps);
    Try "trace errors" to inspect local variables after errors.
    integrate:
        return adaptivegauss(f$,a,b,eps*1000;args(),=maps);

Kita juga bisa menghitung panjang kurva yang berbentuk spiral
logaritmik. Contoh fungsinya yaitu sebagai berikut.


\>a=0.1; plot2d("exp(a\*x)\*cos(x)","exp(a\*x)\*sin(x)",r=2,xmin=0,xmax=2\*pi):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-461.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-461.png)

\>&kill(a)


    
                                     done
    

Perintah diatas digunakan untuk menghapus variabel a.


\>function fx(t) &= exp(a\*t)\*cos(t); $'fx(t)=fx(t)


$${\it fx}\left(\left[ 0 , 0.01 , 0.02 , 0.03 , 0.04 , 0.05 , 0.06 , 
 0.07 , 0.08 , 0.09 , 0.1 , 0.11 , 0.12 , 0.13 , 0.14 , 0.15 , 0.16
  , 0.17 , 0.18 , 0.19 , 0.2 , 0.21 , 0.2200000000000001 , 
 0.2300000000000001 , 0.2400000000000001 , 0.2500000000000001 , 
 0.2600000000000001 , 0.2700000000000001 , 0.2800000000000001 , 
 0.2900000000000001 , 0.3000000000000001 , 0.3100000000000001 , 
 0.3200000000000001 , 0.3300000000000001 , 0.3400000000000001 , 
 0.3500000000000001 , 0.3600000000000002 , 0.3700000000000002 , 
 0.3800000000000002 , 0.3900000000000002 , 0.4000000000000002 , 
 0.4100000000000002 , 0.4200000000000002 , 0.4300000000000002 , 
 0.4400000000000002 , 0.4500000000000002 , 0.4600000000000002 , 
 0.4700000000000003 , 0.4800000000000003 , 0.4900000000000003 , 
 0.5000000000000002 , 0.5100000000000002 , 0.5200000000000002 , 
 0.5300000000000002 , 0.5400000000000003 , 0.5500000000000003 , 
 0.5600000000000003 , 0.5700000000000003 , 0.5800000000000003 , 
 0.5900000000000003 , 0.6000000000000003 , 0.6100000000000003 , 
 0.6200000000000003 , 0.6300000000000003 , 0.6400000000000003 , 
 0.6500000000000004 , 0.6600000000000004 , 0.6700000000000004 , 
 0.6800000000000004 , 0.6900000000000004 , 0.7000000000000004 , 
 0.7100000000000004 , 0.7200000000000004 , 0.7300000000000004 , 
 0.7400000000000004 , 0.7500000000000004 , 0.7600000000000005 , 
 0.7700000000000005 , 0.7800000000000005 , 0.7900000000000005 , 
 0.8000000000000005 , 0.8100000000000005 , 0.8200000000000005 , 
 0.8300000000000005 , 0.8400000000000005 , 0.8500000000000005 , 
 0.8600000000000005 , 0.8700000000000006 , 0.8800000000000006 , 
 0.8900000000000006 , 0.9000000000000006 , 0.9100000000000006 , 
 0.9200000000000006 , 0.9300000000000006 , 0.9400000000000006 , 
 0.9500000000000006 , 0.9600000000000006 , 0.9700000000000006 , 
 0.9800000000000006 , 0.9900000000000007 , 1.000000000000001 , 
 1.010000000000001 , 1.020000000000001 , 1.030000000000001 , 
 1.040000000000001 , 1.050000000000001 , 1.060000000000001 , 
 1.070000000000001 , 1.080000000000001 , 1.090000000000001 , 
 1.100000000000001 , 1.110000000000001 , 1.120000000000001 , 
 1.130000000000001 , 1.140000000000001 , 1.150000000000001 , 
 1.160000000000001 , 1.170000000000001 , 1.180000000000001 , 
 1.190000000000001 , 1.200000000000001 , 1.210000000000001 , 
 1.220000000000001 , 1.230000000000001 , 1.240000000000001 , 
 1.250000000000001 , 1.260000000000001 , 1.270000000000001 , 
 1.280000000000001 , 1.290000000000001 , 1.300000000000001 , 
 1.310000000000001 , 1.320000000000001 , 1.330000000000001 , 
 1.340000000000001 , 1.350000000000001 , 1.360000000000001 , 
 1.370000000000001 , 1.380000000000001 , 1.390000000000001 , 
 1.400000000000001 , 1.410000000000001 , 1.420000000000001 , 
 1.430000000000001 , 1.440000000000001 , 1.450000000000001 , 
 1.460000000000001 , 1.470000000000001 , 1.480000000000001 , 
 1.490000000000001 , 1.500000000000001 , 1.510000000000001 , 
 1.520000000000001 , 1.530000000000001 , 1.540000000000001 , 
 1.550000000000001 , 1.560000000000001 , 1.570000000000001 , 
 1.580000000000001 , 1.590000000000001 , 1.600000000000001 , 
 1.610000000000001 , 1.620000000000001 , 1.630000000000001 , 
 1.640000000000001 , 1.650000000000001 , 1.660000000000001 , 
 1.670000000000001 , 1.680000000000001 , 1.690000000000001 , 
 1.700000000000001 , 1.710000000000001 , 1.720000000000001 , 
 1.730000000000001 , 1.740000000000001 , 1.750000000000001 , 
 1.760000000000001 , 1.770000000000001 , 1.780000000000001 , 
 1.790000000000001 , 1.800000000000001 , 1.810000000000001 , 
 1.820000000000001 , 1.830000000000001 , 1.840000000000001 , 
 1.850000000000001 , 1.860000000000001 , 1.870000000000001 , 
 1.880000000000001 , 1.890000000000001 , 1.900000000000001 , 
 1.910000000000001 , 1.920000000000001 , 1.930000000000001 , 
 1.940000000000002 , 1.950000000000002 , 1.960000000000002 , 
 1.970000000000002 , 1.980000000000002 , 1.990000000000002 , 
 2.000000000000001 , 2.010000000000001 , 2.020000000000001 , 
 2.030000000000001 , 2.04 , 2.05 , 2.06 , 2.07 , 2.08 , 
 2.089999999999999 , 2.099999999999999 , 2.109999999999999 , 
 2.119999999999999 , 2.129999999999999 , 2.139999999999998 , 
 2.149999999999998 , 2.159999999999998 , 2.169999999999998 , 
 2.179999999999997 , 2.189999999999997 , 2.199999999999997 , 
 2.209999999999997 , 2.219999999999997 , 2.229999999999996 , 
 2.239999999999996 , 2.249999999999996 , 2.259999999999996 , 
 2.269999999999996 , 2.279999999999995 , 2.289999999999995 , 
 2.299999999999995 , 2.309999999999995 , 2.319999999999995 , 
 2.329999999999994 , 2.339999999999994 , 2.349999999999994 , 
 2.359999999999994 , 2.369999999999993 , 2.379999999999993 , 
 2.389999999999993 , 2.399999999999993 , 2.409999999999993 , 
 2.419999999999992 , 2.429999999999992 , 2.439999999999992 , 
 2.449999999999992 , 2.459999999999992 , 2.469999999999991 , 
 2.479999999999991 , 2.489999999999991 , 2.499999999999991 , 
 2.50999999999999 , 2.51999999999999 , 2.52999999999999 , 
 2.53999999999999 , 2.54999999999999 , 2.559999999999989 , 
 2.569999999999989 , 2.579999999999989 , 2.589999999999989 , 
 2.599999999999989 , 2.609999999999988 , 2.619999999999988 , 
 2.629999999999988 , 2.639999999999988 , 2.649999999999987 , 
 2.659999999999987 , 2.669999999999987 , 2.679999999999987 , 
 2.689999999999987 , 2.699999999999986 , 2.709999999999986 , 
 2.719999999999986 , 2.729999999999986 , 2.739999999999986 , 
 2.749999999999985 , 2.759999999999985 , 2.769999999999985 , 
 2.779999999999985 , 2.789999999999984 , 2.799999999999984 , 
 2.809999999999984 , 2.819999999999984 , 2.829999999999984 , 
 2.839999999999983 , 2.849999999999983 , 2.859999999999983 , 
 2.869999999999983 , 2.879999999999983 , 2.889999999999982 , 
 2.899999999999982 , 2.909999999999982 , 2.919999999999982 , 
 2.929999999999982 , 2.939999999999981 , 2.949999999999981 , 
 2.959999999999981 , 2.969999999999981 , 2.97999999999998 , 
 2.98999999999998 , 2.99999999999998 , 3.00999999999998 , 
 3.01999999999998 , 3.029999999999979 , 3.039999999999979 , 
 3.049999999999979 , 3.059999999999979 , 3.069999999999979 , 
 3.079999999999978 , 3.089999999999978 , 3.099999999999978 , 
 3.109999999999978 , 3.119999999999977 , 3.129999999999977 \right] 
 \right)=\left[ 1 , 0.9999500004166653\,e^{0.01\,a} , 
 0.9998000066665778\,e^{0.02\,a} , 0.9995500337489875\,e^{0.03\,a} , 
 0.9992001066609779\,e^{0.04\,a} , 0.9987502603949663\,e^{0.05\,a} , 
 0.9982005399352042\,e^{0.06\,a} , 0.9975510002532796\,e^{0.07\,a} , 
 0.9968017063026194\,e^{0.08\,a} , 0.9959527330119943\,e^{0.09\,a} , 
 0.9950041652780258\,e^{0.1\,a} , 0.9939560979566968\,e^{0.11\,a} , 
 0.9928086358538663\,e^{0.12\,a} , 0.9915618937147881\,e^{0.13\,a} , 
 0.9902159962126372\,e^{0.14\,a} , 0.9887710779360422\,e^{0.15\,a} , 
 0.9872272833756269\,e^{0.16\,a} , 0.9855847669095608\,e^{0.17\,a} , 
 0.9838436927881214\,e^{0.18\,a} , 0.9820042351172703\,e^{0.19\,a} , 
 0.9800665778412416\,e^{0.2\,a} , 0.9780309147241483\,e^{0.21\,a} , 
 0.9758974493306055\,e^{0.2200000000000001\,a} , 0.9736663950053748\,
 e^{0.2300000000000001\,a} , 0.9713379748520296\,e^{
 0.2400000000000001\,a} , 0.9689124217106447\,e^{0.2500000000000001\,
 a} , 0.9663899781345132\,e^{0.2600000000000001\,a} , 
 0.9637708963658905\,e^{0.2700000000000001\,a} , 0.9610554383107709\,
 e^{0.2800000000000001\,a} , 0.9582438755126972\,e^{
 0.2900000000000001\,a} , 0.955336489125606\,e^{0.3000000000000001\,a
 } , 0.9523335698857134\,e^{0.3100000000000001\,a} , 
 0.9492354180824408\,e^{0.3200000000000001\,a} , 0.9460423435283869\,
 e^{0.3300000000000001\,a} , 0.9427546655283462\,e^{
 0.3400000000000001\,a} , 0.9393727128473789\,e^{0.3500000000000001\,
 a} , 0.9358968236779348\,e^{0.3600000000000002\,a} , 
 0.9323273456060344\,e^{0.3700000000000002\,a} , 0.9286646355765101\,
 e^{0.3800000000000002\,a} , 0.924909059857313\,e^{0.3900000000000002
 \,a} , 0.921060994002885\,e^{0.4000000000000002\,a} , 
 0.917120822816605\,e^{0.4100000000000002\,a} , 0.9130889403123081\,e
 ^{0.4200000000000002\,a} , 0.9089657496748851\,e^{0.4300000000000002
 \,a} , 0.9047516632199634\,e^{0.4400000000000002\,a} , 
 0.9004471023526768\,e^{0.4500000000000002\,a} , 0.8960524975255252\,
 e^{0.4600000000000002\,a} , 0.8915682881953289\,e^{
 0.4700000000000003\,a} , 0.886994922779284\,e^{0.4800000000000003\,a
 } , 0.8823328586101213\,e^{0.4900000000000003\,a} , 
 0.8775825618903726\,e^{0.5000000000000002\,a} , 0.8727445076457512\,
 e^{0.5100000000000002\,a} , 0.8678191796776498\,e^{
 0.5200000000000002\,a} , 0.8628070705147609\,e^{0.5300000000000002\,
 a} , 0.857708681363824\,e^{0.5400000000000003\,a} , 
 0.8525245220595056\,e^{0.5500000000000003\,a} , 0.847255111013416\,e
 ^{0.5600000000000003\,a} , 0.8419009751622686\,e^{0.5700000000000003
 \,a} , 0.8364626499151868\,e^{0.5800000000000003\,a} , 
 0.8309406791001633\,e^{0.5900000000000003\,a} , 0.8253356149096781\,
 e^{0.6000000000000003\,a} , 0.8196480178454794\,e^{
 0.6100000000000003\,a} , 0.8138784566625338\,e^{0.6200000000000003\,
 a} , 0.8080275083121516\,e^{0.6300000000000003\,a} , 
 0.8020957578842924\,e^{0.6400000000000003\,a} , 0.7960837985490556\,
 e^{0.6500000000000004\,a} , 0.7899922314973649\,e^{
 0.6600000000000004\,a} , 0.783821665880849\,e^{0.6700000000000004\,a
 } , 0.7775727187509277\,e^{0.6800000000000004\,a} , 
 0.7712460149971063\,e^{0.6900000000000004\,a} , 0.7648421872844882\,
 e^{0.7000000000000004\,a} , 0.7583618759905079\,e^{
 0.7100000000000004\,a} , 0.7518057291408947\,e^{0.7200000000000004\,
 a} , 0.7451744023448701\,e^{0.7300000000000004\,a} , 
 0.7384685587295876\,e^{0.7400000000000004\,a} , 0.7316888688738206\,
 e^{0.7500000000000004\,a} , 0.7248360107409049\,e^{
 0.7600000000000005\,a} , 0.7179106696109431\,e^{0.7700000000000005\,
 a} , 0.7109135380122771\,e^{0.7800000000000005\,a} , 
 0.7038453156522357\,e^{0.7900000000000005\,a} , 0.696706709347165\,e
 ^{0.8000000000000005\,a} , 0.6894984329517466\,e^{0.8100000000000005
 \,a} , 0.6822212072876132\,e^{0.8200000000000005\,a} , 
 0.6748757600712667\,e^{0.8300000000000005\,a} , 0.6674628258413078\,
 e^{0.8400000000000005\,a} , 0.6599831458849817\,e^{
 0.8500000000000005\,a} , 0.6524374681640515\,e^{0.8600000000000005\,
 a} , 0.6448265472400008\,e^{0.8700000000000006\,a} , 
 0.6371511441985798\,e^{0.8800000000000006\,a} , 0.6294120265736964\,
 e^{0.8900000000000006\,a} , 0.6216099682706641\,e^{
 0.9000000000000006\,a} , 0.6137457494888111\,e^{0.9100000000000006\,
 a} , 0.6058201566434623\,e^{0.9200000000000006\,a} , 
 0.5978339822872978\,e^{0.9300000000000006\,a} , 0.5897880250310977\,
 e^{0.9400000000000006\,a} , 0.581683089463883\,e^{0.9500000000000006
 \,a} , 0.5735199860724561\,e^{0.9600000000000006\,a} , 
 0.5652995311603538\,e^{0.9700000000000006\,a} , 0.5570225467662168\,
 e^{0.9800000000000006\,a} , 0.548689860581587\,e^{0.9900000000000007
 \,a} , 0.5403023058681392\,e^{1.000000000000001\,a} , 
 0.5318607213743549\,e^{1.010000000000001\,a} , 0.523365951251649\,e
 ^{1.020000000000001\,a} , 0.5148188449699548\,e^{1.030000000000001\,
 a} , 0.5062202572327777\,e^{1.040000000000001\,a} , 
 0.4975710478917263\,e^{1.050000000000001\,a} , 0.4888720818605269\,e
 ^{1.060000000000001\,a} , 0.4801242290285335\,e^{1.070000000000001\,
 a} , 0.4713283641737394\,e^{1.080000000000001\,a} , 
 0.4624853668753002\,e^{1.090000000000001\,a} , 0.4535961214255767\,e
 ^{1.100000000000001\,a} , 0.4446615167417062\,e^{1.110000000000001\,
 a} , 0.4356824462767115\,e^{1.120000000000001\,a} , 
 0.4266598079301566\,e^{1.130000000000001\,a} , 0.4175945039583574\,e
 ^{1.140000000000001\,a} , 0.4084874408841566\,e^{1.150000000000001\,
 a} , 0.3993395294062724\,e^{1.160000000000001\,a} , 
 0.3901516843082294\,e^{1.170000000000001\,a} , 0.380924824366881\,e
 ^{1.180000000000001\,a} , 0.3716598722605322\,e^{1.190000000000001\,
 a} , 0.3623577544766728\,e^{1.200000000000001\,a} , 
 0.3530194012193296\,e^{1.210000000000001\,a} , 0.3436457463160462\,e
 ^{1.220000000000001\,a} , 0.3342377271245018\,e^{1.230000000000001\,
 a} , 0.3247962844387754\,e^{1.240000000000001\,a} , 
 0.3153223623952678\,e^{1.250000000000001\,a} , 0.3058169083782885\,e
 ^{1.260000000000001\,a} , 0.2962808729253179\,e^{1.270000000000001\,
 a} , 0.2867152096319546\,e^{1.280000000000001\,a} , 
 0.2771208750565567\,e^{1.290000000000001\,a} , 0.2674988286245865\,e
 ^{1.300000000000001\,a} , 0.2578500325326687\,e^{1.310000000000001\,
 a} , 0.248175451652372\,e^{1.320000000000001\,a} , 
 0.2384760534337223\,e^{1.330000000000001\,a} , 0.2287528078084585\,e
 ^{1.340000000000001\,a} , 0.2190066870930406\,e^{1.350000000000001\,
 a} , 0.2092386658914184\,e^{1.360000000000001\,a} , 
 0.199449720997572\,e^{1.370000000000001\,a} , 0.1896408312978334\,e
 ^{1.380000000000001\,a} , 0.1798129776729985\,e^{1.390000000000001\,
 a} , 0.1699671429002399\,e^{1.400000000000001\,a} , 
 0.1601043115548302\,e^{1.410000000000001\,a} , 0.1502254699116848\,e
 ^{1.420000000000001\,a} , 0.1403316058467356\,e^{1.430000000000001\,
 a} , 0.1304237087381444\,e^{1.440000000000001\,a} , 
 0.1205027693673655\,e^{1.450000000000001\,a} , 0.1105697798200685\,e
 ^{1.460000000000001\,a} , 0.1006257333869306\,e^{1.470000000000001\,
 a} , 0.09067162446430857\,e^{1.480000000000001\,a} , 
 0.08070844845479952\,e^{1.490000000000001\,a} , 0.0707372016677018\,
 e^{1.500000000000001\,a} , 0.06075888121938479\,e^{1.510000000000001
 \,a} , 0.05077448493357807\,e^{1.520000000000001\,a} , 
 0.04078501124158992\,e^{1.530000000000001\,a} , 0.03079145908246501
 \,e^{1.540000000000001\,a} , 0.02079482780309132\,e^{
 1.550000000000001\,a} , 0.01079611705826628\,e^{1.560000000000001\,a
 } , 7.963267107321531 \times 10^{-4}\,e^{1.570000000000001\,a} , -
 0.009203543268809447\,e^{1.580000000000001\,a} , -
 0.01920249290169376\,e^{1.590000000000001\,a} , -0.02919952230128993
 \,e^{1.600000000000001\,a} , -0.03919363177298882\,e^{
 1.610000000000001\,a} , -0.04918382191417166\,e^{1.620000000000001\,
 a} , -0.05916909371414947\,e^{1.630000000000001\,a} , -
 0.06914844865406328\,e^{1.640000000000001\,a} , -0.07912088880673519
 \,e^{1.650000000000001\,a} , -0.08908541693646028\,e^{
 1.660000000000001\,a} , -0.09904103659872934\,e^{1.670000000000001\,
 a} , -0.1089867522398724\,e^{1.680000000000001\,a} , -
 0.1189215692966135\,e^{1.690000000000001\,a} , -0.128844494295526\,e
 ^{1.700000000000001\,a} , -0.1387545349523789\,e^{1.710000000000001
 \,a} , -0.148650700271365\,e^{1.720000000000001\,a} , -
 0.1585320006441991\,e^{1.730000000000001\,a} , -0.1683974479490783\,
 e^{1.740000000000001\,a} , -0.1782460556494934\,e^{1.750000000000001
 \,a} , -0.1880768388928814\,e^{1.760000000000001\,a} , -
 0.1978888146091103\,e^{1.770000000000001\,a} , -0.2076810016087851\,
 e^{1.780000000000001\,a} , -0.2174524206813659\,e^{1.790000000000001
 \,a} , -0.2272020946930884\,e^{1.800000000000001\,a} , -
 0.236929048684676\,e^{1.810000000000001\,a} , -0.2466323099688353\,e
 ^{1.820000000000001\,a} , -0.256310908227524\,e^{1.830000000000001\,
 a} , -0.2659638756089817\,e^{1.840000000000001\,a} , -
 0.2755902468245142\,e^{1.850000000000001\,a} , -0.2851890592450221\,
 e^{1.860000000000001\,a} , -0.2947593529972622\,e^{1.870000000000001
 \,a} , -0.3043001710598347\,e^{1.880000000000001\,a} , -
 0.3138105593588837\,e^{1.890000000000001\,a} , -0.3232895668635048\,
 e^{1.900000000000001\,a} , -0.3327362456808466\,e^{1.910000000000001
 \,a} , -0.3421496511508996\,e^{1.920000000000001\,a} , -
 0.3515288419409613\,e^{1.930000000000001\,a} , -0.3608728801397686\,
 e^{1.940000000000002\,a} , -0.3701808313512883\,e^{1.950000000000002
 \,a} , -0.3794517647881559\,e^{1.960000000000002\,a} , -
 0.3886847533647534\,e^{1.970000000000002\,a} , -0.3978788737899174\,
 e^{1.980000000000002\,a} , -0.407033206659267\,e^{1.990000000000002
 \,a} , -0.4161468365471436\,e^{2.000000000000001\,a} , -
 0.4252188520981534\,e^{2.010000000000001\,a} , -0.4342483461183013\,
 e^{2.020000000000001\,a} , -0.4432344156657097\,e^{2.030000000000001
 \,a} , -0.4521761621409124\,e^{2.04\,a} , -0.4610726913767131\,e^{
 2.05\,a} , -0.4699231137276022\,e^{2.06\,a} , -0.4787265441587198\,e
 ^{2.07\,a} , -0.487482102334359\,e^{2.08\,a} , -0.4961889127059985\,
 e^{2.089999999999999\,a} , -0.5048461045998568\,e^{2.099999999999999
 \,a} , -0.5134528123039588\,e^{2.109999999999999\,a} , -
 0.5220081751547062\,e^{2.119999999999999\,a} , -0.5305113376229437\,
 e^{2.129999999999999\,a} , -0.5389614493995101\,e^{2.139999999999998
 \,a} , -0.5473576654802695\,e^{2.149999999999998\,a} , -
 0.5556991462506109\,e^{2.159999999999998\,a} , -0.5639850575694082\,
 e^{2.169999999999998\,a} , -0.5722145708524347\,e^{2.179999999999997
 \,a} , -0.5803868631552197\,e^{2.189999999999997\,a} , -
 0.5885011172553434\,e^{2.199999999999997\,a} , -0.5965565217341574\,
 e^{2.209999999999997\,a} , -0.6045522710579269\,e^{2.219999999999997
 \,a} , -0.6124875656583824\,e^{2.229999999999996\,a} , -
 0.6203616120126767\,e^{2.239999999999996\,a} , -0.628173622722736\,e
 ^{2.249999999999996\,a} , -0.6359228165939993\,e^{2.259999999999996
 \,a} , -0.6436084187135371\,e^{2.269999999999996\,a} , -
 0.6512296605275422\,e^{2.279999999999995\,a} , -0.6587857799181841\,
 e^{2.289999999999995\,a} , -0.6662760212798204\,e^{2.299999999999995
 \,a} , -0.673699635594557\,e^{2.309999999999995\,a} , -
 0.6810558805071486\,e^{2.319999999999995\,a} , -0.6883440203992341\,
 e^{2.329999999999994\,a} , -0.6955633264628979\,e^{2.339999999999994
 \,a} , -0.7027130767735495\,e^{2.349999999999994\,a} , -
 0.7097925563621161\,e^{2.359999999999994\,a} , -0.7168010572865383\,
 e^{2.369999999999993\,a} , -0.723737878702564\,e^{2.379999999999993
 \,a} , -0.7306023269338324\,e^{2.389999999999993\,a} , -
 0.7373937155412407\,e^{2.399999999999993\,a} , -0.7441113653915875\,
 e^{2.409999999999993\,a} , -0.7507546047254859\,e^{2.419999999999992
 \,a} , -0.7573227692245386\,e^{2.429999999999992\,a} , -
 0.7638152020777689\,e^{2.439999999999992\,a} , -0.7702312540473021\,
 e^{2.449999999999992\,a} , -0.7765702835332877\,e^{2.459999999999992
 \,a} , -0.7828316566380599\,e^{2.469999999999991\,a} , -
 0.7890147472295257\,e^{2.479999999999991\,a} , -0.7951189370037787\,
 e^{2.489999999999991\,a} , -0.8011436155469281\,e^{2.499999999999991
 \,a} , -0.8070881803961404\,e^{2.50999999999999\,a} , -
 0.8129520370998843\,e^{2.51999999999999\,a} , -0.818734599277376\,e
 ^{2.52999999999999\,a} , -0.8244352886772165\,e^{2.53999999999999\,a
 } , -0.8300535352352164\,e^{2.54999999999999\,a} , -
 0.8355887771314018\,e^{2.559999999999989\,a} , -0.8410404608461957\,
 e^{2.569999999999989\,a} , -0.8464080412157696\,e^{2.579999999999989
 \,a} , -0.8516909814865598\,e^{2.589999999999989\,a} , -
 0.8568887533689413\,e^{2.599999999999989\,a} , -0.8620008370900576\,
 e^{2.609999999999988\,a} , -0.8670267214457965\,e^{2.619999999999988
 \,a} , -0.8719659038519106\,e^{2.629999999999988\,a} , -
 0.8768178903942755\,e^{2.639999999999988\,a} , -0.88158219587828\,e
 ^{2.649999999999987\,a} , -0.886258343877346\,e^{2.659999999999987\,
 a} , -0.8908458667805706\,e^{2.669999999999987\,a} , -
 0.8953443058394861\,e^{2.679999999999987\,a} , -0.8997532112139355\,
 e^{2.689999999999987\,a} , -0.9040721420170553\,e^{2.699999999999986
 \,a} , -0.9083006663593644\,e^{2.709999999999986\,a} , -
 0.9124383613919522\,e^{2.719999999999986\,a} , -0.9164848133487636\,
 e^{2.729999999999986\,a} , -0.920439617587975\,e^{2.739999999999986
 \,a} , -0.9243023786324579\,e^{2.749999999999985\,a} , -
 0.9280727102093271\,e^{2.759999999999985\,a} , -0.9317502352885667\,
 e^{2.769999999999985\,a} , -0.9353345861207334\,e^{2.779999999999985
 \,a} , -0.9388254042737308\,e^{2.789999999999984\,a} , -
 0.9422223406686528\,e^{2.799999999999984\,a} , -0.9455250556146907\,
 e^{2.809999999999984\,a} , -0.948733218843102\,e^{2.819999999999984
 \,a} , -0.9518465095402373\,e^{2.829999999999984\,a} , -
 0.9548646163796215\,e^{2.839999999999983\,a} , -0.9577872375530855\,
 e^{2.849999999999983\,a} , -0.9606140808009476\,e^{2.859999999999983
 \,a} , -0.9633448634412386\,e^{2.869999999999983\,a} , -
 0.9659793123979703\,e^{2.879999999999983\,a} , -0.9685171642284423\,
 e^{2.889999999999982\,a} , -0.9709581651495862\,e^{2.899999999999982
 \,a} , -0.9733020710633444\,e^{2.909999999999982\,a} , -
 0.9755486475810786\,e^{2.919999999999982\,a} , -0.9776976700470092\,
 e^{2.929999999999982\,a} , -0.9797489235606806\,e^{2.939999999999981
 \,a} , -0.9817022029984505\,e^{2.949999999999981\,a} , -
 0.983557313034003\,e^{2.959999999999981\,a} , -0.9853140681578805\,e
 ^{2.969999999999981\,a} , -0.9869722926960345\,e^{2.97999999999998\,
 a} , -0.988531820827393\,e^{2.98999999999998\,a} , -
 0.9899924966004426\,e^{2.99999999999998\,a} , -0.9913541739488232\,e
 ^{3.00999999999998\,a} , -0.9926167167059347\,e^{3.01999999999998\,a
 } , -0.9937799986185533\,e^{3.029999999999979\,a} , -
 0.9948439033594574\,e^{3.039999999999979\,a} , -0.9958083245390593\,
 e^{3.049999999999979\,a} , -0.9966731657160448\,e^{3.059999999999979
 \,a} , -0.997438340407017\,e^{3.069999999999979\,a} , -
 0.9981037720951443\,e^{3.079999999999978\,a} , -0.9986693942378124\,
 e^{3.089999999999978\,a} , -0.9991351502732786\,e^{3.099999999999978
 \,a} , -0.9995009936263272\,e^{3.109999999999978\,a} , -
 0.9997668877129279\,e^{3.119999999999977\,a} , -0.9999328059438936\,
 e^{3.129999999999977\,a} \right] $$\>function fy(t) &= exp(a\*t)\*sin(t); $'fy(t)=fy(t)


$${\it fy}\left(\left[ 0 , 0.01 , 0.02 , 0.03 , 0.04 , 0.05 , 0.06 , 
 0.07 , 0.08 , 0.09 , 0.1 , 0.11 , 0.12 , 0.13 , 0.14 , 0.15 , 0.16
  , 0.17 , 0.18 , 0.19 , 0.2 , 0.21 , 0.2200000000000001 , 
 0.2300000000000001 , 0.2400000000000001 , 0.2500000000000001 , 
 0.2600000000000001 , 0.2700000000000001 , 0.2800000000000001 , 
 0.2900000000000001 , 0.3000000000000001 , 0.3100000000000001 , 
 0.3200000000000001 , 0.3300000000000001 , 0.3400000000000001 , 
 0.3500000000000001 , 0.3600000000000002 , 0.3700000000000002 , 
 0.3800000000000002 , 0.3900000000000002 , 0.4000000000000002 , 
 0.4100000000000002 , 0.4200000000000002 , 0.4300000000000002 , 
 0.4400000000000002 , 0.4500000000000002 , 0.4600000000000002 , 
 0.4700000000000003 , 0.4800000000000003 , 0.4900000000000003 , 
 0.5000000000000002 , 0.5100000000000002 , 0.5200000000000002 , 
 0.5300000000000002 , 0.5400000000000003 , 0.5500000000000003 , 
 0.5600000000000003 , 0.5700000000000003 , 0.5800000000000003 , 
 0.5900000000000003 , 0.6000000000000003 , 0.6100000000000003 , 
 0.6200000000000003 , 0.6300000000000003 , 0.6400000000000003 , 
 0.6500000000000004 , 0.6600000000000004 , 0.6700000000000004 , 
 0.6800000000000004 , 0.6900000000000004 , 0.7000000000000004 , 
 0.7100000000000004 , 0.7200000000000004 , 0.7300000000000004 , 
 0.7400000000000004 , 0.7500000000000004 , 0.7600000000000005 , 
 0.7700000000000005 , 0.7800000000000005 , 0.7900000000000005 , 
 0.8000000000000005 , 0.8100000000000005 , 0.8200000000000005 , 
 0.8300000000000005 , 0.8400000000000005 , 0.8500000000000005 , 
 0.8600000000000005 , 0.8700000000000006 , 0.8800000000000006 , 
 0.8900000000000006 , 0.9000000000000006 , 0.9100000000000006 , 
 0.9200000000000006 , 0.9300000000000006 , 0.9400000000000006 , 
 0.9500000000000006 , 0.9600000000000006 , 0.9700000000000006 , 
 0.9800000000000006 , 0.9900000000000007 , 1.000000000000001 , 
 1.010000000000001 , 1.020000000000001 , 1.030000000000001 , 
 1.040000000000001 , 1.050000000000001 , 1.060000000000001 , 
 1.070000000000001 , 1.080000000000001 , 1.090000000000001 , 
 1.100000000000001 , 1.110000000000001 , 1.120000000000001 , 
 1.130000000000001 , 1.140000000000001 , 1.150000000000001 , 
 1.160000000000001 , 1.170000000000001 , 1.180000000000001 , 
 1.190000000000001 , 1.200000000000001 , 1.210000000000001 , 
 1.220000000000001 , 1.230000000000001 , 1.240000000000001 , 
 1.250000000000001 , 1.260000000000001 , 1.270000000000001 , 
 1.280000000000001 , 1.290000000000001 , 1.300000000000001 , 
 1.310000000000001 , 1.320000000000001 , 1.330000000000001 , 
 1.340000000000001 , 1.350000000000001 , 1.360000000000001 , 
 1.370000000000001 , 1.380000000000001 , 1.390000000000001 , 
 1.400000000000001 , 1.410000000000001 , 1.420000000000001 , 
 1.430000000000001 , 1.440000000000001 , 1.450000000000001 , 
 1.460000000000001 , 1.470000000000001 , 1.480000000000001 , 
 1.490000000000001 , 1.500000000000001 , 1.510000000000001 , 
 1.520000000000001 , 1.530000000000001 , 1.540000000000001 , 
 1.550000000000001 , 1.560000000000001 , 1.570000000000001 , 
 1.580000000000001 , 1.590000000000001 , 1.600000000000001 , 
 1.610000000000001 , 1.620000000000001 , 1.630000000000001 , 
 1.640000000000001 , 1.650000000000001 , 1.660000000000001 , 
 1.670000000000001 , 1.680000000000001 , 1.690000000000001 , 
 1.700000000000001 , 1.710000000000001 , 1.720000000000001 , 
 1.730000000000001 , 1.740000000000001 , 1.750000000000001 , 
 1.760000000000001 , 1.770000000000001 , 1.780000000000001 , 
 1.790000000000001 , 1.800000000000001 , 1.810000000000001 , 
 1.820000000000001 , 1.830000000000001 , 1.840000000000001 , 
 1.850000000000001 , 1.860000000000001 , 1.870000000000001 , 
 1.880000000000001 , 1.890000000000001 , 1.900000000000001 , 
 1.910000000000001 , 1.920000000000001 , 1.930000000000001 , 
 1.940000000000002 , 1.950000000000002 , 1.960000000000002 , 
 1.970000000000002 , 1.980000000000002 , 1.990000000000002 , 
 2.000000000000001 , 2.010000000000001 , 2.020000000000001 , 
 2.030000000000001 , 2.04 , 2.05 , 2.06 , 2.07 , 2.08 , 
 2.089999999999999 , 2.099999999999999 , 2.109999999999999 , 
 2.119999999999999 , 2.129999999999999 , 2.139999999999998 , 
 2.149999999999998 , 2.159999999999998 , 2.169999999999998 , 
 2.179999999999997 , 2.189999999999997 , 2.199999999999997 , 
 2.209999999999997 , 2.219999999999997 , 2.229999999999996 , 
 2.239999999999996 , 2.249999999999996 , 2.259999999999996 , 
 2.269999999999996 , 2.279999999999995 , 2.289999999999995 , 
 2.299999999999995 , 2.309999999999995 , 2.319999999999995 , 
 2.329999999999994 , 2.339999999999994 , 2.349999999999994 , 
 2.359999999999994 , 2.369999999999993 , 2.379999999999993 , 
 2.389999999999993 , 2.399999999999993 , 2.409999999999993 , 
 2.419999999999992 , 2.429999999999992 , 2.439999999999992 , 
 2.449999999999992 , 2.459999999999992 , 2.469999999999991 , 
 2.479999999999991 , 2.489999999999991 , 2.499999999999991 , 
 2.50999999999999 , 2.51999999999999 , 2.52999999999999 , 
 2.53999999999999 , 2.54999999999999 , 2.559999999999989 , 
 2.569999999999989 , 2.579999999999989 , 2.589999999999989 , 
 2.599999999999989 , 2.609999999999988 , 2.619999999999988 , 
 2.629999999999988 , 2.639999999999988 , 2.649999999999987 , 
 2.659999999999987 , 2.669999999999987 , 2.679999999999987 , 
 2.689999999999987 , 2.699999999999986 , 2.709999999999986 , 
 2.719999999999986 , 2.729999999999986 , 2.739999999999986 , 
 2.749999999999985 , 2.759999999999985 , 2.769999999999985 , 
 2.779999999999985 , 2.789999999999984 , 2.799999999999984 , 
 2.809999999999984 , 2.819999999999984 , 2.829999999999984 , 
 2.839999999999983 , 2.849999999999983 , 2.859999999999983 , 
 2.869999999999983 , 2.879999999999983 , 2.889999999999982 , 
 2.899999999999982 , 2.909999999999982 , 2.919999999999982 , 
 2.929999999999982 , 2.939999999999981 , 2.949999999999981 , 
 2.959999999999981 , 2.969999999999981 , 2.97999999999998 , 
 2.98999999999998 , 2.99999999999998 , 3.00999999999998 , 
 3.01999999999998 , 3.029999999999979 , 3.039999999999979 , 
 3.049999999999979 , 3.059999999999979 , 3.069999999999979 , 
 3.079999999999978 , 3.089999999999978 , 3.099999999999978 , 
 3.109999999999978 , 3.119999999999977 , 3.129999999999977 \right] 
 \right)=\left[ 0 , 0.009999833334166664\,e^{0.01\,a} , 
 0.01999866669333308\,e^{0.02\,a} , 0.02999550020249566\,e^{0.03\,a}
  , 0.03998933418663416\,e^{0.04\,a} , 0.04997916927067833\,e^{0.05\,
 a} , 0.0599640064794446\,e^{0.06\,a} , 0.06994284733753277\,e^{0.07
 \,a} , 0.0799146939691727\,e^{0.08\,a} , 0.08987854919801104\,e^{
 0.09\,a} , 0.09983341664682814\,e^{0.1\,a} , 0.1097783008371748\,e^{
 0.11\,a} , 0.1197122072889193\,e^{0.12\,a} , 0.1296341426196948\,e^{
 0.13\,a} , 0.1395431146442365\,e^{0.14\,a} , 0.1494381324735992\,e^{
 0.15\,a} , 0.159318206614246\,e^{0.16\,a} , 0.169182349066996\,e^{
 0.17\,a} , 0.1790295734258242\,e^{0.18\,a} , 0.1888588949765006\,e^{
 0.19\,a} , 0.1986693307950612\,e^{0.2\,a} , 0.2084598998460996\,e^{
 0.21\,a} , 0.2182296230808694\,e^{0.2200000000000001\,a} , 
 0.2279775235351885\,e^{0.2300000000000001\,a} , 0.2377026264271347\,
 e^{0.2400000000000001\,a} , 0.247403959254523\,e^{0.2500000000000001
 \,a} , 0.2570805518921552\,e^{0.2600000000000001\,a} , 
 0.2667314366888312\,e^{0.2700000000000001\,a} , 0.2763556485641138\,
 e^{0.2800000000000001\,a} , 0.2859522251048356\,e^{
 0.2900000000000001\,a} , 0.2955202066613397\,e^{0.3000000000000001\,
 a} , 0.3050586364434436\,e^{0.3100000000000001\,a} , 
 0.3145665606161179\,e^{0.3200000000000001\,a} , 0.3240430283948685\,
 e^{0.3300000000000001\,a} , 0.3334870921408145\,e^{
 0.3400000000000001\,a} , 0.3428978074554515\,e^{0.3500000000000001\,
 a} , 0.3522742332750901\,e^{0.3600000000000002\,a} , 
 0.3616154319649622\,e^{0.3700000000000002\,a} , 0.3709204694129828\,
 e^{0.3800000000000002\,a} , 0.3801884151231616\,e^{
 0.3900000000000002\,a} , 0.3894183423086507\,e^{0.4000000000000002\,
 a} , 0.3986093279844231\,e^{0.4100000000000002\,a} , 
 0.4077604530595704\,e^{0.4200000000000002\,a} , 0.416870802429211\,e
 ^{0.4300000000000002\,a} , 0.4259394650659998\,e^{0.4400000000000002
 \,a} , 0.4349655341112304\,e^{0.4500000000000002\,a} , 
 0.44394810696552\,e^{0.4600000000000002\,a} , 0.4528862853790685\,e
 ^{0.4700000000000003\,a} , 0.4617791755414831\,e^{0.4800000000000003
 \,a} , 0.4706258881711582\,e^{0.4900000000000003\,a} , 
 0.4794255386042032\,e^{0.5000000000000002\,a} , 0.4881772468829077\,
 e^{0.5100000000000002\,a} , 0.4968801378437369\,e^{
 0.5200000000000002\,a} , 0.5055333412048472\,e^{0.5300000000000002\,
 a} , 0.5141359916531133\,e^{0.5400000000000003\,a} , 
 0.5226872289306594\,e^{0.5500000000000003\,a} , 0.5311861979208836\,
 e^{0.5600000000000003\,a} , 0.5396320487339695\,e^{
 0.5700000000000003\,a} , 0.5480239367918738\,e^{0.5800000000000003\,
 a} , 0.556361022912784\,e^{0.5900000000000003\,a} , 
 0.5646424733950356\,e^{0.6000000000000003\,a} , 0.5728674601004815\,
 e^{0.6100000000000003\,a} , 0.5810351605373053\,e^{
 0.6200000000000003\,a} , 0.5891447579422698\,e^{0.6300000000000003\,
 a} , 0.5971954413623923\,e^{0.6400000000000003\,a} , 
 0.6051864057360399\,e^{0.6500000000000004\,a} , 0.6131168519734341\,
 e^{0.6600000000000004\,a} , 0.6209859870365599\,e^{
 0.6700000000000004\,a} , 0.6287930240184688\,e^{0.6800000000000004\,
 a} , 0.6365371822219682\,e^{0.6900000000000004\,a} , 
 0.6442176872376913\,e^{0.7000000000000004\,a} , 0.651833771021537\,e
 ^{0.7100000000000004\,a} , 0.6593846719714734\,e^{0.7200000000000004
 \,a} , 0.6668696350036982\,e^{0.7300000000000004\,a} , 
 0.6742879116281454\,e^{0.7400000000000004\,a} , 0.6816387600233345\,
 e^{0.7500000000000004\,a} , 0.6889214451105516\,e^{
 0.7600000000000005\,a} , 0.696135238627357\,e^{0.7700000000000005\,a
 } , 0.7032794192004105\,e^{0.7800000000000005\,a} , 
 0.7103532724176082\,e^{0.7900000000000005\,a} , 0.7173560908995231\,
 e^{0.8000000000000005\,a} , 0.7242871743701429\,e^{
 0.8100000000000005\,a} , 0.7311458297268962\,e^{0.8200000000000005\,
 a} , 0.7379313711099631\,e^{0.8300000000000005\,a} , 
 0.7446431199708596\,e^{0.8400000000000005\,a} , 0.751280405140293\,e
 ^{0.8500000000000005\,a} , 0.7578425628952773\,e^{0.8600000000000005
 \,a} , 0.7643289370255054\,e^{0.8700000000000006\,a} , 
 0.7707388788989696\,e^{0.8800000000000006\,a} , 0.7770717475268242\,
 e^{0.8900000000000006\,a} , 0.7833269096274837\,e^{
 0.9000000000000006\,a} , 0.7895037396899508\,e^{0.9100000000000006\,
 a} , 0.7956016200363664\,e^{0.9200000000000006\,a} , 
 0.8016199408837775\,e^{0.9300000000000006\,a} , 0.8075581004051147\,
 e^{0.9400000000000006\,a} , 0.8134155047893741\,e^{
 0.9500000000000006\,a} , 0.8191915683009986\,e^{0.9600000000000006\,
 a} , 0.8248857133384504\,e^{0.9700000000000006\,a} , 
 0.8304973704919708\,e^{0.9800000000000006\,a} , 0.8360259786005209\,
 e^{0.9900000000000007\,a} , 0.8414709848078968\,e^{1.000000000000001
 \,a} , 0.8468318446180155\,e^{1.010000000000001\,a} , 
 0.8521080219493633\,e^{1.020000000000001\,a} , 0.8572989891886037\,e
 ^{1.030000000000001\,a} , 0.8624042272433388\,e^{1.040000000000001\,
 a} , 0.8674232255940173\,e^{1.050000000000001\,a} , 
 0.8723554823449866\,e^{1.060000000000001\,a} , 0.877200504274682\,e
 ^{1.070000000000001\,a} , 0.8819578068849478\,e^{1.080000000000001\,
 a} , 0.8866269144494876\,e^{1.090000000000001\,a} , 
 0.8912073600614356\,e^{1.100000000000001\,a} , 0.895698685680048\,e
 ^{1.110000000000001\,a} , 0.9001004421765053\,e^{1.120000000000001\,
 a} , 0.9044121893788263\,e^{1.130000000000001\,a} , 
 0.9086334961158836\,e^{1.140000000000001\,a} , 0.9127639402605214\,e
 ^{1.150000000000001\,a} , 0.9168031087717673\,e^{1.160000000000001\,
 a} , 0.920750597736136\,e^{1.170000000000001\,a} , 
 0.9246060124080206\,e^{1.180000000000001\,a} , 0.928368967249167\,e
 ^{1.190000000000001\,a} , 0.9320390859672266\,e^{1.200000000000001\,
 a} , 0.9356160015533862\,e^{1.210000000000001\,a} , 
 0.9390993563190678\,e^{1.220000000000001\,a} , 0.9424888019316978\,e
 ^{1.230000000000001\,a} , 0.9457839994495393\,e^{1.240000000000001\,
 a} , 0.9489846193555865\,e^{1.250000000000001\,a} , 
 0.9520903415905161\,e^{1.260000000000001\,a} , 0.9551008555846925\,e
 ^{1.270000000000001\,a} , 0.9580158602892253\,e^{1.280000000000001\,
 a} , 0.9608350642060729\,e^{1.290000000000001\,a} , 
 0.9635581854171932\,e^{1.300000000000001\,a} , 0.9661849516127343\,e
 ^{1.310000000000001\,a} , 0.9687151001182654\,e^{1.320000000000001\,
 a} , 0.9711483779210448\,e^{1.330000000000001\,a} , 
 0.9734845416953196\,e^{1.340000000000001\,a} , 0.9757233578266593\,e
 ^{1.350000000000001\,a} , 0.9778646024353164\,e^{1.360000000000001\,
 a} , 0.9799080613986144\,e^{1.370000000000001\,a} , 
 0.9818535303723599\,e^{1.380000000000001\,a} , 0.9837008148112767\,e
 ^{1.390000000000001\,a} , 0.9854497299884604\,e^{1.400000000000001\,
 a} , 0.9871001010138505\,e^{1.410000000000001\,a} , 0.98865176285172
 \,e^{1.420000000000001\,a} , 0.990104560337178\,e^{1.430000000000001
 \,a} , 0.9914583481916867\,e^{1.440000000000001\,a} , 
 0.9927129910375886\,e^{1.450000000000001\,a} , 0.993868363411645\,e
 ^{1.460000000000001\,a} , 0.994924349777581\,e^{1.470000000000001\,a
 } , 0.9958808445376401\,e^{1.480000000000001\,a} , 
 0.9967377520431435\,e^{1.490000000000001\,a} , 0.9974949866040546\,e
 ^{1.500000000000001\,a} , 0.9981524724975482\,e^{1.510000000000001\,
 a} , 0.9987101439755831\,e^{1.520000000000001\,a} , 
 0.999167945271476\,e^{1.530000000000001\,a} , 0.9995258306054791\,e
 ^{1.540000000000001\,a} , 0.999783764189357\,e^{1.550000000000001\,a
 } , 0.9999417202299663\,e^{1.560000000000001\,a} , 
 0.9999996829318346\,e^{1.570000000000001\,a} , 0.9999576464987401\,e
 ^{1.580000000000001\,a} , 0.9998156151342908\,e^{1.590000000000001\,
 a} , 0.9995736030415051\,e^{1.600000000000001\,a} , 
 0.9992316344213905\,e^{1.610000000000001\,a} , 0.998789743470524\,e
 ^{1.620000000000001\,a} , 0.9982479743776324\,e^{1.630000000000001\,
 a} , 0.9976063813191736\,e^{1.640000000000001\,a} , 
 0.9968650284539188\,e^{1.650000000000001\,a} , 0.9960239899165366\,e
 ^{1.660000000000001\,a} , 0.9950833498101801\,e^{1.670000000000001\,
 a} , 0.9940432021980758\,e^{1.680000000000001\,a} , 
 0.9929036510941184\,e^{1.690000000000001\,a} , 0.9916648104524685\,e
 ^{1.700000000000001\,a} , 0.9903268041561579\,e^{1.710000000000001\,
 a} , 0.9888897660047012\,e^{1.720000000000001\,a} , 
 0.9873538397007162\,e^{1.730000000000001\,a} , 0.9857191788355533\,e
 ^{1.740000000000001\,a} , 0.9839859468739367\,e^{1.750000000000001\,
 a} , 0.9821543171376182\,e^{1.760000000000001\,a} , 
 0.9802244727880453\,e^{1.770000000000001\,a} , 0.9781966068080444\,e
 ^{1.780000000000001\,a} , 0.9760709219825239\,e^{1.790000000000001\,
 a} , 0.9738476308781949\,e^{1.800000000000001\,a} , 
 0.971526955822315\,e^{1.810000000000001\,a} , 0.9691091288804561\,e
 ^{1.820000000000001\,a} , 0.9665943918332972\,e^{1.830000000000001\,
 a} , 0.9639829961524478\,e^{1.840000000000001\,a} , 
 0.9612752029752996\,e^{1.850000000000001\,a} , 0.9584712830789138\,e
 ^{1.860000000000001\,a} , 0.9555715168529435\,e^{1.870000000000001\,
 a} , 0.9525761942715949\,e^{1.880000000000001\,a} , 0.94948561486463
 \,e^{1.890000000000001\,a} , 0.946300087687414\,e^{1.900000000000001
 \,a} , 0.94301993129001\,e^{1.910000000000001\,a} , 
 0.9396454736853244\,e^{1.920000000000001\,a} , 0.9361770523163055\,e
 ^{1.930000000000001\,a} , 0.9326150140221999\,e^{1.940000000000002\,
 a} , 0.9289597150038688\,e^{1.950000000000002\,a} , 
 0.9252115207881677\,e^{1.960000000000002\,a} , 0.9213708061913948\,e
 ^{1.970000000000002\,a} , 0.9174379552818093\,e^{1.980000000000002\,
 a} , 0.9134133613412245\,e^{1.990000000000002\,a} , 
 0.9092974268256812\,e^{2.000000000000001\,a} , 0.9050905633252004\,e
 ^{2.010000000000001\,a} , 0.9007931915226269\,e^{2.020000000000001\,
 a} , 0.8964057411515596\,e^{2.030000000000001\,a} , 
 0.8919286509533794\,e^{2.04\,a} , 0.8873623686333753\,e^{2.05\,a} , 
 0.8827073508159741\,e^{2.06\,a} , 0.8779640629990781\,e^{2.07\,a} , 
 0.8731329795075167\,e^{2.08\,a} , 0.8682145834456129\,e^{
 2.089999999999999\,a} , 0.8632093666488742\,e^{2.099999999999999\,a}
  , 0.8581178296348094\,e^{2.109999999999999\,a} , 0.8529404815528769
 \,e^{2.119999999999999\,a} , 0.8476778401335705\,e^{
 2.129999999999999\,a} , 0.8423304316366466\,e^{2.139999999999998\,a}
  , 0.8368987907984987\,e^{2.149999999999998\,a} , 0.8313834607786843
 \,e^{2.159999999999998\,a} , 0.8257849931056094\,e^{
 2.169999999999998\,a} , 0.8201039476213756\,e^{2.179999999999997\,a}
  , 0.8143408924257975\,e^{2.189999999999997\,a} , 0.8084964038195919
 \,e^{2.199999999999997\,a} , 0.8025710662467491\,e^{
 2.209999999999997\,a} , 0.7965654722360886\,e^{2.219999999999997\,a}
  , 0.790480222342007\,e^{2.229999999999996\,a} , 0.7843159250844224
 \,e^{2.239999999999996\,a} , 0.7780731968879238\,e^{
 2.249999999999996\,a} , 0.7717526620201285\,e^{2.259999999999996\,a}
  , 0.7653549525292563\,e^{2.269999999999996\,a} , 0.7588807081809249
 \,e^{2.279999999999995\,a} , 0.7523305763941739\,e^{
 2.289999999999995\,a} , 0.7457052121767236\,e^{2.299999999999995\,a}
  , 0.7390052780594745\,e^{2.309999999999995\,a} , 0.7322314440302551
 \,e^{2.319999999999995\,a} , 0.7253843874668235\,e^{
 2.329999999999994\,a} , 0.7184647930691302\,e^{2.339999999999994\,a}
  , 0.7114733527908488\,e^{2.349999999999994\,a} , 0.7044107657701806
 \,e^{2.359999999999994\,a} , 0.6972777382599425\,e^{
 2.369999999999993\,a} , 0.6900749835569413\,e^{2.379999999999993\,a}
  , 0.6828032219306449\,e^{2.389999999999993\,a} , 0.6754631805511563
 \,e^{2.399999999999993\,a} , 0.6680555934164966\,e^{
 2.409999999999993\,a} , 0.6605812012792064\,e^{2.419999999999992\,a}
  , 0.6530407515722708\,e^{2.429999999999992\,a} , 0.6454349983343768
 \,e^{2.439999999999992\,a} , 0.6377647021345101\,e^{
 2.449999999999992\,a} , 0.6300306299958988\,e^{2.459999999999992\,a}
  , 0.6222335553193116\,e^{2.469999999999991\,a} , 0.6143742578057187
 \,e^{2.479999999999991\,a} , 0.6064535233783221\,e^{
 2.489999999999991\,a} , 0.598472144103964\,e^{2.499999999999991\,a}
  , 0.5904309181139206\,e^{2.50999999999999\,a} , 0.5823306495240899
 \,e^{2.51999999999999\,a} , 0.5741721483545806\,e^{2.52999999999999
 \,a} , 0.5659562304487112\,e^{2.53999999999999\,a} , 
 0.5576837173914255\,e^{2.54999999999999\,a} , 0.5493554364271356\,e
 ^{2.559999999999989\,a} , 0.5409722203769975\,e^{2.569999999999989\,
 a} , 0.5325349075556305\,e^{2.579999999999989\,a} , 
 0.5240443416872855\,e^{2.589999999999989\,a} , 0.515501371821474\,e
 ^{2.599999999999989\,a} , 0.5069068522480634\,e^{2.609999999999988\,
 a} , 0.4982616424118489\,e^{2.619999999999988\,a} , 0.48956660682661
 \,e^{2.629999999999988\,a} , 0.4808226149886591\,e^{
 2.639999999999988\,a} , 0.4720305412898936\,e^{2.649999999999987\,a}
  , 0.4631912649303566\,e^{2.659999999999987\,a} , 0.4543056698303179
 \,e^{2.669999999999987\,a} , 0.4453746445418831\,e^{
 2.679999999999987\,a} , 0.4363990821601383\,e^{2.689999999999987\,a}
  , 0.4273798802338422\,e^{2.699999999999986\,a} , 0.4183179406756715
 \,e^{2.709999999999986\,a} , 0.4092141696720303\,e^{
 2.719999999999986\,a} , 0.4000694775924326\,e^{2.729999999999986\,a}
  , 0.3908847788984657\,e^{2.739999999999986\,a} , 0.3816609920523453
 \,e^{2.749999999999985\,a} , 0.3723990394250693\,e^{
 2.759999999999985\,a} , 0.3630998472041824\,e^{2.769999999999985\,a}
  , 0.3537643453011572\,e^{2.779999999999985\,a} , 0.3443934672584046
 \,e^{2.789999999999984\,a} , 0.3349881501559197\,e^{
 2.799999999999984\,a} , 0.3255493345175751\,e^{2.809999999999984\,a}
  , 0.316077964217069\,e^{2.819999999999984\,a} , 0.3065749863835386
 \,e^{2.829999999999984\,a} , 0.2970413513068481\,e^{
 2.839999999999983\,a} , 0.2874780123425605\,e^{2.849999999999983\,a}
  , 0.277885925816603\,e^{2.859999999999983\,a} , 0.2682660509296346
 \,e^{2.869999999999983\,a} , 0.2586193496611275\,e^{
 2.879999999999983\,a} , 0.2489467866731698\,e^{2.889999999999982\,a}
  , 0.2392493292139997\,e^{2.899999999999982\,a} , 0.2295279470212819
 \,e^{2.909999999999982\,a} , 0.2197836122251347\,e^{
 2.919999999999982\,a} , 0.2100172992509174\,e^{2.929999999999982\,a}
  , 0.2002299847217888\,e^{2.939999999999981\,a} , 0.1904226473610458
 \,e^{2.949999999999981\,a} , 0.1805962678942517\,e^{
 2.959999999999981\,a} , 0.1707518289511646\,e^{2.969999999999981\,a}
  , 0.1608903149674751\,e^{2.97999999999998\,a} , 0.1510127120863636
 \,e^{2.98999999999998\,a} , 0.141120008059887\,e^{2.99999999999998\,
 a} , 0.131213192150204\,e^{3.00999999999998\,a} , 0.12129325503065\,
 e^{3.01999999999998\,a} , 0.1113611886866703\,e^{3.029999999999979\,
 a} , 0.1014179863166226\,e^{3.039999999999979\,a} , 
 0.09146464223245798\,e^{3.049999999999979\,a} , 0.08150215176029037
 \,e^{3.059999999999979\,a} , 0.07153151114086496\,e^{
 3.069999999999979\,a} , 0.06155371742993487\,e^{3.079999999999978\,a
 } , 0.05156976839855636\,e^{3.089999999999978\,a} , 
 0.04158066243331267\,e^{3.099999999999978\,a} , 0.03158739843647609
 \,e^{3.109999999999978\,a} , 0.0215909757261186\,e^{
 3.119999999999977\,a} , 0.01159239393618092\,e^{3.129999999999977\,a
 } \right] $$\>function df(t) &= trigreduce(radcan(sqrt(diff(fx(t),t)^2+diff(fy(t),t)^2))); $'df(t)=df(t)


    Maxima said:
    diff: second argument must be a variable; found errexp1
     -- an error. To debug this try: debugmode(true);
    
    Error in:
    ... e(radcan(sqrt(diff(fx(t),t)^2+diff(fy(t),t)^2))); $'df(t)=df(t ...
                                                         ^

\>S &=integrate(df(t),t,0,2\*%pi); $S


    Maxima said:
    defint: variable of integration cannot be a constant; found errexp1
     -- an error. To debug this try: debugmode(true);
    
    Error in:
    S &amp;=integrate(df(t),t,0,2*%pi); $S ...
                                  ^

Variabel S diatas menunjukan panjang kurva spiral.


\>S(a=0.1) // Panjang kurva untuk a=0.1


    Function S not found.
    Try list ... to find functions!
    Error in:
    S(a=0.1) // Panjang kurva untuk a=0.1 ...
            ^

Bentuk kurva yang dapat kita hitung lagi dengan integral yaitu
parabola.


Misalnya menunjukkan bahwa keliling lingkaran dengan jari-jari r
adalah K=2.pi.r


\>plot2d("x^2",xmin=-1,xmax=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-464.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-464.png)

# FUNGSI MULTIVARIABEL

Sebuah fungsi multivariabel adalah pemetaan matematis yang
menghubungkan beberapa variabel independen dengan satu variabel
dependen. Fungsi ini umumnya dinotasikan sebagai


Fungsi multivariabel dapat diwakili dalam bentuk peta atau grafik tiga
dimensi.


Contoh fungsi multivariabel :


Dimana variabel bebasnya yaitu x dan y.


# Grafik Fungsi Multivariabel

Pada fungsi multivariabel, grafik fungsinya merupakan grafik tiga
dimensi. Ruang dimensi tiga dilambangkan dengan




Permukaan dalam R^3 terdapat dua macam yakni permukaan linear dan
kuadratik. Setiap permukaan linear berupa bidang datar, sedangkan
permukaan kuadratik berupa bidang lengkung yang kelengkungannya
bergantung atas bentuk persamaannya.


Untuk membuat grafik fungsi tiga dimensi, maka kita dapat menggunakan
perintah "plot3d()"


## Grafik Fungsi Persamaan Linear Dalam Dimensi Tiga

Bentuk umum persamaan permukaan linear adalah


Contoh grafik persamaan linear di ruang tiga dimensi


\>plot3d("x-1"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-465.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-465.png)

\>plot3d("3\*x+4\*y-12"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-466.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-466.png)

\>plot3d("7\*x-1"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-467.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-467.png)

## Grafik Fungsi Kuadratik di Ruang Dimensi Tiga

Persamaan kuadratik mempunyai rumus umum :


Permukaan-permukaan kuadratik dapat berupa permukaan bola, ellipsoida,
paraboloida, tabung ellips, tabung lingkaran, atau tabung parabola.


Contoh grafik fungsi kuadratik di ruang dimensi tiga:


\>plot3d("x^2+y^2"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-468.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-468.png)

Pada contoh diatas, digunakan ekspresi langsung dalam fungsi plot3d
dan permukaan tersebut berupa paraboloida.


\>function f(x,y) := exp(-(x^2+y^2))

\>plot3d("f", r=5):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-469.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-469.png)

## Latihan:

\>plot3d("y^2-x^2",r=2,):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-470.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-470.png)

Gambar di atas merupakan paraboloida hiperbolik


## Menggambar kurva perpotongan dari dua persamaan

Di EMT kita juga dapat menggabungkan dua kurva pada satu bidang untuk
menggambarkan perpotongan. Untuk masalah ini kita gunakan fungsi &gt;add
dalam prosesnya.


Contoh 1:


\>plot3d("x^2+y^2+z-4",r=5, implicit=3):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-471.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-471.png)

\>plot3d("x^2+y^2-1",implicit=3, r=5, \>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-472.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-472.png)

Dari persamaan diatas, kita dapatkan perpotongan antara paraboloida
dengan tabung lingkaran.


contoh 2:


\>plot3d("x^2+y^2+2z-9",r=5,implicit=3):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-473.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-473.png)

\>plot3d("y-1",r=5, implicit=3, \>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-474.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-474.png)

Dari persamaan diatas, didapatkan perpotongan antara bidang datar dan
bidang lengkung.


## Latihan:

\>plot3d("x^2+y^2-4",r=5,implicit=3); plot3d("y^2+z^2-4",r=5,implicit=3,\>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-475.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-475.png)

Didapatkan perpotongan antara dua tabung lingkaran.


# Turunan Fungsi Multivariabel

## Turunan Fungsi Dua Variabel

Turunan parsial, yaitu turunan fungsi terhadap satu variabel bebas
sementara variabel bebas lainnya dianggap tetap atau konstan.


* 
Turunan Parsial terhadap f terhadap x di (x0,y0)


* 
Turunan Parsial f terhadap y di (x0,y0)


Contoh soal untuk turunan parsial :


\>z &= 2\*x\*y-(1-x^2)


    
                                         2
                                2 x y + x  - 1
    

\>$showev('limit(((2\*(x+h)\*y)-(1-(x+h)^2))/h,h,0))


$$\lim_{h\rightarrow 0}{\frac{2\,\left(x+h\right)\,y+\left(x+h\right)
 ^2-1}{h}}=\lim_{h\rightarrow 0}{\frac{2\,\left(x+h\right)\,y+\left(x
 +h\right)^2-1}{h}}$$Perhitungan akan dilakukan menggunakan diff


\>&diff(z,x) // z akan diturunkan terhadap x


    
                                  2 y + 2 x
    

Karena pada fungsi z terdapat 2xy yang merupakan perkalian, untuk
menghitung turunannya kita gunakan u'v+uv', sehingga turunan dari 2xy:




Kemudian turunan dari variabel berpangkat yaitu:




Jadi turunan dari x^2:




Turunan dari konstanta adalah 0


sehingga, turunan dari fungsi




terhadap x adalah


\>&diff(z,y) // z akan diturunkan terhadap y


    
                                     2 x
    

Seperti pada turunan terhadap x, kita gunakan langkah yang sama namun
kita anggap x konstan.


Jadi, turunan terhadap y dari f(x,y) adalah 2x.


Sehingga, turunan parsial dari


Apabila kita gambarkan grafik untuk masing-masing turunan tersebut
adalah sebagai berikut:


\>plot3d("2\*x+2\*y"): // turunan terhadap x


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-477.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-477.png)

\>plot3d("2\*x"): // turunan terhadap y


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-478.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-478.png)

# Integral

## Integral Lipat Dua

Integral lipat dua f pada R, diberikan oleh




atau bisa ditulis dengan




Misalkan R adalah sebuah persegipanjang dengan sisi-sisi sejajar
sumbu-sumbu koordinat; yaitu, misalkan


Urutan dx dan dy penting karena ia merinci integrasi mana yang akan
dilakukan pertama.


SIFAT-SIFAT INTEGRAL LIPAT DUA:


1. Integral lipat dua bersifat linear, yaitu:


2. Integral lipat dua bersifat aditif(dapat dijumlahkan) pada
persegipanjang yang saling berhimpit pada hanya sebuah ruas garis


3. Sifat perbandingan berlaku jika


CONTOH :


1. Hitung


Dengan memperhatikan urutan dx dan dy, pada soal kali ini kita hitung
integralnya dari sebelah dalam yaitu kita integralkan terhadap x
terlebih dahulu.


\>qx &= integrate((2\*x\*y),x)


    
                                      2
                                     x  y
    

Setelah kita integralkan terhadap x, lalu hasilnya kita integralkan
terhadap y.


\>qy &= integrate(qx,y)


    
                                     2  2
                                    x  y
                                    -----
                                      2
    

Jadi, hasil dari




adalah


2. Hitung


\>f &= 2\*x+3\*y


    
                                  3 y + 2 x
    

Dalam integral sebelah dalam, y berupa konstanta, sehingga


\>fx &= integrate((2\*x+3\*y),x,1,2)


    
                                   3 y + 3
    

Setelah mencari integral terhadap x, lalu kita integralkan hasil
tersebut terhadap y, akibatnya


\>fy &= integrate((3+3\*y),y,0,3)


    
                                      45
                                      --
                                      2
    

# Aplikasi Fungsi Multivariabel

## Penerapan Plot Kontur

Peta kontur seringkali digunakan untuk memperlihatkan kondisi cuaca
atau lainnya dari berbagai titik dalam peta.


1.Buatlah plot kontur dari fungsi berikut


\>f &= 1/2\*(x^2+y^2)


    
                                    2    2
                                   y  + x
                                   -------
                                      2
    

\>aspect(1.5);

\>plot2d(f,level=0:2:20,\>hue,\>spectral,n=200,grid=4,r=5):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-479.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-479.png)

2. Seorang ahli geologi sedang melakukan penelitian di daerah
vulkanik. Dia tertarik untuk memahami bagaimana ketinggian permukaan
tanah di sekitar gunung berapi berubah. Ketinggian di suatu titik (x,
y) dalam kilometer di sekitar gunung berapi tersebut dapat dijelaskan
oleh fungsi ketinggian H(x, y), di mana x dan y adalah koordinat dalam
kilometer. Fungsi ketinggian H(x, y) diberikan oleh persamaan:


Gambarkan plot kontur dari fungsi ketinggian H(x, y) untuk
memvisualisasikan perubahan ketinggian di sekitar gunung berapi dengan
level ketinggian 1 sampai 7 km.


\>h &= 3\*x^2-2\*y^2


    
                                    2      2
                                 3 x  - 2 y
    

\>aspect(1.5);

\>plot2d(h,level=1:1:7,\>hue,\>spectral,n=200,grid=4,r=2):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-480.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-480.png)

# EMT Geometri

# Visualisasi dan Perhitungan Geometri dengan EMT

Euler menyediakan beberapa fungsi untuk melakukan visualisasi dan
perhitungan geometri, baik secara numerik maupun analitik (seperti
biasanya tentunya, menggunakan Maxima). Fungsi-fungsi untuk
visualisasi dan perhitungan geometeri tersebut disimpan di dalam file
program "geometry.e", sehingga file tersebut harus dipanggil sebelum
menggunakan fungsi-fungsi atau perintah-perintah untuk geometri.


\>load geometry


    Numerical and symbolic geometry.

## Fungsi-fungsi Geometri

Fungsi-fungsi untuk Menggambar Objek Geometri:


  defaultd:=textheight()*1.5: nilai asli untuk parameter d  
  setPlotrange(x1,x2,y1,y2): menentukan rentang x dan y pada bidang  

koordinat


  setPlotRange(r): pusat bidang koordinat (0,0) dan batas-batas
sumbu-x dan y adalah -r sd r


  plotPoint (P, "P"): menggambar titik P dan diberi label "P"


  plotSegment (A,B, "AB", d): menggambar ruas garis AB, diberi label
"AB" sejauh d


  plotLine (g, "g", d): menggambar garis g diberi label "g" sejauh d


  plotCircle (c,"c",v,d): Menggambar lingkaran c dan diberi label "c"


  plotLabel (label, P, V, d): menuliskan label pada posisi P


Fungsi-fungsi Geometri Analitik (numerik maupun simbolik):


  turn(v, phi): memutar vektor v sejauh phi  
  turnLeft(v):   memutar vektor v ke kiri  
  turnRight(v):  memutar vektor v ke kanan  
  normalize(v): normal vektor v  
  crossProduct(v, w): hasil kali silang vektorv dan w.  
  lineThrough(A, B): garis melalui A dan B, hasilnya [a,b,c] sdh.  

ax+by=c.


  lineWithDirection(A,v): garis melalui A searah vektor v


  getLineDirection(g): vektor arah (gradien) garis g


  getNormal(g): vektor normal (tegak lurus) garis g


  getPointOnLine(g):  titik pada garis g


  perpendicular(A, g):  garis melalui A tegak lurus garis g


  parallel (A, g):  garis melalui A sejajar garis g


  lineIntersection(g, h):  titik potong garis g dan h


  projectToLine(A, g):   proyeksi titik A pada garis g


  distance(A, B):  jarak titik A dan B


  distanceSquared(A, B):  kuadrat jarak A dan B


  quadrance(A, B): kuadrat jarak A dan B


  areaTriangle(A, B, C):  luas segitiga ABC


  computeAngle(A, B, C):   besar sudut &lt;ABC


  angleBisector(A, B, C): garis bagi sudut &lt;ABC


  circleWithCenter (A, r): lingkaran dengan pusat A dan jari-jari r


  getCircleCenter(c):  pusat lingkaran c


  getCircleRadius(c):  jari-jari lingkaran c


  circleThrough(A,B,C):  lingkaran melalui A, B, C


  middlePerpendicular(A, B): titik tengah AB


  lineCircleIntersections(g, c): titik potong garis g dan lingkran c


  circleCircleIntersections (c1, c2):  titik potong lingkaran c1 dan
c2


  planeThrough(A, B, C):  bidang melalui titik A, B, C


Fungsi-fungsi Khusus Untuk Geometri Simbolik:


  getLineEquation (g,x,y): persamaan garis g dinyatakan dalam x dan y  
  getHesseForm (g,x,y,A): bentuk Hesse garis g dinyatakan dalam x dan  

y dengan titik A pada


  sisi positif (kanan/atas) garis


  quad(A,B): kuadrat jarak AB


  spread(a,b,c): Spread segitiga dengan panjang sisi-sisi a,b,c, yakni
sin(alpha)^2 dengan


  alpha sudut yang menghadap sisi a.


  crosslaw(a,b,c,sa): persamaan 3 quads dan 1 spread pada segitiga
dengan panjang sisi a, b, c.


  triplespread(sa,sb,sc): persamaan 3 spread sa,sb,sc yang memebntuk
suatu segitiga


  doublespread(sa): Spread sudut rangkap Spread 2*phi, dengan
sa=sin(phi)^2 spread a.


## Contoh 1: Luas, Lingkaran Luar, Lingkaran Dalam Segitiga

Untuk menggambar objek-objek geometri, langkah pertama adalah
menentukan rentang sumbu-sumbu koordinat. Semua objek geometri akan
digambar pada satu bidang koordinat, sampai didefinisikan bidang
koordinat yang baru.


\>setPlotRange(-0.5,2.5,-0.5,2.5): // mendefinisikan bidang koordinat baru 


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-481.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-481.png)

Sekarang tetapkan tiga titik dan plotlah.


\>A=[1,0]; plotPoint(A,"A"): // definisi dan gambar tiga titik


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-482.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-482.png)

\>B=[0,1]; plotPoint(B,"B"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-483.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-483.png)

\>C=[2,2]; plotPoint(C,"C"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-484.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-484.png)

Lalu tiga segmen.


\>plotSegment(A,B,"c"): // c=AB


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-485.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-485.png)

\>plotSegment(B,C,"a"): // a=BC


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-486.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-486.png)

\>plotSegment(A,C,"b"): // b=AC


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-487.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-487.png)

Fungsi geometri mencakup fungsi untuk membuat garis dan lingkaran.
Format untuk garis adalah [a,b,c], yang merepresentasikan garis dengan
persamaan ax+by=c.


\>lineThrough(B,C) // garis yang melalui B dan C


    [-1,  2,  2]

Hitunglah garis tegak lurus melalui A pada BC.


\>h=perpendicular(A,lineThrough(B,C)): // garis h tegak lurus BC melalui A


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-488.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-488.png)

Dan persimpangannya dengan BC.


\>D=lineIntersection(h,lineThrough(B,C)): // D adalah titik potong h dan BC


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-489.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-489.png)

Gambarkan itu.


\>plotPoint(D,value=1): // koordinat D ditampilkan


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-490.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-490.png)

\>aspect(1); plotSegment(A,D): // tampilkan semua gambar hasil plot...()


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-491.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-491.png)

Hitung luas ABC:


\>norm(A-D)\*norm(B-C)/2 // AD=norm(A-D), BC=norm(B-C)


    1.5

Compare with determinant formula.


\>areaTriangle(A,B,C) // hitung luas segitiga langusng dengan fungsi


    1.5

Cara lain menghitung luas segitigas ABC:


\>distance(A,D)\*distance(B,C)/2


    1.5

Sudut di C.


\>degprint(computeAngle(B,C,A))


    36°52'11.63''

Sekarang lingkaran luar segitiga.


\>c=circleThrough(A,B,C): // lingkaran luar segitiga ABC


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-492.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-492.png)

\>R=getCircleRadius(c): // jari2 lingkaran luar 


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-493.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-493.png)

\>O=getCircleCenter(c): // titik pusat lingkaran c


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-494.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-494.png)

\>plotPoint(O,"O"): // gambar titik "O"


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-495.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-495.png)

\>plotCircle(c,"Lingkaran luar segitiga ABC"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-496.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-496.png)

Tampilkan koordinat titik pusat dan jari-jari lingkaran luar.


\>O, R


    [1.16667,  1.16667]
    1.17851130198

Sekarang akan digambar lingkaran dalam segitiga ABC. Titik pusat
lingkaran dalam adalah titik potong garis-garis bagi sudut.


\>l=angleBisector(A,C,B): // garis bagi <ACB


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-497.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-497.png)

\>g=angleBisector(C,A,B): // garis bagi <CAB


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-498.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-498.png)

\>P=lineIntersection(l,g) // titik potong kedua garis bagi sudut


    [0.86038,  0.86038]

Tambahkan semuanya ke dalam alur cerita.


\>color(5); plotLine(l); plotLine(g); color(1): // gambar kedua garis bagi sudut


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-499.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-499.png)

\>plotPoint(P,"P"): // gambar titik potongnya


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-500.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-500.png)

\>r=norm(P-projectToLine(P,lineThrough(A,B))) // jari-jari lingkaran dalam


    0.509653732104

\>plotCircle(circleWithCenter(P,r),"Lingkaran dalam segitiga ABC"): // gambar lingkaran dalam


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-501.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-501.png)

## Latihan

1. Tentukan ketiga titik singgung lingkaran dalam dengan sisi-sisi
segitiga ABC.


\>setPlotRange(-2.5,4.5,-2.5,4.5); A=[-2,1]; plotPoint(A,"A");...  
\>   B=[1,-2]; plotPoint(B,"B"); C=[4,4]; plotPoint(C,"C"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-502.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-502.png)

2. Gambar segitiga dengan titik-titik sudut ketiga titik singgung
tersebut.


\>plotSegment(A,B,"c"); plotSegment(B,C,"a"); plotSegment(A,C,"b");...  
\>   aspect(1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-503.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-503.png)

3. Tunjukkan bahwa garis bagi sudut yang ke tiga juga melalui titik
pusat lingkaran dalam.


\>l=angleBisector(A,C,B); g=angleBisector(C,A,B) 


    [1.25658,  7.74342,  5.23025]

\>P=lineIntersection(l,g)


    [0.581139,  0.581139]

\>color(5); plotLine(l); plotLine(g); color(1); plotPoint(P,"P"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-504.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-504.png)

\>r=norm(P-projectToLine(P,lineThrough(A,B)))


    1.52896119631

\>plotCircle(circleWithCenter(P,r),"Lingkaran dalam segitiga ABC"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-505.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-505.png)

Jadi, terbukti bahwa garis bagi sudut yang ketiga juga melalui titik
pusat lingkaran dalam.


4. Gambar jari-jari lingkaran dalam.


\>r=norm(P-projectToLine(P,lineThrough(A,B)))


    1.52896119631

\>plotCircle(circleWithCenter(P,r),"Lingkaran dalam segitiga ABC"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-506.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-506.png)

# Contoh 2: Geometri Smbolik

Kita dapat menghitung geometri eksak dan simbolik menggunakan Maxima.


File geometry.e menyediakan fungsi yang sama (dan lebih banyak lagi)
di Maxima. Akan tetapi, kita sekarang dapat menggunakan perhitungan
simbolik.


\>A &= [1,0]; B &= [0,1]; C &= [2,2]; // menentukan tiga titik A, B, C


Fungsi untuk garis dan lingkaran bekerja seperti fungsi Euler, tetapi
menyediakan perhitungan simbolis.


\>c &= lineThrough(B,C) // c=BC


    
                                 [- 1, 2, 2]
    

Kita dapat memperoleh persamaan garis dengan mudah.


\>$getLineEquation(c,x,y), $solve(%,y) | expand // persamaan garis c


$$2\,y-x=2$$$$\left[ y=\frac{x}{2}+1 \right] $$\>$getLineEquation(lineThrough([x1,y1],[x2,y2]),x,y), $solve(%,y) // persamaan garis melalui(x1, y1) dan (x2, y2)


$$x\,\left({\it y_1}-{\it y_2}\right)+\left(\frac{\sqrt{5}-1}{2}-
 {\it x_1}\right)\,y={\it x_1}\,\left({\it y_1}-{\it y_2}\right)+
 \left(\frac{\sqrt{5}-1}{2}-{\it x_1}\right)\,{\it y_1}$$$$\left[ y=\frac{\left(2\,{\it x_1}-2\,x\right)\,{\it y_2}+\left(2\,x
 -\sqrt{5}+1\right)\,{\it y_1}}{2\,{\it x_1}-\sqrt{5}+1} \right] $$\>$getLineEquation(lineThrough(A,[x1,y1]),x,y) // persamaan garis melalui A dan (x1, y1)


$$\left({\it x_1}-1\right)\,y-x\,{\it y_1}=-{\it y_1}$$\>h &= perpendicular(A,lineThrough(B,C)) // h melalui A tegak lurus BC


    
                                  [2, 1, 2]
    

\>Q &= lineIntersection(c,h) // Q titik potong garis c=BC dan h


    
                                     2  6
                                    [-, -]
                                     5  5
    

\>$projectToLine(A,lineThrough(B,C)) // proyeksi A pada BC


$$\left[ \frac{2}{5} , \frac{6}{5} \right] $$\>$distance(A,Q) // jarak AQ


$$\frac{3}{\sqrt{5}}$$\>cc &= circleThrough(A,B,C); $cc // (titik pusat dan jari-jari) lingkaran melalui A, B, C


$$\left[ \frac{7}{6} , \frac{7}{6} , \frac{5}{3\,\sqrt{2}} \right] $$\>r&=getCircleRadius(cc); $r , $float(r) // tampilkan nilai jari-jari


$$\frac{5}{3\,\sqrt{2}}$$$$1.178511301977579$$\>$computeAngle(A,C,B) // nilai <ACB


$$\arccos \left(\frac{4}{5}\right)$$\>$solve(getLineEquation(angleBisector(A,C,B),x,y),y)[1] // persamaan garis bagi <ACB


$$y=x$$\>P &= lineIntersection(angleBisector(A,C,B),angleBisector(C,B,A)); $P // titik potong 2 garis bagi sudut


$$\left[ \frac{\sqrt{2}\,\sqrt{5}+2}{6} , \frac{\sqrt{2}\,\sqrt{5}+2
 }{6} \right] $$\>P() // hasilnya sama dengan perhitungan sebelumnya


    [0.86038,  0.86038]

## Garis dan Lingkaran yang Berpotongan

Tentu saja, kita juga dapat membuat garis berpotongan dengan
lingkaran, dan lingkaran dengan lingkaran.


\>A &:= [1,0]; c=circleWithCenter(A,4)


    [1,  0,  4]

\>B &:= [1,2]; C &:= [2,1]; l=lineThrough(B,C)


    [1,  1,  3]

\>setPlotRange(5); plotCircle(c); plotLine(l):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-520.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-520.png)

Perpotongan garis dengan lingkaran menghasilkan dua titik dan jumlah
titik perpotongan.


\>a{P1,P2,f}&=lineCircleIntersections(l,c):


    } missing!
    Error in:
    a{P1,P2,f}&amp;=lineCircleIntersections(l,c): ...
           ^

\>P1, P2, f


    Variable P1 not found!
    Error in:
    P1, P2, f ...
      ^

\>plotPoint(P1); plotPoint(P2):


    Variable or function P1 not found.
    Error in:
    plotPoint(P1); plotPoint(P2): ...
                ^

Sama halnya di Maxima.


\>c &= circleWithCenter(A,4) // lingkaran dengan pusat A jari-jari 4


    
                                  [1, 0, 4]
    

\>l &= lineThrough(B,C) // garis l melalui B dan C


    
                                  [1, 1, 3]
    

\>$lineCircleIntersections(l,c) | radcan, // titik potong lingkaran c dan garis l


$$\left[ \left[ \sqrt{7}+2 , 1-\sqrt{7} \right]  , \left[ 2-\sqrt{7}
  , \sqrt{7}+1 \right]  \right] $$Akan ditunjukkan bahwa sudut-sudut yang menghadap bsuusr yang sama
adalah sama besar.


\>C=A+normalize([-2,-3])\*4; plotPoint(C); plotSegment(P1,C); plotSegment(P2,C):


    Variable or function P1 not found.
    Error in:
    ... ormalize([-2,-3])*4; plotPoint(C); plotSegment(P1,C); plotSegm ...
                                                         ^

\>degprint(computeAngle(P1,C,P2))


    Variable or function P1 not found.
    Error in:
    degprint(computeAngle(P1,C,P2)) ...
                            ^

\>C=A+normalize([-4,-3])\*4; plotPoint(C); plotSegment(P1,C); plotSegment(P2,C):


    Variable or function P1 not found.
    Error in:
    ... ormalize([-4,-3])*4; plotPoint(C); plotSegment(P1,C); plotSegm ...
                                                         ^

\>degprint(computeAngle(P1,C,P2))


    Variable or function P1 not found.
    Error in:
    degprint(computeAngle(P1,C,P2)) ...
                            ^

\>insimg;


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-522.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-522.png)

## Garis Sumbu

Berikut adalah langkah-langkah menggambar garis sumbu ruas garis AB:


1. Gambar lingkaran dengan pusat A melalui B.


2. Gambar lingkaran dengan pusat B melalui A.


3. Tarik garis melallui kedua titik potong kedua lingkaran tersebut.
Garis ini merupakan garis sumbu (melalui titik tengah dan tegak lurus)
AB.


\>A=[2,2]; B=[-1,-2];

\>c1=circleWithCenter(A,distance(A,B));

\>c2=circleWithCenter(B,distance(A,B));

\>{P1,P2,f}=circleCircleIntersections(c1,c2);

\>l=lineThrough(P1,P2);

\>setPlotRange(5); plotCircle(c1); plotCircle(c2):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-523.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-523.png)

\>plotPoint(A); plotPoint(B); plotSegment(A,B); plotLine(l):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-524.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-524.png)

Selanjutnya, kita melakukan hal yang sama di Maxima dengan koordinat
umum.


\>A &= [a1,a2]; B &= [b1,b2];

\>c1 &= circleWithCenter(A,distance(A,B));

\>c2 &= circleWithCenter(B,distance(A,B));

\>P &= circleCircleIntersections(c1,c2); P1 &= P[1]; P2 &= P[2];


Persamaan untuk perpotongan cukup rumit. Namun, kita dapat
menyederhanakannya, jika kita mencari nilai y.


\>g &= getLineEquation(lineThrough(P1,P2),x,y);

\>$solve(g,y)


$$\left[ y=\frac{-\left(2\,{\it b_1}-2\,{\it a_1}\right)\,x+{\it b_2}
 ^2+{\it b_1}^2-{\it a_2}^2-{\it a_1}^2}{2\,{\it b_2}-2\,{\it a_2}}
  \right] $$Ini memang sama dengan tegak lurus tengah, yang dihitung dengan cara
yang sepenuhnya berbeda.


\>$solve(getLineEquation(middlePerpendicular(A,B),x,y),y)


$$\left[ y=\frac{-\left(2\,{\it b_1}-2\,{\it a_1}\right)\,x+{\it b_2}
 ^2+{\it b_1}^2-{\it a_2}^2-{\it a_1}^2}{2\,{\it b_2}-2\,{\it a_2}}
  \right] $$\>h &=getLineEquation(lineThrough(A,B),x,y);

\>$solve(h,y)


$$\left[ y=\frac{\left({\it b_2}-{\it a_2}\right)\,x-{\it a_1}\,
 {\it b_2}+{\it a_2}\,{\it b_1}}{{\it b_1}-{\it a_1}} \right] $$Perhatikan hasil kali gradien garis g dan h adalah:


Artinya kedua garis tegak lurus.


\> 


# Contoh 3: Rumus Heron

Rumus Heron menyatakan bahwa luas segitiga dengan panjang sisi-sisi a,
b dan c adalah:


atau bisa ditulis dalam bentuk lain:


Untuk membuktikan hal ini kita misalkan C(0,0), B(a,0) dan A(x,y),
b=AC, c=AB. Luas segitiga ABC adalah


Nilai y didapat dengan menyelesaikan sistem persamaan:


\>setPlotRange(-1,10,-1,8); plotPoint([0,0], "C(0,0)"); plotPoint([5.5,0], "B(a,0)");  ...  
\>   plotPoint([7.5,6], "A(x,y)"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-528.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-528.png)

\>plotSegment([0,0],[5.5,0], "a",25); plotSegment([5.5,0],[7.5,6],"c",15);  ...  
\>   plotSegment([0,0],[7.5,6],"b",25):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-529.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-529.png)

\>plotSegment([7.5,6],[7.5,0],"t=y",25):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-530.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-530.png)

\>&assume(a\>0); sol &= solve([x^2+y^2=b^2,(x-a)^2+y^2=c^2],[x,y])


    
                                      []
    

Ekstrak solusi y.


\>ysol &= y with sol[2][2]; $'y=sqrt(factor(ysol^2))


    Maxima said:
    part: invalid index of list or matrix.
     -- an error. To debug this try: debugmode(true);
    
    Error in:
    ysol &amp;= y with sol[2][2]; $'y=sqrt(factor(ysol^2)) ...
                            ^

Kita mendapatkan rumus Heron.


\>function H(a,b,c) &= sqrt(factor((ysol\*a/2)^2)); $'H(a,b,c)=H(a,b,c)


$$H\left(a , b , \left[ 1 , 0 , 4 \right] \right)=\frac{a\,\left| 
 {\it ysol}\right| }{2}$$\>$'Luas=H(2,5,6) // luas segitiga dengan panjang sisi-sisi 2, 5, 6


$${\it Luas}=\left| {\it ysol}\right| $$Tentu saja, setiap segitiga siku-siku adalah kasus yang terkenal.


\>H(3,4,5) //luas segitiga siku-siku dengan panjang sisi 3, 4, 5


    Variable or function ysol not found.
    Try "trace errors" to inspect local variables after errors.
    H:
        useglobal; return a*abs(ysol)/2 
    Error in:
    H(3,4,5) //luas segitiga siku-siku dengan panjang sisi 3, 4, 5 ...
            ^

Dan jelas pula, bahwa ini adalah segitiga dengan luas maksimal dan dua
sisinya 3 dan 4.


\>aspect (1.5); plot2d(&H(3,4,x),1,7): // Kurva luas segitiga sengan panjang sisi 3, 4, x (1<= x <=7)//


    Variable or function ysol not found.
    Error in expression: 3*abs(ysol)/2
    %ploteval:
        y0=f$(x[1],args());
    adaptiveevalone:
        s=%ploteval(g$,t;args());
    Try "trace errors" to inspect local variables after errors.
    plot2d:
        dw/n,dw/n^2,dw/n,auto;args());

Kasus umum juga berfungsi.


\>$solve(diff(H(a,b,c)^2,c)=0,c)mxb


    Maxima said:
    incorrect syntax: mxb is not an infix operator
    a,b,c)^2,c)=0,c)mxb;
                      ^
    
    Error in:
    $solve(diff(H(a,b,c)^2,c)=0,c)mxb ...
                                     ^

Sekarang mari kita cari himpunan semua titik di mana b+c=d untuk suatu
konstanta d. Diketahui bahwa ini adalah elips.


\>s1 &= subst(d-c,b,sol[2]); $s1


    Maxima said:
    part: invalid index of list or matrix.
     -- an error. To debug this try: debugmode(true);
    
    Error in:
    s1 &amp;= subst(d-c,b,sol[2]); $s1 ...
                             ^

Dan buat fungsi ini.


\>function fx(a,c,d) &= rhs(s1[1]); $fx(a,c,d), function fy(a,c,d) &= rhs(s1[2]); $fy(a,c,d)


$$0$$$$0$$Sekarang kita dapat menggambar himpunannya. Sisi b bervariasi dari 1
hingga 4. Diketahui bahwa kita mendapatkan elips.


\>aspect(1); plot2d(&fx(3,x,5),&fy(3,x,5),xmin=1,xmax=4,square=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-535.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-535.png)

Kita dapat memeriksa persamaan umum untuk elips ini, yaitu:


di mana (xm,ym) adalah pusat, dan u dan v adalah sumbu setengah.


\>$ratsimp((fx(a,c,d)-a/2)^2/u^2+fy(a,c,d)^2/v^2 with [u=d/2,v=sqrt(d^2-a^2)/2])


$$\left[ \frac{a^2}{d^2} , \frac{a^2}{d^2} , \frac{a^2}{d^2} , \frac{
 a^2}{d^2} , \frac{a^2}{d^2} , \frac{a^2}{d^2} , \frac{a^2}{d^2} , 
 \frac{a^2}{d^2} , \frac{a^2}{d^2} , \frac{a^2}{d^2} , \frac{a^2}{d^2
 } \right] $$Kita melihat bahwa tinggi dan luas segitiga tersebut adalah maksimum
untuk x=0. Jadi luas segitiga dengan a+b+c=d adalah maksimum, jika
segitiga tersebut sama sisi. Kita ingin memperolehnya secara analitis.


\>eqns &= [diff(H(a,b,d-(a+b))^2,a)=0,diff(H(a,b,d-(a+b))^2,b)=0]; $eqns


$$\left[ \frac{a\,{\it ysol}^2}{2}=0 , 0=0 \right] $$Kita memperoleh beberapa nilai minimum, yang dimiliki oleh segitiga
dengan satu sisi 0, dan solusinya a=b=c=d/3.


\>$solve(eqns,[a,b])


$$\left[ \left[ a=0 , b={\it \%r_1} \right]  \right] $$\>&solve([diff(H(a,b,c)^2,a)=la,diff(H(a,b,c)^2,b)=la, ...  
\>      diff(H(a,b,c)^2,c)=la,a+b+c=d],[a,b,c,la])


    Maxima said:
    diff: second argument must be a variable; found [1,0,4]
     -- an error. To debug this try: debugmode(true);
    
    Error in:
    ... la,    diff(H(a,b,c)^2,c)=la,a+b+c=d],[a,b,c,la]) ...
                                                         ^

Kita bisa membuat plot dari situasinya


Pertama-tama atur titik di Maxima.


\>A &= at([x,y],sol[2]); $A


    Maxima said:
    part: invalid index of list or matrix.
     -- an error. To debug this try: debugmode(true);
    
    Error in:
    A &amp;= at([x,y],sol[2]); $A ...
                         ^

\>B &= [0,0]; $B, C &= [a,0]; $C


$$\left[ 0 , 0 \right] $$$$\left[ a , 0 \right] $$Kemudian atur rentang plot dan plot titik-titiknya.


\>setPlotRange(0,5,-2,3); ...  
\>   a=4; b=3; c=2; ...  
\>   plotPoint(mxmeval("B"),"B"); plotPoint(mxmeval("C"),"C"); ...  
\>   plotPoint(mxmeval("A"),"A"):


    Variable a1 not found!
    Use global variables or parameters for string evaluation.
    Error in Evaluate, superfluous characters found.
    Try "trace errors" to inspect local variables after errors.
    mxmeval:
        return evaluate(mxm(s));
    Error in:
    ... otPoint(mxmeval("C"),"C"); plotPoint(mxmeval("A"),"A"): ...
                                                         ^

Plot segmen.


\>splotSegment(mxmeval("A"),mxmeval("C")); ...  
\>   plotSegment(mxmeval("B"),mxmeval("C")); ...  
\>   plotSegment(mxmeval("B"),mxmeval("A")):


    Variable a1 not found!
    Use global variables or parameters for string evaluation.
    Error in Evaluate, superfluous characters found.
    Try "trace errors" to inspect local variables after errors.
    mxmeval:
        return evaluate(mxm(s));
    Error in:
    splotSegment(mxmeval("A"),mxmeval("C")); plotSegment(mxmeval(" ...
                             ^

Hitunglah garis tegak lurus tengah di Maxima.


\>h &= middlePerpendicular(A,B); g &= middlePerpendicular(B,C);


Dan pusat kelilingnya.


\>U &= lineIntersection(h,g);


Kita mendapatkan rumus untuk jari-jari lingkaran luar.


\>&assume(a\>0,b\>0,c\>0); $distance(U,B) | radcan


$$\frac{\sqrt{{\it a_2}^2+{\it a_1}^2}\,\sqrt{{\it a_2}^2+{\it a_1}^2
 -2\,a\,{\it a_1}+a^2}}{2\,\left| {\it a_2}\right| }$$Mari kita tambahkan ini ke dalam alur cerita.


\>plotPoint(U()); ...  
\>   plotCircle(circleWithCenter(mxmeval("U"),mxmeval("distance(U,C)"))):


    Variable a2 not found!
    Use global variables or parameters for string evaluation.
    Error in ^
    Error in expression: [a/2,(a2^2+a1^2-a*a1)/(2*a2)]
    Error in:
    plotPoint(U()); plotCircle(circleWithCenter(mxmeval("U"),mxmev ...
                 ^

Dengan menggunakan geometri, kita peroleh rumus sederhana


untuk jari-jari. Kita dapat memeriksa apakah ini benar dengan Maxima.
Maxima akan memfaktorkan ini hanya jika kita mengkuadratkannya.


\>$c^2/sin(computeAngle(A,B,C))^2  | factor


$$\left[ \frac{{\it a_2}^2+{\it a_1}^2}{{\it a_2}^2} , 0 , \frac{16\,
 \left({\it a_2}^2+{\it a_1}^2\right)}{{\it a_2}^2} \right] $$# Contoh 4: Garis Euler dan Parabola

Garis Euler adalah garis yang ditentukan dari sembarang segitiga yang
tidak sama sisi. Garis ini merupakan garis pusat segitiga, dan
melewati beberapa titik penting yang ditentukan dari segitiga
tersebut, termasuk orthocenter, circumcenter, centroid, titik Exeter,
dan titik pusat lingkaran sembilan titik pada segitiga tersebut.


Sebagai contoh, kita hitung dan plot garis Euler dalam sebuah
segitiga.


Pertama, kita definisikan sudut-sudut segitiga dalam Euler. Kita
gunakan definisi, yang terlihat dalam ekspresi simbolik.


\>A::=[-1,-1]; B::=[2,0]; C::=[1,2];


Untuk memplot objek geometris, kita menyiapkan area plot, dan
menambahkan titik-titik ke dalamnya. Semua plot objek geometris
ditambahkan ke plot saat ini.


\>setPlotRange(3); plotPoint(A,"A"); plotPoint(B,"B"); plotPoint(C,"C");


Kita juga dapat menambahkan sisi-sisi segitiga.


\>plotSegment(A,B,""); plotSegment(B,C,""); plotSegment(C,A,""):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-543.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-543.png)

Berikut adalah luas segitiga, menggunakan rumus determinan. Tentu
saja, kita harus mengambil nilai absolut dari hasil ini.


\>$areaTriangle(A,B,C)


$$-\frac{7}{2}$$Kita dapat menghitung koefisien sisi c.


\>c &= lineThrough(A,B)


    
                                [- 1, 3, - 2]
    

Dan dapatkan juga rumus untuk garis ini.


\>$getLineEquation(c,x,y)


$$3\,y-x=-2$$Untuk bentuk Hesse, kita perlu menentukan suatu titik, sehingga titik
tersebut berada di sisi positif bentuk Hesse. Memasukkan titik akan
menghasilkan jarak positif ke garis.


\>$getHesseForm(c,x,y,C), $at(%,[x=C[1],y=C[2]])


$$\frac{3\,y-x+2}{\sqrt{10}}$$$$\frac{7}{\sqrt{10}}$$Sekarang kita hitung lingkaran luar ABC.


\>LL &= circleThrough(A,B,C); $getCircleEquation(LL,x,y)


$$\left(y-\frac{5}{14}\right)^2+\left(x-\frac{3}{14}\right)^2=\frac{
 325}{98}$$\>O &= getCircleCenter(LL); $O


$$\left[ \frac{3}{14} , \frac{5}{14} \right] $$Gambarkan lingkaran dan titik pusatnya. Cu dan U adalah simbol. Kita
evaluasi ekspresi ini untuk Euler.


\>plotCircle(LL()); plotPoint(O(),"O"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-550.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-550.png)

Kita dapat menghitung perpotongan tinggi di ABC (orthocenter) secara
numerik dengan perintah berikut.


\>H &= lineIntersection(perpendicular(A,lineThrough(C,B)),...  
\>    perpendicular(B,lineThrough(A,C))); $H


$$\left[ \frac{11}{7} , \frac{2}{7} \right] $$Sekarang kita dapat menghitung garis Euler dari segitiga tersebut.


\>el &= lineThrough(H,O); $getLineEquation(el,x,y)


$$-\frac{19\,y}{14}-\frac{x}{14}=-\frac{1}{2}$$Tambahkan ke plot kita.


\>plotPoint(H(),"H"); plotLine(el(),"Garis Euler"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-553.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-553.png)

Pusat gravitasi seharusnya berada pada garis ini.


\>M &= (A+B+C)/3; $getLineEquation(el,x,y) with [x=M[1],y=M[2]]


$$-\frac{1}{2}=-\frac{1}{2}$$\>plotPoint(M(),"M"): // titik berat


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-555.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-555.png)

Teori ini memberi tahu kita MH=2*MO. Kita perlu menyederhanakannya
dengan radcan untuk mencapainya.


\>$distance(M,H)/distance(M,O)|radcan


$$2$$Fungsinya termasuk fungsi untuk sudut juga.


\>$computeAngle(A,C,B), degprint(%())


$$\arccos \left(\frac{4}{\sqrt{5}\,\sqrt{13}}\right)$$    60°15'18.43''

Persamaan untuk pusat lingkaran dalam tidak terlalu bagus.


\>Q &= lineIntersection(angleBisector(A,C,B),angleBisector(C,B,A))|radcan; $Q


$$\left[ \frac{\left(2^{\frac{3}{2}}+1\right)\,\sqrt{5}\,\sqrt{13}-15
 \,\sqrt{2}+3}{14} , \frac{\left(\sqrt{2}-3\right)\,\sqrt{5}\,\sqrt{
 13}+5\,2^{\frac{3}{2}}+5}{14} \right] $$Mari kita hitung juga ekspresi untuk jari-jari lingkaran dalam.


\>r &= distance(Q,projectToLine(Q,lineThrough(A,B)))|ratsimp; $r


$$\frac{\sqrt{\left(-41\,\sqrt{2}-31\right)\,\sqrt{5}\,\sqrt{13}+115
 \,\sqrt{2}+614}}{7\,\sqrt{2}}$$\>LD &=  circleWithCenter(Q,r); // Lingkaran dalam


Mari kita tambahkan ini ke dalam alur cerita.


\>color(5); plotCircle(LD()):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-560.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-560.png)

## Parabola

Selanjutnya akan dicari persamaan tempat kedudukan titik-titik yang
berjarak sama ke titik C dan ke garis AB.


\>p &= getHesseForm(lineThrough(A,B),x,y,C)-distance([x,y],C); $p='0


$$\frac{3\,y-x+2}{\sqrt{10}}-\sqrt{\left(2-y\right)^2+\left(1-x
 \right)^2}=0$$Persamaan tersebut dapat digambar menjadi satu dengan gambar
sebelumnya.


\>plot2d(p,level=0,add=1,contourcolor=6):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-562.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-562.png)

Ini seharusnya merupakan suatu fungsi, tetapi penyelesai default
Maxima hanya dapat menemukan solusinya, jika kita mengkuadratkan
persamaannya. Akibatnya, kita mendapatkan solusi palsu.


\>akar &= solve(getHesseForm(lineThrough(A,B),x,y,C)^2-distance([x,y],C)^2,y)


    
             [y = - 3 x - sqrt(70) sqrt(9 - 2 x) + 26, 
                                  y = - 3 x + sqrt(70) sqrt(9 - 2 x) + 26]
    

Solusi pertama adalah


maxima: akar[1]


Dengan menambahkan solusi pertama ke dalam plot, terlihat bahwa itu
memang jalur yang kita cari. Teori tersebut memberi tahu kita bahwa
itu adalah parabola yang diputar.


\>plot2d(&rhs(akar[1]),add=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-563.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-563.png)

\>function g(x) &= rhs(akar[1]); $'g(x)= g(x)// fungsi yang mendefinisikan kurva di atas


$$g\left(x\right)=-3\,x-\sqrt{70}\,\sqrt{9-2\,x}+26$$\>T &=[-1, g(-1)]; // ambil sebarang titik pada kurva tersebut

\>dTC &= distance(T,C); $fullratsimp(dTC), $float(%) // jarak T ke C


$$\sqrt{1503-54\,\sqrt{11}\,\sqrt{70}}$$$$2.135605779339061$$\>U &= projectToLine(T,lineThrough(A,B)); $U // proyeksi T pada garis AB 


$$\left[ \frac{80-3\,\sqrt{11}\,\sqrt{70}}{10} , \frac{20-\sqrt{11}\,
 \sqrt{70}}{10} \right] $$Ternyata jarak T ke C sama dengan jarak T ke AB. Coba Anda pilih titik


\>dU2AB &= distance(T,U); $fullratsimp(dU2AB), $float(%) // jatak T ke AB


$$\sqrt{1503-54\,\sqrt{11}\,\sqrt{70}}$$$$2.135605779339061$$Ternyata jarak T ke C sama dengan jarak T ke AB. Coba Anda pilih titik
T yang lain dan ulangi perhitungan-perhitungan di atas untuk
menunjukkan bahwa hasilnya juga sama.


# Contoh 5: Trigonometri Rasional

Hal ini terinspirasi dari ceramah N.J.Wildberger. Dalam bukunya
"Divine Proportions", Wildberger mengusulkan untuk mengganti konsep
klasik jarak dan sudut dengan kuadran dan sebaran. Dengan menggunakan
konsep ini, memang memungkinkan untuk menghindari fungsi trigonometri
dalam banyak contoh, dan tetap "rasional".


Berikut ini, saya memperkenalkan konsep-konsep tersebut, dan
memecahkan beberapa masalah. Saya menggunakan perhitungan simbolik
Maxima di sini, yang menyembunyikan keuntungan utama trigonometri
rasional bahwa perhitungan dapat dilakukan hanya dengan kertas dan
pensil. Anda diundang untuk memeriksa hasilnya tanpa komputer.


Intinya adalah bahwa perhitungan simbolik rasional sering kali
menghasilkan hasil yang sederhana. Sebaliknya, trigonometri klasik
menghasilkan hasil trigonometri yang rumit, yang hanya mengevaluasi
perkiraan numerik.


\>load geometry;


Untuk pengenalan pertama, kami menggunakan segitiga siku-siku dengan
proporsi Mesir yang terkenal yaitu 3, 4, dan 5. Perintah berikut
adalah perintah Euler untuk memplot geometri bidang yang terdapat
dalam file Euler "geometry.e".


\>C&:=[0,0]; A&:=[4,0]; B&:=[0,3]; ...  
\>   setPlotRange(-1,5,-1,5); ...  
\>   plotPoint(A,"A"); plotPoint(B,"B"); plotPoint(C,"C"); ...  
\>   plotSegment(B,A,"c"); plotSegment(A,C,"b"); plotSegment(C,B,"a"); ...  
\>   insimg(30);


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-570.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-570.png)

Tentu saja,


di mana wa adalah sudut di A. Cara yang biasa untuk menghitung sudut
ini adalah dengan mengambil kebalikan dari fungsi sinus. Hasilnya
adalah sudut yang tidak dapat dicerna, yang hanya dapat dicetak secara
perkiraan.


\>wa := arcsin(3/5); degprint(wa)


    36°52'11.63''

Trigonometri rasional mencoba menghindari hal ini.


Gagasan pertama trigonometri rasional adalah kuadran, yang
menggantikan jarak. Faktanya, itu hanyalah kuadrat jarak. Dalam
persamaan berikut, a, b, dan c menunjukkan kuadran sisi-sisi.


Teorema Pythogoras menjadi a+b=c.


\>a &= 3^2; b &= 4^2; c &= 5^2; &a+b=c


    
                                   25 = 25
    

Gagasan kedua trigonometri rasional adalah sebaran. Sebaran mengukur
bukaan antara garis. Nilainya 0, jika garis sejajar, dan 1, jika garis
persegi panjang. Nilainya adalah kuadrat sinus sudut antara dua garis.


Sebaran garis AB dan AC pada gambar di atas didefinisikan sebagai


di mana a dan c adalah kuadran dari setiap segitiga persegi panjang
dengan satu sudut di A.


\>sa &= a/c; $sa


$$\frac{9}{25}$$Tentu saja, ini lebih mudah dihitung daripada sudut. Namun, Anda
kehilangan sifat bahwa sudut dapat ditambahkan dengan mudah.


Tentu saja, kita dapat mengubah nilai perkiraan untuk sudut wa menjadi
sprad, dan mencetaknya sebagai pecahan.


\>fracprint(sin(wa)^2)


    9/25

Hukum kosinus dari trgonometri klasik diterjemahkan ke dalam "hukum
silang" berikut.


Di sini a, b, dan c adalah kuadran sisi-sisi segitiga, dan sa adalah
sebaran di sudut A. Sisi a, seperti biasa, berseberangan dengan sudut
A.


Hukum-hukum ini diimplementasikan dalam berkas geometry.e yang kami
muat ke Euler.


\>$crosslaw(aa,bb,cc,saa)


$$\left[ \left({\it bb}-{\it aa}+\frac{7}{6}\right)^2 , \left(
 {\it bb}-{\it aa}+\frac{7}{6}\right)^2 , \left({\it bb}-{\it aa}+
 \frac{5}{3\,\sqrt{2}}\right)^2 \right] =\left[ \frac{14\,{\it bb}\,
 \left(1-{\it saa}\right)}{3} , \frac{14\,{\it bb}\,\left(1-{\it saa}
 \right)}{3} , \frac{5\,2^{\frac{3}{2}}\,{\it bb}\,\left(1-{\it saa}
 \right)}{3} \right] $$Dalam kasus kami, kami mendapatkan


\>$crosslaw(a,b,c,sa)


$$1024=1024$$Mari kita gunakan hukum silang ini untuk menemukan sebaran di A. Untuk
melakukannya, kita buat hukum silang untuk kuadran a, b, dan c, dan
selesaikan untuk sebaran yang tidak diketahui sa.


Anda dapat melakukannya dengan mudah secara manual, tetapi saya
menggunakan Maxima. Tentu saja, kita mendapatkan hasil yang sudah kita
miliki.


\>$crosslaw(a,b,c,x), $solve(%,x)


$$1024=1600\,\left(1-x\right)$$$$\left[ x=\frac{9}{25} \right] $$Kita sudah tahu ini. Definisi sebaran adalah kasus khusus dari hukum
silang.


Kita juga dapat memecahkan ini untuk a,b,c umum. Hasilnya adalah rumus
yang menghitung sebaran sudut segitiga yang diberikan kuadran ketiga
sisinya.


\>$solve(crosslaw(aa,bb,cc,x),x)


$$\left[ \left[ \frac{168\,{\it bb}\,x+36\,{\it bb}^2+\left(-72\,
 {\it aa}-84\right)\,{\it bb}+36\,{\it aa}^2-84\,{\it aa}+49}{36} , 
 \frac{168\,{\it bb}\,x+36\,{\it bb}^2+\left(-72\,{\it aa}-84\right)
 \,{\it bb}+36\,{\it aa}^2-84\,{\it aa}+49}{36} , \frac{15\,2^{\frac{
 5}{2}}\,{\it bb}\,x+18\,{\it bb}^2+\left(-36\,{\it aa}-15\,2^{\frac{
 3}{2}}\right)\,{\it bb}+18\,{\it aa}^2-15\,2^{\frac{3}{2}}\,{\it aa}
 +25}{18} \right] =0 \right] $$Kita dapat membuat fungsi dari hasil tersebut. Fungsi tersebut telah
didefinisikan dalam berkas geometry.e milik Euler.


\>$spread(a,b,c)


$$\frac{9}{25}$$Sebagai contoh, kita dapat menggunakannya untuk menghitung sudut
segitiga dengan sisi-sisi


Hasilnya rasional, yang tidak mudah didapat jika kita menggunakan
trigonometri klasik.


\>$spread(a,a,4\*a/7)


$$\frac{6}{7}$$Ini adalah sudut dalam derajat.


\>degprint(arcsin(sqrt(6/7)))


    67°47'32.44''

## Contoh Lain

Sekarang, mari kita coba contoh yang lebih maju.


Kita tentukan tiga sudut segitiga sebagai berikut.


\>A&:=[1,2]; B&:=[4,3]; C&:=[0,4]; ...  
\>   setPlotRange(-1,5,1,7); ...  
\>   plotPoint(A,"A"); plotPoint(B,"B"); plotPoint(C,"C"); ...  
\>   plotSegment(B,A,"c"); plotSegment(A,C,"b"); plotSegment(C,B,"a"); ...  
\>   insimg;


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-579.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-579.png)

Dengan menggunakan Pythogoras, mudah untuk menghitung jarak antara dua
titik. Pertama-tama saya menggunakan fungsi distance dari file Euler
untuk geometri. Fungsi distance menggunakan geometri klasik.


\>$distance(A,B)


$$\sqrt{10}$$Euler juga memuat fungsi untuk kuadran antara dua titik.


Dalam contoh berikut, karena c+b bukan a, segitiga tersebut bukan
persegi panjang.


\>c &= quad(A,B); $c, b &= quad(A,C); $b, a &= quad(B,C); $a,


$$10$$$$5$$$$17$$Pertama, mari kita hitung sudut tradisional. Fungsi computeAngle
menggunakan metode biasa berdasarkan perkalian titik dua vektor.
Hasilnya adalah beberapa perkiraan floating point.


\>wb &= computeAngle(A,B,C); $wb, $(wb/pi\*180)()


$$\arccos \left(\frac{11}{\sqrt{10}\,\sqrt{17}}\right)$$    32.4711922908

Dengan menggunakan pensil dan kertas, kita dapat melakukan hal yang
sama dengan hukum silang. Kita masukkan kuadran a, b, dan c ke dalam
hukum silang dan selesaikan untuk x.


\>$crosslaw(a,b,c,x), $solve(%,x), //(b+c-a)^=4b.c(1-x)


$$4=200\,\left(1-x\right)$$$$\left[ x=\frac{49}{50} \right] $$Yaitu, apa yang dilakukan fungsi sebaran yang didefinisikan dalam
"geometry.e".


\>sb &= spread(b,a,c); $sb


$$\frac{49}{170}$$Maxima memperoleh hasil yang sama dengan menggunakan trigonometri
biasa, jika kita memaksakannya. Maxima memang menyelesaikan suku
sin(arccos(...)) menjadi hasil pecahan. Sebagian besar siswa tidak
dapat melakukan ini.


\>$sin(computeAngle(A,B,C))^2


$$\frac{49}{170}$$Setelah kita memiliki sebaran di B, kita dapat menghitung tinggi ha
pada sisi a. Ingat bahwa


menurut definisi.


\>ha &= c\*sb; $ha


$$\frac{49}{17}$$Gambar berikut ini dibuat dengan program geometri C.a.R., yang dapat
menggambar kuadran dan sebaran.


image: (20) Rational_Geometry_CaR.png


Menurut definisi, panjang ha adalah akar kuadrat dari kuadrannya.


\>$sqrt(ha)


$$\frac{7}{\sqrt{17}}$$Sekarang kita bisa menghitung luas segitiga. Jangan lupa, bahwa kita
sedang membahas tentang kuadran!


\>$sqrt(ha)\*sqrt(a)/2


$$\frac{7}{2}$$Rumus determinan yang biasa menghasilkan hasil yang sama.


\>$areaTriangle(B,A,C)


$$\frac{7}{2}$$## Rumus Heron

Sekarang, mari kita selesaikan masalah ini secara umum!


\>&remvalue(a,b,c,sb,ha);


Pertama-tama kita hitung sebaran di B untuk segitiga dengan sisi a, b,
dan c. Kemudian kita hitung luas kuadrat (yang disebut "quadrea"?),
faktorkan dengan Maxima, dan kita dapatkan rumus Heron yang terkenal.


Memang, ini sulit dilakukan dengan pensil dan kertas.


\>$spread(b^2,c^2,a^2), $factor(%\*c^2\*a^2/4)


$$\frac{-c^4-\left(-2\,b^2-2\,a^2\right)\,c^2-b^4+2\,a^2\,b^2-a^4}{4
 \,a^2\,c^2}$$$$\frac{\left(-c+b+a\right)\,\left(c-b+a\right)\,\left(c+b-a\right)\,
 \left(c+b+a\right)}{16}$$## Aturan Triple Spread

Kerugian spread adalah tidak lagi sekadar menambahkan sudut yang sama.


Namun, tiga spread segitiga memenuhi aturan "triple spread" berikut.


\>&remvalue(sa,sb,sc); $triplespread(sa,sb,sc)


$$\left({\it sc}+{\it sb}+{\it sa}\right)^2=2\,\left({\it sc}^2+
 {\it sb}^2+{\it sa}^2\right)+4\,{\it sa}\,{\it sb}\,{\it sc}$$Aturan ini berlaku untuk tiga sudut yang jumlahnya mencapai 180°.


Karena sebaran


sama, aturan sebaran rangkap tiga juga berlaku, jika


Karena sebaran sudut negatif sama, aturan sebaran rangkap tiga juga
berlaku, jika


Misalnya, kita dapat menghitung sebaran sudut 60°. Yaitu 3/4.
Persamaan tersebut memiliki solusi kedua, di mana semua sebarannya
adalah 0.


\>$solve(triplespread(x,x,x),x)


$$\left[ x=\frac{3}{4} , x=0 \right] $$Sebaran 90° jelas adalah 1. Jika dua sudut dijumlahkan menjadi 90°,
sebarannya memecahkan persamaan sebaran rangkap tiga dengan a,b,1.
Dengan perhitungan berikut kita memperoleh a+b=1.


\>$triplespread(x,y,1), $solve(%,x)


$$\left(y+x+1\right)^2=2\,\left(y^2+x^2+1\right)+4\,x\,y$$$$\left[ x=1-y \right] $$Karena sebaran 180°-t sama dengan sebaran t, rumus sebaran rangkap
tiga juga berlaku, jika satu sudut adalah jumlah atau selisih dari dua
sudut lainnya.


Jadi kita dapat menemukan sebaran sudut yang digandakan. Perhatikan
bahwa ada dua solusi lagi. Kita buat ini menjadi fungsi.


\>$solve(triplespread(a,a,x),x), function doublespread(a) &= factor(rhs(%[1]))


$$\left[ x=4\,a-4\,a^2 , x=0 \right] $$    
                                - 4 (a - 1) a
    

## Garis Bagi Sudut

Kita sudah tahu situasinya seperti ini.


\>C&:=[0,0]; A&:=[4,0]; B&:=[0,3]; ...  
\>   setPlotRange(-1,5,-1,5); ...  
\>   plotPoint(A,"A"); plotPoint(B,"B"); plotPoint(C,"C"); ...  
\>   plotSegment(B,A,"c"); plotSegment(A,C,"b"); plotSegment(C,B,"a"); ...  
\>   insimg;


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-600.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-600.png)

Mari kita hitung panjang garis bagi sudut di A. Namun, kita ingin
menyelesaikannya untuk a,b,c umum.


\>&remvalue(a,b,c);


Jadi pertama-tama kita hitung sebaran sudut yang dibagi dua di A,
menggunakan rumus sebaran rangkap tiga.


Masalah dengan rumus ini muncul lagi. Rumus ini memiliki dua solusi.
Kita harus memilih yang benar. Solusi lainnya mengacu pada sudut yang
dibagi dua 180°-wa.


\>$triplespread(x,x,a/(a+b)), $solve(%,x), sa2 &= rhs(%[1]); $sa2


$$\left(2\,x+\frac{a}{b+a}\right)^2=2\,\left(2\,x^2+\frac{a^2}{\left(
 b+a\right)^2}\right)+\frac{4\,a\,x^2}{b+a}$$$$\left[ x=\frac{-\sqrt{b}\,\sqrt{b+a}+b+a}{2\,b+2\,a} , x=\frac{
 \sqrt{b}\,\sqrt{b+a}+b+a}{2\,b+2\,a} \right] $$$$\frac{-\sqrt{b}\,\sqrt{b+a}+b+a}{2\,b+2\,a}$$Mari kita periksa persegi panjang Mesir.


\>$sa2 with [a=3^2,b=4^2]


$$\frac{1}{10}$$Kita dapat mencetak sudut dalam Euler, setelah mentransfer sebaran ke
radian.


\>wa2 := arcsin(sqrt(1/10)); degprint(wa2)


    18°26'5.82''

Titik P merupakan perpotongan garis bagi sudut dengan sumbu y.


\>P := [0,tan(wa2)\*4]


    [0,  1.33333]

\>plotPoint(P,"P"); plotSegment(A,P):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-605.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-605.png)

Mari kita periksa sudut-sudut pada contoh spesifik kita.


\>computeAngle(C,A,P), computeAngle(P,A,B)


    0.321750554397
    0.321750554397

Sekarang kita hitung panjang garis bagi AP.


Kita gunakan teorema sinus dalam segitiga APC. Teorema ini menyatakan
bahwa


berlaku di sembarang segitiga. Kuadratkan, maka akan menghasilkan apa
yang disebut "hukum sebaran"


di mana a,b,c menunjukkan kuadran.


Karena CPA sebaran adalah 1-sa2, kita peroleh darinya bisa/1=b/(1-sa2)
dan dapat menghitung bisa (kuadran garis bagi sudut).


\>&factor(ratsimp(b/(1-sa2))); bisa &= %; $bisa


$$\frac{2\,b\,\left(b+a\right)}{\sqrt{b}\,\sqrt{b+a}+b+a}$$Mari kita periksa rumus ini untuk nilai-nilai Mesir kita.


\>sqrt(mxmeval("at(bisa,[a=3^2,b=4^2])")), distance(A,P)


    4.21637021356
    4.21637021356

Kita juga dapat menghitung P menggunakan rumus spread.


\>py&=factor(ratsimp(sa2\*bisa)); $py


$$-\frac{b\,\left(\sqrt{b}\,\sqrt{b+a}-b-a\right)}{\sqrt{b}\,\sqrt{b+
 a}+b+a}$$Nilainya sama dengan yang kita dapatkan dengan rumus trigonometri.


\>sqrt(mxmeval("at(py,[a=3^2,b=4^2])"))


    1.33333333333

## Sudut Tali

Perhatikan situasi berikut.


\>setPlotRange(1.2); ...  
\>   color(1); plotCircle(circleWithCenter([0,0],1)); ...  
\>   A:=[cos(1),sin(1)]; B:=[cos(2),sin(2)]; C:=[cos(6),sin(6)]; ...  
\>   plotPoint(A,"A"); plotPoint(B,"B"); plotPoint(C,"C"); ...  
\>   color(3); plotSegment(A,B,"c"); plotSegment(A,C,"b"); plotSegment(C,B,"a"); ...  
\>   color(1); O:=[0,0];  plotPoint(O,"0"); ...  
\>   plotSegment(A,O); plotSegment(B,O); plotSegment(C,O,"r"); ...  
\>   insimg;


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-608.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-608.png)

Kita dapat menggunakan Maxima untuk memecahkan rumus penyebaran
rangkap tiga untuk sudut-sudut di pusat O untuk r. Dengan demikian,
kita memperoleh rumus untuk jari-jari kuadrat pericircle dalam bentuk
kuadran sisi-sisinya.


Kali ini, Maxima menghasilkan beberapa nol kompleks, yang kita
abaikan.


\>&remvalue(a,b,c,r); // hapus nilai-nilai sebelumnya untuk perhitungan baru

\>rabc &= rhs(solve(triplespread(spread(b,r,r),spread(a,r,r),spread(c,r,r)),r)[4]); $rabc


$$-\frac{a\,b\,c}{c^2-2\,b\,c+a\,\left(-2\,c-2\,b\right)+b^2+a^2}$$Kita dapat menjadikannya fungsi Euler.


\>function periradius(a,b,c) &= rabc;


Mari kita periksa hasilnya untuk titik A, B, C.


\>a:=quadrance(B,C); b:=quadrance(A,C); c:=quadrance(A,B);


Radiusnya memang 1.


\>periradius(a,b,c)


    1

Faktanya, sebaran CBA hanya bergantung pada b dan c. Ini adalah
teorema sudut tali busur.


\>$spread(b,a,c)\*rabc | ratsimp


$$\frac{b}{4}$$Faktanya, sebarannya adalah b/(4r), dan kita melihat bahwa sudut tali
busur b adalah setengah sudut pusat.


\>$doublespread(b/(4\*r))-spread(b,r,r) | ratsimp


$$0$$# Contoh 6: Jarak Minimal pada Bidang

## Catatan awal

Fungsi yang, pada titik M di bidang, menetapkan jarak AM antara titik
tetap A dan M, memiliki garis datar yang agak sederhana: lingkaran
yang berpusat di A.


\>&remvalue();

\>A=[-1,-1];

\>function d1(x,y):=sqrt((x-A[1])^2+(y-A[2])^2)

\>fcontour("d1",xmin=-2,xmax=0,ymin=-2,ymax=0,hue=1, ...  
\>   title="If you see ellipses, please set your window square"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-612.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-612.png)

dan grafiknya cukup sederhana: bagian atas kerucut:


\>plot3d("d1",xmin=-2,xmax=0,ymin=-2,ymax=0):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-613.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-613.png)

Tentu saja minimum 0 dicapai di A.


## Dua titik

Sekarang kita lihat fungsi MA+MB di mana A dan B adalah dua titik
(tetap). Merupakan "fakta yang diketahui" bahwa kurva level adalah
elips, titik fokusnya adalah A dan B; kecuali untuk minimum AB yang
konstan pada segmen [AB]:


\>B=[1,-1];

\>function d2(x,y):=d1(x,y)+sqrt((x-B[1])^2+(y-B[2])^2)

\>fcontour("d2",xmin=-2,xmax=2,ymin=-3,ymax=1,hue=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-614.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-614.png)

Grafiknya lebih menarik:


\>plot3d("d2",xmin=-2,xmax=2,ymin=-3,ymax=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-615.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-615.png)

Pembatasan pada garis (AB) lebih terkenal:


\>plot2d("abs(x+1)+abs(x-1)",xmin=-3,xmax=3):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-616.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-616.png)

## Tiga poin

Sekarang semuanya menjadi kurang sederhana: Tidak banyak yang tahu
bahwa MA+MB+MC mencapai nilai minimumnya di satu titik bidang, tetapi
menentukannya tidaklah sesederhana itu:


1) Jika salah satu sudut segitiga ABC lebih dari 120° (misalkan di A),
maka nilai minimumnya tercapai di titik ini (misalkan AB+AC).


Contoh:


\>C=[-4,1];

\>function d3(x,y):=d2(x,y)+sqrt((x-C[1])^2+(y-C[2])^2)

\>plot3d("d3",xmin=-5,xmax=3,ymin=-4,ymax=4);

\>insimg;


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-617.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-617.png)

\>fcontour("d3",xmin=-4,xmax=1,ymin=-2,ymax=2,hue=1,title="The minimum is on A");

\>P=(A\_B\_C\_A)'; plot2d(P[1],P[2],add=1,color=12);

\>insimg;


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-618.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-618.png)

2) Namun jika semua sudut segitiga ABC kurang dari 120°, maka nilai
minimumnya berada di titik F di bagian dalam segitiga, yang merupakan
satu-satunya titik yang sudut-sudut sisi ABC-nya sama (masing-masing
sudutnya 120°):


\>C=[-0.5,1];

\>plot3d("d3",xmin=-2,xmax=2,ymin=-2,ymax=2):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-619.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-619.png)

\>fcontour("d3",xmin=-2,xmax=2,ymin=-2,ymax=2,hue=1,title="The Fermat point");

\>P=(A\_B\_C\_A)'; plot2d(P[1],P[2],add=1,color=12);

\>insimg;


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-620.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-620.png)

Merupakan aktivitas yang menarik untuk mewujudkan gambar di atas
dengan perangkat lunak geometri; misalnya, saya mengetahui perangkat
lunak yang ditulis dalam Java yang memiliki instruksi "garis
kontur"...


Semua ini ditemukan oleh seorang hakim Prancis bernama Pierre de
Fermat; ia menulis surat kepada para dilettan lain seperti pendeta
Marin Mersenne dan Blaise Pascal yang bekerja di pajak penghasilan.
Jadi titik unik F sehingga FA+FB+FC minimal, disebut titik Fermat dari
segitiga tersebut. Namun tampaknya beberapa tahun sebelumnya,
Torriccelli dari Italia telah menemukan titik ini sebelum Fermat
menemukannya! Bagaimanapun tradisinya adalah mencatat titik F ini...


## Empat titik

Langkah berikutnya adalah menambahkan titik ke-4 D dan mencoba
meminimalkan MA+MB+MC+MD; katakanlah Anda adalah operator TV kabel dan
ingin mencari di bidang mana Anda harus meletakkan antena Anda
sehingga Anda dapat menyalurkan sinyal ke empat desa dan menggunakan
panjang kabel sesedikit mungkin!


\>D=[1,1];

\>function d4(x,y):=d3(x,y)+sqrt((x-D[1])^2+(y-D[2])^2)

\>plot3d("d4",xmin=-1.5,xmax=1.5,ymin=-1.5,ymax=1.5):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-621.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-621.png)

\>fcontour("d4",xmin=-1.5,xmax=1.5,ymin=-1.5,ymax=1.5,hue=1);

\>P=(A\_B\_C\_D)'; plot2d(P[1],P[2],points=1,add=1,color=12);

\>insimg;


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-622.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-622.png)

Masih terdapat nilai minimum dan tidak tercapai di titik A, B, C,
maupun D:


\>function f(x):=d4(x[1],x[2])

\>neldermin("f",[0.2,0.2])


    [0.142858,  0.142857]

Tampaknya dalam kasus ini, koordinat titik optimal bersifat rasional
atau mendekati rasional...


Sekarang ABCD adalah persegi, kita mengharapkan bahwa titik optimal
akan menjadi pusat ABCD:


\>C=[-1,1];

\>plot3d("d4",xmin=-1,xmax=1,ymin=-1,ymax=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-623.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-623.png)

\>fcontour("d4",xmin=-1.5,xmax=1.5,ymin=-1.5,ymax=1.5,hue=1);

\>P=(A\_B\_C\_D)'; plot2d(P[1],P[2],add=1,color=12,points=1);

\>insimg;


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-624.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-624.png)

# Contoh 7: Bola Dandelin dengan Povray

Anda dapat menjalankan demonstrasi ini, jika Anda telah menginstal
Povray, dan pvengine.exe di jalur program.


Pertama, kita hitung jari-jari bola.


Jika Anda melihat gambar di bawah, Anda melihat bahwa kita memerlukan
dua lingkaran yang menyentuh dua garis yang membentuk kerucut, dan
satu garis yang membentuk bidang yang memotong kerucut.


Kami menggunakan file geometry.e milik Euler untuk ini.


\>load geometry;


Pertama dua garis membentuk kerucut.


\>g1 &= lineThrough([0,0],[1,a])


    
                                 [- a, 1, 0]
    

\>g2 &= lineThrough([0,0],[-1,a])


    
                                [- a, - 1, 0]
    

Lalu baris ketiga.


\>g &= lineThrough([-1,0],[1,1])


    
                                 [- 1, 2, 1]
    

Kita merencanakan segalanya sejauh ini.


\>setPlotRange(-1,1,0,2);

\>color(black); plotLine(g(),"")

\>a:=2; color(blue); plotLine(g1(),""), plotLine(g2(),""):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-625.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-625.png)

Sekarang kita ambil titik umum pada sumbu y.


\>P &= [0,u]


    
                                    [0, u]
    

Hitunglah jarak ke g1.


\>d1 &= distance(P,projectToLine(P,g1)); $d1


$$\sqrt{\left(\frac{a^2\,u}{a^2+1}-u\right)^2+\frac{a^2\,u^2}{\left(a
 ^2+1\right)^2}}$$Hitunglah jarak ke g.


\>d &= distance(P,projectToLine(P,g)); $d


$$\sqrt{\left(\frac{u+2}{5}-u\right)^2+\frac{\left(2\,u-1\right)^2}{
 25}}$$Dan temukan pusat kedua lingkaran, yang jaraknya sama.


\>sol &= solve(d1^2=d^2,u); $sol


$$\left[ u=\frac{-\sqrt{5}\,\sqrt{a^2+1}+2\,a^2+2}{4\,a^2-1} , u=
 \frac{\sqrt{5}\,\sqrt{a^2+1}+2\,a^2+2}{4\,a^2-1} \right] $$Ada dua solusi.


Kita mengevaluasi solusi simbolik, dan menemukan kedua pusat, dan
kedua jarak.


\>u := sol()


    [0.333333,  1]

\>dd := d()


    [0.149071,  0.447214]

Gambarkan lingkaran-lingkaran tersebut ke dalam gambar.


\>color(red); plotCircle(circleWithCenter([0,u[1]],dd[1]),""); ...  
\>   plotCircle(circleWithCenter([0,u[2]],dd[2]),""); insimg;


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-629.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-629.png)

## Plot dengan Povray

Selanjutnya kita plot semuanya dengan Povray. Perhatikan bahwa Anda
mengubah perintah apa pun dalam urutan perintah Povray berikut, dan
menjalankan kembali semua perintah dengan Shift-Return.


Pertama-tama kita memuat fungsi povray.


\>load povray;

\>defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

Kami menyiapkan suasananya dengan tepat.


\>povstart(zoom=11,center=[0,0,0.5],height=10°,angle=140°);


Berikutnya kita menulis kedua bola itu ke dalam file Povray.


\>writeln(povsphere([0,0,u[1]],dd[1],povlook(red)));

\>writeln(povsphere([0,0,u[2]],dd[2],povlook(red)));


Dan kerucutnya, transparan.


\>writeln(povcone([0,0,0],0,[0,0,a],1,povlook(lightgray,1)));


Kita buat bidang yang dibatasi pada kerucut.


\>gp=g();

\>pc=povcone([0,0,0],0,[0,0,a],1,"");

\>vp=[gp[1],0,gp[2]]; dp=gp[3];

\>writeln(povplane(vp,dp,povlook(blue,0.5),pc));


Sekarang kita buat dua titik pada lingkaran, di mana bola menyentuh
kerucut.


\>function turnz(v) := return [-v[2],v[1],v[3]]

\>P1=projectToLine([0,u[1]],g1()); P1=turnz([P1[1],0,P1[2]]);

\>writeln(povpoint(P1,povlook(yellow)));

\>P2=projectToLine([0,u[2]],g1()); P2=turnz([P2[1],0,P2[2]]);


Kemudian kita buat dua titik tempat bola-bola tersebut menyentuh
bidang. Titik-titik ini adalah fokus elips.


\>P3=projectToLine([0,u[1]],g()); P3=[P3[1],0,P3[2]];

\>writeln(povpoint(P3,povlook(yellow)));

\>P4=projectToLine([0,u[2]],g()); P4=[P4[1],0,P4[2]];

\>writeln(povpoint(P4,povlook(yellow)));


Berikutnya kita hitung perpotongan P1P2 dengan bidang.


\>t1=scalp(vp,P1)-dp; t2=scalp(vp,P2)-dp; P5=P1+t1/(t1-t2)\*(P2-P1);

\>writeln(povpoint(P5,povlook(yellow)));


Kita menghubungkan titik-titik dengan segmen garis.


\>writeln(povsegment(P1,P2,povlook(yellow)));

\>writeln(povsegment(P5,P3,povlook(yellow)));

\>writeln(povsegment(P5,P4,povlook(yellow)));


Sekarang kita buat pita abu-abu, di mana bola-bola menyentuh kerucut.


\>pcw=povcone([0,0,0],0,[0,0,a],1.01);

\>pc1=povcylinder([0,0,P1[3]-defaultpointsize/2],[0,0,P1[3]+defaultpointsize/2],1);

\>writeln(povintersection([pcw,pc1],povlook(gray)));

\>pc2=povcylinder([0,0,P2[3]-defaultpointsize/2],[0,0,P2[3]+defaultpointsize/2],1);

\>writeln(povintersection([pcw,pc2],povlook(gray)));


Mulai program Povray.


\>povend();


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-630.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-630.png)

Untuk mendapatkan Anaglyph ini, kita perlu memasukkan semuanya ke
dalam fungsi scene. Fungsi ini akan digunakan dua kali nanti.


\>function scene () ...


    endfunction
</pre>
Anda memerlukan kacamata merah/cyan untuk menghargai efek berikut.


\>povanaglyph("scene",zoom=11,center=[0,0,0.5],height=10°,angle=140°):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-631.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-631.png)

![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-632.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-632.png)

# Contoh 8: Geometri Bumi

Dalam buku catatan ini, kami ingin melakukan beberapa perhitungan
sferis. Fungsi-fungsi tersebut terdapat dalam berkas "spherical.e" di
folder contoh. Kami perlu memuat berkas tersebut terlebih dahulu.


\>load "spherical.e";


Untuk memasukkan posisi geografis, kami menggunakan vektor dengan dua
koordinat dalam radian (utara dan timur, nilai negatif untuk selatan
dan barat). Berikut ini adalah koordinat untuk Kampus FMIPA UNY.


\>FMIPA=[rad(-7,-46.467),rad(110,23.05)]


    [-0.13569,  1.92657]

Anda dapat mencetak posisi ini dengan sposprint (cetak posisi bulat).


\>sposprint(FMIPA) // posisi garis lintang dan garis bujur FMIPA UNY


    S 7°46.467' E 110°23.050'

Mari kita tambahkan dua kota lagi, Solo dan Semarang.


\>Solo=[rad(-7,-34.333),rad(110,49.683)]; Semarang=[rad(-6,-59.05),rad(110,24.533)];

\>sposprint(Solo), sposprint(Semarang),


    S 7°34.333' E 110°49.683'
    S 6°59.050' E 110°24.533'

Pertama, kita hitung vektor dari satu ke yang lain pada bola ideal.
Vektor ini adalah [arah, jarak] dalam radian. Untuk menghitung jarak
di bumi, kita kalikan dengan jari-jari bumi pada garis lintang 7°.


\>br=svector(FMIPA,Solo); degprint(br[1]), br[2]\*rearth(7°)-\>km // perkiraan jarak FMIPA-Solo


    65°20'26.60''
    53.8945384608

Ini adalah perkiraan yang bagus. Rutin berikut menggunakan perkiraan
yang lebih baik lagi. Pada jarak yang pendek, hasilnya hampir sama.


\>esdist(FMIPA,Semarang)-\>" km"; // perkiraan jarak FMIPA-Semarang


Ada fungsi untuk judul, yang memperhitungkan bentuk elips bumi. Sekali
lagi, kami mencetak dengan cara yang canggih.


\>sdegprint(esdir(FMIPA,Solo))


         65.34°

Sudut suatu segitiga melebihi 180° pada bola.


\>asum=sangle(Solo,FMIPA,Semarang)+sangle(FMIPA,Solo,Semarang)+sangle(FMIPA,Semarang,Solo); degprint(asum)


    180°0'10.77''

Ini dapat digunakan untuk menghitung luas segitiga. Catatan: Untuk
segitiga kecil, ini tidak akurat karena kesalahan pengurangan dalam
asum-pi.


\>(asum-pi)\*rearth(48°)^2-\>" km^2"; // perkiraan luas segitiga FMIPA-Solo-Semarang


Ada fungsi untuk ini, yang menggunakan lintang rata-rata segitiga
untuk menghitung jari-jari bumi, dan menangani kesalahan pembulatan
untuk segitiga yang sangat kecil.


\>esarea(Solo,FMIPA,Semarang)-\>" km^2", //perkiraan yang sama dengan fungsi esarea()


    2123.64310526 km^2

Kita juga dapat menambahkan vektor ke posisi. Vektor berisi arah dan
jarak, keduanya dalam radian. Untuk mendapatkan vektor, kita
menggunakan svector. Untuk menambahkan vektor ke posisi, kita
menggunakan saddvector.


\>v=svector(FMIPA,Solo); sposprint(saddvector(FMIPA,v)), sposprint(Solo),


    S 7°34.333' E 110°49.683'
    S 7°34.333' E 110°49.683'

Fungsi-fungsi ini mengasumsikan bentuk bola yang ideal. Sama halnya di
bumi.


\>sposprint(esadd(FMIPA,esdir(FMIPA,Solo),esdist(FMIPA,Solo))), sposprint(Solo),


    S 7°34.333' E 110°49.683'
    S 7°34.333' E 110°49.683'

Mari kita lihat contoh yang lebih besar, Tugu Jogja dan Monas Jakarta
(menggunakan Google Earth untuk mencari koordinatnya).


\>Tugu=[-7.7833°,110.3661°]; Monas=[-6.175°,106.811944°];

\>sposprint(Tugu), sposprint(Monas)


    S 7°46.998' E 110°21.966'
    S 6°10.500' E 106°48.717'

Menurut Google Earth, jaraknya adalah 429,66 km. Kami memperoleh
perkiraan yang baik.


\>esdist(Tugu,Monas)-\>" km"; // perkiraan jarak Tugu Jogja - Monas Jakarta


Judulnya sama dengan yang dihitung di Google Earth.


\>degprint(esdir(Tugu,Monas))


    294°17'2.85''

Akan tetapi, kita tidak lagi memperoleh posisi target yang tepat, jika
kita menambahkan arah dan jarak ke posisi awal. Hal ini terjadi karena
kita tidak menghitung fungsi invers secara tepat, tetapi mengambil
perkiraan radius bumi di sepanjang lintasan.


\>sposprint(esadd(Tugu,esdir(Tugu,Monas),esdist(Tugu,Monas)))


    S 6°10.500' E 106°48.717'

Namun, kesalahannya tidak besar.


\>sposprint(Monas),


    S 6°10.500' E 106°48.717'

Tentu saja, kita tidak dapat berlayar dengan arah yang sama dari satu
tujuan ke tujuan lain, jika kita ingin mengambil jalur terpendek.
Bayangkan, Anda terbang ke arah timur laut mulai dari titik mana pun
di bumi. Kemudian Anda akan berputar ke kutub utara. Lingkaran besar
tidak mengikuti arah yang konstan!


Perhitungan berikut menunjukkan bahwa kita jauh dari tujuan yang
benar, jika kita menggunakan arah yang sama selama perjalanan kita.


\>dist=esdist(Tugu,Monas); hd=esdir(Tugu,Monas);


Sekarang kita tambahkan 10 dikalikan sepersepuluh jaraknya, dengan
memakai arah ke Monas, kita sampai di Tugu.


\>p=Tugu; loop 1 to 10; p=esadd(p,hd,dist/10); end;


Hasilnya sangat jauh.


\>sposprint(p), skmprint(esdist(p,Monas))


    S 6°11.250' E 106°48.372'
         1.529km

Sebagai contoh lain, mari kita ambil dua titik di bumi pada garis
lintang yang sama.


\>P1=[30°,10°]; P2=[30°,50°];


Lintasan terpendek dari P1 ke P2 bukanlah lingkaran lintang 30°,
tetapi lintasan yang lebih pendek yang dimulai 10° lebih jauh ke utara
di P1.


\>sdegprint(esdir(P1,P2))


         79.69°

Namun, jika kita mengikuti pembacaan kompas ini, kita akan berputar ke
kutub utara! Jadi kita harus menyesuaikan arah kita di sepanjang
jalan. Untuk tujuan kasar, kita menyesuaikannya pada 1/10 dari total
jarak.


\>p=P1;  dist=esdist(P1,P2); ...  
\>   loop 1 to 10; dir=esdir(p,P2); sdegprint(dir), p=esadd(p,dir,dist/10); end;


         79.69°
         81.67°
         83.71°
         85.78°
         87.89°
         90.00°
         92.12°
         94.22°
         96.29°
         98.33°

Jaraknya tidak tepat, karena kita akan menambahkan sedikit kesalahan,
jika kita mengikuti arah yang sama terlalu lama.


\>skmprint(esdist(p,P2))


         0.203km

Kita memperoleh perkiraan yang baik, jika kita menyesuaikan arah
setelah setiap 1/100 jarak total dari Tugu ke Monas.


\>p=Tugu; dist=esdist(Tugu,Monas); ...  
\>   loop 1 to 100; p=esadd(p,esdir(p,Monas),dist/100); end:


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-633.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-633.png)

\>skmprint(esdist(p,Monas))


         0.000km

Untuk keperluan navigasi, kita bisa mendapatkan urutan posisi GPS
sepanjang lingkaran besar menuju Monas dengan fungsi navigasi.


\>load spherical; v=navigate(Tugu,Monas,10); ...  
\>   loop 1 to rows(v); sposprint(v[#]), end;


    S 7°46.998' E 110°21.966'
    S 7°37.422' E 110°0.573'
    S 7°27.829' E 109°39.196'
    S 7°18.219' E 109°17.834'
    S 7°8.592' E 108°56.488'
    S 6°58.948' E 108°35.157'
    S 6°49.289' E 108°13.841'
    S 6°39.614' E 107°52.539'
    S 6°29.924' E 107°31.251'
    S 6°20.219' E 107°9.977'
    S 6°10.500' E 106°48.717'

Kita menulis suatu fungsi yang memplot bumi, dua posisi, dan posisi di
antaranya.


\>function testplot ...


    $useglobal;
    endfunction
</pre>
Sekarang rencanakan semuanya.


\>plot3d("testplot",angle=25, height=6,\>own,\>user,zoom=4):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-634.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-634.png)

Atau gunakan plot3d untuk mendapatkan tampilan anaglifnya. Ini tampak
sangat bagus dengan kaca mata merah/biru kehijauan.


\>plot3d("testplot",angle=25,height=6,distance=5,own=1,anaglyph=1,zoom=4):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-635.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-635.png)

# Latihan

1. Gambarlah segi-n beraturan jika diketahui titik pusat O, n, dan
jarak titik pusat ke titik-titik sudut segi-n tersebut (jari-jari
lingkaran luar segi-n), r.


Petunjuk:


* 
Besar sudut pusat yang menghadap masing-masing sisi segi-n adalah
* (360/n).

* 
Titik-titik sudut segi-n merupakan perpotongan lingkaran luar segi-n
* dan garis-garis yang melalui pusat dan saling membentuk sudut sebesar
* kelipatan (360/n).

* 
Untuk n ganjil, pilih salah satu titik sudut adalah di atas.

* 
Untuk n genap, pilih 2 titik di kanan dan kiri lurus dengan titik
* pusat.

* 
Anda dapat menggambar segi-3, 4, 5, 6, 7, dst beraturan.


\>load geometry


    Numerical and symbolic geometry.

\>setPlotRange(-3.5,3.5,-3.5,3.5);

\>A=[-2,-2]; plotPoint(A,"A");

\>B=[2,-2]; plotPoint(B,"B");

\>C=[0,3]; plotPoint(C,"C");

\>plotSegment(A,B,"c");

\>plotSegment(B,C,"a");

\>plotSegment(A,C,"b");

\>aspect(1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-636.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-636.png)

\>c=circleThrough(A,B,C); R=getCircleRadius(c); O=getCircleCenter(c);...  
\>   plotPoint(O,"O"); l=angleBisector(A,C,B); color(2); plotLine(l); color(1);...  
\>   plotCircle(c,"Lingkaran luar segitiga ABC"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-637.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-637.png)

2. Gambarlah suatu parabola yang melalui 3 titik yang diketahui.


Petunjuk:


- Misalkan persamaan parabolanya y= ax^2+bx+c.


- Substitusikan koordinat titik-titik yang diketahui ke persamaan
tersebut.


- Selesaikan SPL yang terbentuk untuk mendapatkan nilai-nilai a, b, c.


\>load geometry;

\>setPlotRange(5); P=[2,0]; Q=[4,0]; R=[0,-4];

\>plotPoint(P,"P"); plotPoint(Q,"Q"); plotPoint(R,"R"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-638.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-638.png)

\>sol &= solve([a+b=-c,16\*a+4\*b=-c,c=-4],[a,b,c])


    
                         [[a = - 1, b = 5, c = - 4]]
    

\>function y&=-x^2+5\*x-4


    
                                   2
                                - x  + 5 x - 4
    

\>plot2d("-x^2+5\*x-4",-5,5,-5,5):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-639.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-639.png)

3. Gambarlah suatu segi-4 yang diketahui keempat titik sudutnya,
misalnya A, B, C, D.


   - Tentukan apakah segi-4 tersebut merupakan segi-4 garis singgung
(sisinya-sisintya merupakan garis singgung lingkaran yang sama yakni
lingkaran dalam segi-4 tersebut).


   - Suatu segi-4 merupakan segi-4 garis singgung apabila keempat
garis bagi sudutnya bertemu di satu titik.


   - Jika segi-4 tersebut merupakan segi-4 garis singgung, gambar
lingkaran dalamnya.


   - Tunjukkan bahwa syarat suatu segi-4 merupakan segi-4 garis
singgung apabila hasil kali panjang sisi-sisi yang berhadapan sama.


\>load geometry


    Numerical and symbolic geometry.

\>setPlotRange(-4.5,4.5,-4.5,4.5);

\>A=[-3,-3]; plotPoint(A,"A");

\>B=[3,-3]; plotPoint(B,"B");

\>C=[3,3]; plotPoint(C,"C");

\>D=[-3,3]; plotPoint(D,"D");

\>plotSegment(A,B,"");

\>plotSegment(B,C,"");

\>plotSegment(C,D,"");

\>plotSegment(A,D,"");

\>aspect(1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-640.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-640.png)

\>l=angleBisector(A,B,C); m=angleBisector(B,C,D); P=lineIntersection(l,m);...  
\>   color(5); plotLine(l); plotLine(m); color(1); plotPoint(P,"P"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-641.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-641.png)

Dari gambar diatas terlihat bahwa keempat garis bagi sudutnya bertemu
di satu titik yaitu titik P.


\>r=norm(P-projectToLine(P,lineThrough(A,B)));

\>plotCircle(circleWithCenter(P,r),"Lingkaran dalam segiempat ABCD"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-642.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-642.png)

Dari gambar diatas, terlihat bahwa sisi-sisinya merupakan garis
singgung lingkaran yang sama yaitu lingkaran dalam segiempat.


Akan ditunjukkan bahwa hasil kali panjang sisi-sisi yang berhadapan
sama.


\>AB=norm(A-B) //panjang sisi AB


    6

\>CD=norm(C-D) //panjang sisi CD


    6

\>AD=norm(A-D) //panjang sisi AD


    6

\>BC=norm(B-C) //panjang sisi BC


    6

\>AB.CD, AD.BC


    36
    36

Terbukti bahwa hasil kali panjang sisi-sisi yang berhadapan sama yaitu
36. Jadi dapat dipastikan bahwa segiempat tersebut merupakan segiempat
garis singgung.


4. Gambarlah suatu ellips jika diketahui kedua titik fokusnya,
misalnya P dan Q. Ingat ellips dengan fokus P dan Q adalah tempat
kedudukan titik-titik yang jumlah jarak ke P dan ke Q selalu sama
(konstan).


Penyelesaian :


Diketahui kedua titik fokus P = [-1,-1] dan Q = [1,-1]


\>P=[-1,-1]; Q=[1,-1];

\>function d1(x,y):=sqrt((x-P[1])^2+(y-P[2])^2)

\>Q=[1,-1]; function d2(x,y):=sqrt((x-P[1])^2+(y-P[2])^2)+sqrt((x-Q[1])^2+(y-Q[2])^2)

\>fcontour("d2",xmin=-2,xmax=2,ymin=-3,ymax=1,hue=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-643.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-643.png)

\>reset()


    0

Grafik yang lebih menarik


\>plot3d("d2",xmin=-2,xmax=2,ymin=-3,ymax=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-644.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-644.png)

5. Gambarlah suatu hiperbola jika diketahui kedua titik fokusnya,
misalnya P dan Q. Ingat ellips dengan fokus P dan Q adalah tempat
kedudukan titik-titik yang selisih jarak ke P dan ke Q selalu sama
(konstan).


\>P=[-1,-1]; Q=[1,-1];

\>function d1(x,y):=sqrt((x-p[1])^2+(y-p[2])^2)

\>Q=[1,-1]; function d2(x,y):=sqrt((x-P[1])^2+(y-P[2])^2)+sqrt((x+Q[1])^2+(y+Q[2])^2)

\>fcontour("d2",xmin=-2,xmax=2,ymin=-3,ymax=1,hue=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-645.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-645.png)

\>reset()


    0

\>plot3d("d2",xmin=-2,xmax=2,ymin=-3,ymax=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-646.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-646.png)

\>reset()


    0

\>plot2d("abs(x+1)+abs(x-1)",xmin=-3,xmax=3):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-647.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-647.png)

# EMT untuk Statistika

Di buku catatan ini, kami mendemonstrasikan plot statistik utama,
pengujian, dan distribusi di Euler.


Mari kita mulai dengan beberapa statistik deskriptif. Ini bukan
pengantar statistik. Jadi, Anda mungkin memerlukan latar belakang
untuk memahami detailnya.


Asumsikan pengukuran berikut. Kami ingin menghitung nilai rata-rata
dan deviasi standar yang diukur.


\>M=[1000,1004,998,997,1002,1001,998,1004,998,997]; ...  
\>   median(M), mean(M), dev(M),


    999
    999.9
    2.72641400622

Kita dapat memplot plot kotak-dan-kumis untuk datanya. Dalam kasus
kami, tidak ada outlier.


\>aspect(1.75); boxplot(M):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-648.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-648.png)

Kami menghitung probabilitas suatu nilai lebih besar dari 1005, dengan
asumsi nilai terukur berdistribusi normal.


Semua fungsi untuk distribusi di Euler diakhiri dengan ...dis dan
menghitung distribusi probabilitas kumulatif (CPF).


Kami mencetak hasilnya dalam % dengan akurasi 2 digit menggunakan
fungsi print.


\>print((1-normaldis(1005,mean(M),dev(M)))\*100,2,unit=" %")


          3.07 %

Untuk contoh berikutnya, kita asumsikan jumlah pria berikut dalam
rentang ukuran tertentu.


\>r=155.5:4:187.5; v=[22,71,136,169,139,71,32,8];


Berikut adalah alur pendistribusiannya.


\>plot2d(r,v,a=150,b=200,c=0,d=190,bar=1,style="\\/"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-649.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-649.png)

Kita bisa memasukkan data mentah tersebut ke dalam tabel.


Tabel adalah metode untuk menyimpan data statistik. Tabel kita harus
berisi tiga kolom: Awal jangkauan, akhir jangkauan, jumlah pria dalam
jangkauan.


Tabel dapat dicetak dengan header. Kami menggunakan vektor string
untuk mengatur header.


\>T:=r[1:8]' | r[2:9]' | v'; writetable(T,labc=["BB","BA","Frek"])


            BB        BA      Frek
         155.5     159.5        22
         159.5     163.5        71
         163.5     167.5       136
         167.5     171.5       169
         171.5     175.5       139
         175.5     179.5        71
         179.5     183.5        32
         183.5     187.5         8

Jika kita memerlukan nilai rata-rata dan statistik ukuran lainnya,
kita perlu menghitung titik tengah rentang tersebut. Kita bisa
menggunakan dua kolom pertama tabel kita untuk ini.


Sumbol "|" digunakan untuk memisahkan kolom, fungsi "writetable"
digunakan untuk menulis tabel, dengan opsi "labc" untuk menentukan
header kolom.


\>(T[,1]+T[,2])/2 // the midpoint of each interval


            157.5 
            161.5 
            165.5 
            169.5 
            173.5 
            177.5 
            181.5 
            185.5 

Namun akan lebih mudah jika menjumlahkan rentang dengan vektor
[1/2,1/2].


\>M=fold(r,[0.5,0.5])


    [157.5,  161.5,  165.5,  169.5,  173.5,  177.5,  181.5,  185.5]

Sekarang kita dapat menghitung mean dan deviasi sampel dengan
frekuensi tertentu.


\>{m,d}=meandev(M,v); m, d,


    169.901234568
    5.98912964449

Mari kita tambahkan distribusi nilai normal ke diagram batang di atas.
Rumus distribusi normal dengan mean m dan simpangan baku d adalah:


Karena nilainya antara 0 dan 1, maka untuk memplotnya pada bar plot
harus dikalikan dengan 4 kali jumlah data.


\>plot2d("qnormal(x,m,d)\*sum(v)\*4", ...  
\>     xmin=min(r),xmax=max(r),thickness=3,add=1):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-650.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-650.png)

# Tabel

Di direktori buku catatan ini Anda menemukan file dengan tabel. Data
tersebut merupakan hasil survei. Berikut adalah empat baris pertama
file tersebut. Datanya berasal dari buku online Jerman "Einführung in
die Statistik mit R" oleh A. Handl.


\>printfile("table.dat",4);


    Could not open the file
    table.dat
    for reading!
    Try "trace errors" to inspect local variables after errors.
    printfile:
        open(filename,"r");

Tabel berisi 7 kolom angka atau token (string). Kami ingin membaca
tabel dari file. Pertama, kami menggunakan terjemahan kami sendiri
untuk tokennya.


Untuk ini, kami mendefinisikan kumpulan token. Fungsi strtokens()
mendapatkan vektor string token dari string tertentu.


\>mf:=["m","f"]; yn:=["y","n"]; ev:=strtokens("g vg m b vb");


Sekarang kita membaca tabel dengan terjemahan ini.


Argumen tok2, tok4 dll. adalah terjemahan dari kolom tabel. Argumen
ini tidak ada dalam daftar parameter readtable(), jadi Anda perlu
menyediakannya dengan ":=".


\>{MT,hd}=readtable("table.dat",tok2:=mf,tok4:=yn,tok5:=ev,tok7:=yn);


    Could not open the file
    table.dat
    for reading!
    Try "trace errors" to inspect local variables after errors.
    readtable:
        if filename!=none then open(filename,"r"); endif;

\>load over statistics;


Untuk mencetak, kita perlu menentukan kumpulan token yang sama. Kami
mencetak empat baris pertama saja.


\>writetable(MT[1:10],labc=hd,wc=5,tok2:=mf,tok4:=yn,tok5:=ev,tok7:=yn);


    MT is not a variable!
    Error in:
    writetable(MT[1:10],labc=hd,wc=5,tok2:=mf,tok4:=yn,tok5:=ev,to ...
                       ^

Titik "." mewakili nilai-nilai, yang tidak tersedia.


Jika kita tidak ingin menentukan token yang akan diterjemahkan
terlebih dahulu, kita hanya perlu menentukan, kolom mana yang berisi
token dan bukan angka.


\>ctok=[2,4,5,7]; {MT,hd,tok}=readtable("table.dat",ctok=ctok);


    Could not open the file
    table.dat
    for reading!
    Try "trace errors" to inspect local variables after errors.
    readtable:
        if filename!=none then open(filename,"r"); endif;

Fungsi readtable() kini mengembalikan sekumpulan token.


\>tok


    Variable tok not found!
    Error in:
    tok ...
       ^

Tabel berisi entri dari file dengan token yang diterjemahkan ke dalam
angka.


String khusus NA = "." diartikan sebagai "Tidak Tersedia", dan
mendapatkan NAN (bukan angka) di tabel. Terjemahan ini dapat diubah
dengan parameter NA, dan NAval.


\>MT[1]


    MT is not a variable!
    Error in:
    MT[1] ...
         ^

Berikut isi tabel dengan nomor yang belum diterjemahkan.


\>writetable(MT,wc=5)


    Variable or function MT not found.
    Error in:
    writetable(MT,wc=5) ...
                 ^

Untuk kenyamanan, Anda dapat memasukkan keluaran readtable() ke dalam
daftar.


\>Table={{readtable("table.dat",ctok=ctok)}};


    Could not open the file
    table.dat
    for reading!
    Try "trace errors" to inspect local variables after errors.
    readtable:
        if filename!=none then open(filename,"r"); endif;

Dengan menggunakan kolom token yang sama dan token yang dibaca dari
file, kita dapat mencetak tabel. Kita dapat menentukan ctok, tok, dll.
atau menggunakan tabel daftar.


\>writetable(Table,ctok=ctok,wc=5);


    Variable or function Table not found.
    Error in:
    writetable(Table,ctok=ctok,wc=5); ...
                    ^

Fungsi tablecol() mengembalikan nilai kolom tabel, melewatkan baris
apa pun dengan nilai NAN ("." dalam file), dan indeks kolom, yang
berisi nilai-nilai ini.


\>{c,i}=tablecol(MT,[5,6]);


    Variable or function MT not found.
    Error in:
    {c,i}=tablecol(MT,[5,6]); ...
                     ^

Kita bisa menggunakan ini untuk mengekstrak kolom dari tabel untuk
tabel baru.


\>j=[1,5,6]; writetable(MT[i,j],labc=hd[j],ctok=[2],tok=tok)


    MT is not a variable!
    Error in:
    j=[1,5,6]; writetable(MT[i,j],labc=hd[j],ctok=[2],tok=tok) ...
                                 ^

Tentu saja, kita perlu mengekstrak tabel itu sendiri dari daftar Tabel
dalam kasus ini.


\>MT=Table[1];


    Table is not a variable!
    Error in:
    MT=Table[1]; ...
               ^

Tentu saja, kita juga dapat menggunakannya untuk menentukan nilai
rata-rata suatu kolom atau nilai statistik lainnya.


\>mean(tablecol(MT,6))


    Variable or function MT not found.
    Error in:
    mean(tablecol(MT,6)) ...
                    ^

Fungsi getstatistics() mengembalikan elemen dalam vektor, dan
jumlahnya. Kami menerapkannya pada nilai "m" dan "f" di kolom kedua
tabel kami.


\>{xu,count}=getstatistics(tablecol(MT,2)); xu, count,


    Variable or function MT not found.
    Error in:
    {xu,count}=getstatistics(tablecol(MT,2)); xu, count, ...
                                        ^

Kita bisa mencetak hasilnya di tabel baru.


\>writetable(count',labr=tok[xu])


    Variable count not found!
    Error in:
    writetable(count',labr=tok[xu]) ...
                     ^

Fungsi selecttable() mengembalikan tabel baru dengan nilai dalam satu
kolom yang dipilih dari vektor indeks. Pertama kita mencari indeks
dari dua nilai kita di tabel token.


\>v:=indexof(tok,["g","vg"])


    Variable or function tok not found.
    Error in:
    v:=indexof(tok,["g","vg"]) ...
                  ^

Sekarang kita dapat memilih baris tabel, yang memiliki salah satu
nilai v pada baris ke-5.


\>MT1:=MT[selectrows(MT,5,v)]; i:=sortedrows(MT1,5);


    Variable or function MT not found.
    Error in:
    MT1:=MT[selectrows(MT,5,v)]; i:=sortedrows(MT1,5); ...
                         ^

Sekarang kita dapat mencetak tabel, dengan nilai yang diekstraksi dan
diurutkan di kolom ke-5.


\>writetable(MT1[i],labc=hd,ctok=ctok,tok=tok,wc=7);


    MT1 is not a variable!
    Error in:
    writetable(MT1[i],labc=hd,ctok=ctok,tok=tok,wc=7); ...
                     ^

Untuk statistik selanjutnya, kami ingin menghubungkan dua kolom tabel.
Jadi kita ekstrak kolom 2 dan 4 dan urutkan tabelnya.


\>i=sortedrows(MT,[2,4]);  ...  
\>     writetable(tablecol(MT[i],[2,4])',ctok=[1,2],tok=tok)


    Variable or function MT not found.
    Error in:
    i=sortedrows(MT,[2,4]);    writetable(tablecol(MT[i],[2,4])',c ...
                   ^

Dengan getstatistics(), kita juga bisa menghubungkan jumlah dalam dua
kolom tabel satu sama lain.


\>MT24=tablecol(MT,[2,4]); ...  
\>   {xu1,xu2,count}=getstatistics(MT24[1],MT24[2]); ...  
\>   writetable(count,labr=tok[xu1],labc=tok[xu2])


    Variable or function MT not found.
    Error in:
    MT24=tablecol(MT,[2,4]); {xu1,xu2,count}=getstatistics(MT24[1] ...
                    ^

Sebuah tabel dapat ditulis ke file.


\>filename="test.dat"; ...  
\>   writetable(count,labr=tok[xu1],labc=tok[xu2],file=filename);


    Variable or function count not found.
    Error in:
    filename="test.dat"; writetable(count,labr=tok[xu1],labc=tok[x ...
                                         ^

Kemudian kita bisa membaca tabel dari file tersebut.


\>{MT2,hd,tok2,hdr}=readtable(filename,\>clabs,\>rlabs); ...  
\>   writetable(MT2,labr=hdr,labc=hd)


    Could not open the file
    test.dat
    for reading!
    Try "trace errors" to inspect local variables after errors.
    readtable:
        if filename!=none then open(filename,"r"); endif;

Dan hapus file tersebut.


\>fileremove(filename);


# Distribusi

Dengan plot2d, ada metode yang sangat mudah untuk memplot sebaran data
eksperimen.


\>p=normal(1,1000); //1000 random normal-distributed sample p

\>plot2d(p,distribution=20,style="\\/"); // plot the random sample p

\>plot2d("qnormal(x,0,1)",add=1): // add the standard normal distribution plot


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-651.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-651.png)

Perlu diperhatikan perbedaan antara bar plot (sampel) dan kurva normal
(distribusi sebenarnya). Masukkan kembali ketiga perintah untuk
melihat hasil pengambilan sampel lainnya.


Berikut adalah perbandingan 10 simulasi dari 1000 nilai terdistribusi
normal menggunakan apa yang disebut plot kotak. Plot ini menunjukkan
median, kuartil 25% dan 75%, nilai minimal dan maksimal, serta
outlier.


\>p=normal(10,1000); boxplot(p):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-652.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-652.png)

Untuk menghasilkan bilangan bulat acak, Euler memiliki intrandom. Mari
kita simulasikan lemparan dadu dan plot distribusinya.


Kita menggunakan fungsi getmultiplicities(v,x), yang menghitung
seberapa sering elemen v muncul di x. Kemudian kita plot hasilnya
menggunakan kolomplot().


\>k=intrandom(1,6000,6);  ...  
\>   columnsplot(getmultiplicities(1:6,k));  ...  
\>   ygrid(1000,color=red):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-653.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-653.png)

Meskipun inrandom(n,m,k) mengembalikan bilangan bulat yang
terdistribusi secara seragam dari 1 hingga k, distribusi bilangan
bulat lainnya dapat digunakan dengan randpint().


Dalam contoh berikut, probabilitas untuk 1,2,3 masing-masing adalah
0,4,0.1,0.5.


\>randpint(1,1000,[0.4,0.1,0.5]); getmultiplicities(1:3,%)


    [395,  106,  499]

Euler dapat menghasilkan nilai acak dari lebih banyak distribusi.
Lihat referensinya.


Misalnya, kita mencoba distribusi eksponensial. Variabel acak kontinu
X dikatakan berdistribusi eksponensial, jika PDF-nya diberikan oleh




dengan parameter


\>plot2d(randexponential(1,1000,2),\>distribution):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-654.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-654.png)

Untuk banyak distribusi, Euler dapat menghitung fungsi distribusi dan
inversnya.


\>plot2d("normaldis",-4,4): 


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-655.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-655.png)

Berikut ini adalah salah satu cara untuk memplot kuantil.


\>plot2d("qnormal(x,1,1.5)",-4,6);  ...  
\>   plot2d("qnormal(x,1,1.5)",a=2,b=5,\>add,\>filled):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-656.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-656.png)



Peluang berada di kawasan hijau adalah sebagai berikut.


\>normaldis(5,1,1.5)-normaldis(2,1,1.5)


    0.248662156979

Ini dapat dihitung secara numerik dengan integral berikut.


\>gauss("qnormal(x,1,1.5)",2,5)


    0.248662156979

Mari kita bandingkan distribusi binomial dengan distribusi normal yang
mean dan deviasinya sama. Fungsi invbindis() menyelesaikan interpolasi
linier antara nilai integer.


\>invbindis(0.95,1000,0.5), invnormaldis(0.95,500,0.5\*sqrt(1000))


    525.516721219
    526.007419394

Fungsi qdis() adalah kepadatan distribusi chi-kuadrat. Seperti biasa,
Euler memetakan vektor ke fungsi ini. Dengan demikian kita mendapatkan
plot semua distribusi chi-kuadrat dengan derajat 5 sampai 30 dengan
mudah dengan cara berikut.


\>plot2d("qchidis(x,(5:5:50)')",0,50):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-657.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-657.png)

Euler memiliki fungsi akurat untuk mengevaluasi distribusi. Mari kita
periksa chidis() dengan integral.


Penamaannya mencoba untuk konsisten. Misalnya.,


* 
distribusi chi-kuadratnya adalah chidis(),

* 
fungsi kebalikannya adalah invchidis(),

* 
kepadatannya adalah qchidis().


Pelengkap distribusi (ekor atas) adalah chicdis().


\>chidis(1.5,2), integrate("qchidis(x,2)",0,1.5)


    0.527633447259
    0.527633447259

# Distribusi Diskrit

Untuk menentukan distribusi diskrit Anda sendiri, Anda dapat
menggunakan metode berikut.


Pertama kita atur fungsi distribusinya.


\>wd = 0|((1:6)+[-0.01,0.01,0,0,0,0])/6


    [0,  0.165,  0.335,  0.5,  0.666667,  0.833333,  1]

Artinya dengan probabilitas wd[i+1]-wd[i] kita menghasilkan nilai acak
i.


Ini hampir merupakan distribusi yang seragam. Mari kita tentukan
generator nomor acak untuk ini. Fungsi find(v,x) mencari nilai x pada
vektor v. Fungsi ini juga berfungsi untuk vektor x.


\>function wrongdice (n,m) := find(wd,random(n,m))


Kesalahannya sangat halus sehingga kita hanya melihatnya dengan banyak
iterasi.


\>columnsplot(getmultiplicities(1:6,wrongdice(1,1000000))):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-658.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-658.png)

Berikut adalah fungsi sederhana untuk memeriksa keseragaman distribusi
nilai 1...K dalam v. Kita menerima hasilnya, jika untuk semua
frekuensi


\>function checkrandom (v, delta=1) ...


      K=max(v); n=cols(v);
      fr=getfrequencies(v,1:K);
      return max(fr/n-1/K)<delta/sqrt(n);
      endfunction
</pre>
Memang fungsinya menolak distribusi seragam.


\>checkrandom(wrongdice(1,1000000))


    0

Dan ia menerima generator acak bawaan.


\>checkrandom(intrandom(1,1000000,6))


    1

Kita dapat menghitung distribusi binomial. Pertama ada binomialsum(),
yang mengembalikan probabilitas i atau kurang hit dari n percobaan.


\>bindis(410,1000,0.4)


    0.751401349654

Fungsi Beta terbalik digunakan untuk menghitung interval kepercayaan
Clopper-Pearson untuk parameter p. Tingkat defaultnya adalah alfa.


Arti dari interval ini adalah jika p berada di luar interval, hasil
pengamatan 410 dalam 1000 jarang terjadi.


\>clopperpearson(410,1000)


    [0.37932,  0.441212]

Perintah berikut adalah cara langsung untuk mendapatkan hasil di atas.
Namun untuk n yang besar, penjumlahan langsungnya tidak akurat dan
lambat.


\>p=0.4; i=0:410; n=1000; sum(bin(n,i)\*p^i\*(1-p)^(n-i))


    0.751401349655

invbinsum() menghitung kebalikan dari binomialsum().


\>invbindis(0.75,1000,0.4)


    409.932733047

Di Bridge, kami mengasumsikan 5 kartu beredar (dari 52) di dua tangan
(26 kartu). Mari kita hitung probabilitas distribusi yang lebih buruk
dari 3:2 (misalnya 0:5, 1:4, 4:1, atau 5:0).


\>2\*hypergeomsum(1,5,13,26)


    0.321739130435

Ada juga simulasi distribusi multinomial.


\>randmultinomial(10,1000,[0.4,0.1,0.5])


              406            80           514 
              419            92           489 
              413           110           477 
              396            88           516 
              385           107           508 
              366            93           541 
              399            98           503 
              431            74           495 
              398           111           491 
              395           116           489 

# Merencanakan Data

Untuk memetakan data, kami mencoba hasil pemilu Jerman sejak tahun
1990, diukur dalam jumlah kursi.


\>BW := [ ...  
\>   1990,662,319,239,79,8,17; ...  
\>   1994,672,294,252,47,49,30; ...  
\>   1998,669,245,298,43,47,36; ...  
\>   2002,603,248,251,47,55,2; ...  
\>   2005,614,226,222,61,51,54; ...  
\>   2009,622,239,146,93,68,76; ...  
\>   2013,631,311,193,0,63,64];


Untuk pesta, kami menggunakan rangkaian nama.


\>P:=["CDU/CSU","SPD","FDP","Gr","Li"];


Mari kita cetak persentasenya dengan baik.


Pertama kita mengekstrak kolom yang diperlukan. Kolom 3 sampai 7
adalah kursi masing-masing partai, dan kolom 2 adalah jumlah kursi
seluruhnya. kolom adalah tahun pemilihan.


\>BT:=BW[,3:7]; BT:=BT/sum(BT); YT:=BW[,1]';


Kemudian statistiknya kita cetak dalam bentuk tabel. Kami menggunakan
nama sebagai header kolom, dan tahun sebagai header untuk baris. Lebar
default untuk kolom adalah wc=10, tetapi kami lebih memilih keluaran
yang lebih padat. Kolom akan diperluas untuk label kolom, jika perlu.


\>writetable(BT\*100,wc=6,dc=0,\>fixed,labc=P,labr=YT)


           CDU/CSU   SPD   FDP    Gr    Li
      1990      48    36    12     1     3
      1994      44    38     7     7     4
      1998      37    45     6     7     5
      2002      41    42     8     9     0
      2005      37    36    10     8     9
      2009      38    23    15    11    12
      2013      49    31     0    10    10

Perkalian matriks berikut ini menjumlahkan persentase dua partai besar
yang menunjukkan bahwa partai-partai kecil berhasil memperoleh suara
di parlemen hingga tahun 2009.


\>BT1:=(BT.[1;1;0;0;0])'\*100


    [84.29,  81.25,  81.1659,  82.7529,  72.9642,  61.8971,  79.8732]

Ada juga plot statistik sederhana. Kami menggunakannya untuk
menampilkan garis dan titik secara bersamaan. Alternatifnya adalah
memanggil plot2d dua kali dengan &gt;add.


\>statplot(YT,BT1,"b"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-659.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-659.png)

Tentukan beberapa warna untuk setiap pesta.


\>CP:=[rgb(0.5,0.5,0.5),red,yellow,green,rgb(0.8,0,0)];


Sekarang kita bisa memplot hasil pemilu 2009 dan perubahannya menjadi
satu plot dengan menggunakan gambar. Kita dapat menambahkan vektor
kolom ke setiap plot.


\>figure(2,1);  ...  
\>   figure(1); columnsplot(BW[6,3:7],P,color=CP); ...  
\>   figure(2); columnsplot(BW[6,3:7]-BW[5,3:7],P,color=CP);  ...  
\>   figure(0):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-660.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-660.png)

Plot data menggabungkan deretan data statistik dalam satu plot.


\>J:=BW[,1]'; DP:=BW[,3:7]'; ...  
\>   dataplot(YT,BT',color=CP);  ...  
\>   labelbox(P,colors=CP,styles="[]",\>points,w=0.2,x=0.3,y=0.4):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-661.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-661.png)

Plot kolom 3D memperlihatkan baris data statistik dalam bentuk kolom.
Kami memberikan label untuk baris dan kolom. sudut adalah sudut
pandang.


\>columnsplot3d(BT,scols=P,srows=YT, ...  
\>     angle=30°,ccols=CP):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-662.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-662.png)

Representasi lainnya adalah plot mosaik. Perhatikan bahwa kolom plot
mewakili kolom matriks di sini. Karena panjang label CDU/CSU, kami
mengambil jendela yang lebih kecil dari biasanya.


\>shrinkwindow(\>smaller);  ...  
\>   mosaicplot(BT',srows=YT,scols=P,color=CP,style="#"); ...  
\>   shrinkwindow():


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-663.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-663.png)

Kita juga bisa membuat diagram lingkaran. Karena hitam dan kuning
membentuk koalisi, kami menyusun ulang elemen-elemennya.


\>i=[1,3,5,4,2]; piechart(BW[6,3:7][i],color=CP[i],lab=P[i]):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-664.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-664.png)

Ini adalah jenis plot lainnya.


\>starplot(normal(1,10)+4,lab=1:10,\>rays):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-665.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-665.png)

Beberapa plot di plot2d bagus untuk statika. Berikut adalah plot
impuls dari data acak, terdistribusi secara seragam di [0,1].


\>plot2d(makeimpulse(1:10,random(1,10)),\>bar):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-666.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-666.png)

Namun untuk data yang terdistribusi secara eksponensial, kita mungkin
memerlukan plot logaritmik.


\>logimpulseplot(1:10,-log(random(1,10))\*10):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-667.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-667.png)

Fungsi Columnplot() lebih mudah digunakan, karena hanya memerlukan
vektor nilai. Selain itu, ia dapat mengatur labelnya ke apa pun yang
kita inginkan, kami telah mendemonstrasikannya di tutorial ini.


Ini adalah aplikasi lain, di mana kita menghitung karakter dalam
sebuah kalimat dan membuat statistik.


\>v=strtochar("the quick brown fox jumps over the lazy dog"); ...  
\>   w=ascii("a"):ascii("z"); x=getmultiplicities(w,v); ...  
\>   cw=[]; for k=w; cw=cw|char(k); end; ...  
\>   columnsplot(x,lab=cw,width=0.05):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-668.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-668.png)

Dimungkinkan juga untuk mengatur sumbu secara manual.


\>n=10; p=0.4; i=0:n; x=bin(n,i)\*p^i\*(1-p)^(n-i); ...  
\>   columnsplot(x,lab=i,width=0.05,<frame,<grid); ...  
\>   yaxis(0,0:0.1:1,style="-\>",\>left); xaxis(0,style="."); ...  
\>   label("p",0,0.25), label("i",11,0); ...  
\>   textbox(["Binomial distribution","with p=0.4"]):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-669.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-669.png)

Berikut ini cara memplot frekuensi bilangan dalam suatu vektor.


Kami membuat vektor bilangan acak bilangan bulat 1 hingga 6.


\>v:=intrandom(1,10,10)


    [2,  3,  7,  10,  3,  9,  10,  5,  1,  5]

Kemudian ekstrak nomor unik di v.


\>vu:=unique(v)


    [1,  2,  3,  5,  7,  9,  10]

Dan plot frekuensi dalam plot kolom.


\>columnsplot(getmultiplicities(vu,v),lab=vu,style="/"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-670.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-670.png)

Kami ingin mendemonstrasikan fungsi distribusi nilai empiris.


\>x=normal(1,20);


Fungsi empdist(x,vs) memerlukan array nilai yang diurutkan. Jadi kita
harus mengurutkan x sebelum kita dapat menggunakannya.


\>xs=sort(x);


Kemudian kita plot distribusi empiris dan beberapa batang kepadatan ke
dalam satu plot. Alih-alih plot batang untuk distribusi kali ini kami
menggunakan plot gigi gergaji.


\>figure(2,1); ...  
\>   figure(1); plot2d("empdist",-4,4;xs); ...  
\>   figure(2); plot2d(histo(x,v=-4:0.2:4,<bar));  ...  
\>   figure(0):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-671.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-671.png)

Plot sebar mudah dilakukan di Euler dengan plot titik biasa. Grafik
berikut menunjukkan bahwa X dan X+Y jelas berkorelasi positif.


\>x=normal(1,100); plot2d(x,x+rotright(x),\>points,style=".."):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-672.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-672.png)

Seringkali kita ingin membandingkan dua sampel dengan distribusi yang
berbeda. Hal ini dapat dilakukan dengan plot kuantil-kuantil.


Untuk pengujiannya, kami mencoba distribusi student-t dan distribusi
eksponensial.


\>x=randt(1,1000,5); y=randnormal(1,1000,mean(x),dev(x)); ...  
\>   plot2d("x",r=6,style="--",yl="normal",xl="student-t",\>vertical); ...  
\>   plot2d(sort(x),sort(y),\>points,color=red,style="x",\>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-673.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-673.png)

Plot tersebut dengan jelas menunjukkan bahwa nilai terdistribusi
normal cenderung lebih kecil di ujung ekstrim.


Jika kita mempunyai dua distribusi yang ukurannya berbeda, kita dapat
memperluas distribusi yang lebih kecil atau mengecilkan distribusi
yang lebih besar. Fungsi berikut ini baik untuk keduanya. Dibutuhkan
nilai median dengan persentase antara 0 dan 1.


\>function medianexpand (x,n) := median(x,p=linspace(0,1,n-1));


Mari kita bandingkan dua distribusi yang sama.


\>x=random(1000); y=random(400); ...  
\>   plot2d("x",0,1,style="--"); ...  
\>   plot2d(sort(medianexpand(x,400)),sort(y),\>points,color=red,style="x",\>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-674.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-674.png)

# Regresi dan Korelasi

Regresi linier dapat dilakukan dengan fungsi polyfit() atau berbagai
fungsi fit.


Sebagai permulaan kita menemukan garis regresi untuk data univariat
dengan polyfit(x,y,1).


\>x=1:10; y=[2,3,1,5,6,3,7,8,9,8]; writetable(x'|y',labc=["x","y"])


             x         y
             1         2
             2         3
             3         1
             4         5
             5         6
             6         3
             7         7
             8         8
             9         9
            10         8

Kami ingin membandingkan kecocokan yang tidak berbobot dan berbobot.
Pertama koefisien kecocokan linier.


\>p=polyfit(x,y,1)


    [0.733333,  0.812121]

Sekarang koefisien dengan bobot yang menekankan nilai terakhir.


\>w &= "exp(-(x-10)^2/10)"; pw=polyfit(x,y,1,w=w(x))


    [4.71566,  0.38319]

Kami memasukkan semuanya ke dalam satu plot untuk titik dan garis
regresi, dan untuk bobot yang digunakan.


\>figure(2,1);  ...  
\>   figure(1); statplot(x,y,"b",xl="Regression"); ...  
\>     plot2d("evalpoly(x,p)",\>add,color=blue,style="--"); ...  
\>     plot2d("evalpoly(x,pw)",5,10,\>add,color=red,style="--"); ...  
\>   figure(2); plot2d(w,1,10,\>filled,style="/",fillcolor=red,xl=w); ...  
\>   figure(0):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-675.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-675.png)

Contoh lain kita membaca survei siswa, usia mereka, usia orang tua
mereka dan jumlah saudara kandung dari sebuah file.


Tabel ini berisi "m" dan "f" di kolom kedua. Kami menggunakan variabel
tok2 untuk mengatur terjemahan yang tepat alih-alih membiarkan
readtable() mengumpulkan terjemahannya.


\>{MS,hd}:=readtable("table1.dat",tok2:=["m","f"]);  ...  
\>   writetable(MS,labc=hd,tok2:=["m","f"]);


    Could not open the file
    table1.dat
    for reading!
    Try "trace errors" to inspect local variables after errors.
    readtable:
        if filename!=none then open(filename,"r"); endif;

Bagaimana usia bergantung satu sama lain? Kesan pertama muncul dari
plot sebar berpasangan.


\>scatterplots(tablecol(MS,3:5),hd[3:5]):


    Variable or function MS not found.
    Error in:
    scatterplots(tablecol(MS,3:5),hd[3:5]): ...
                            ^

Jelas terlihat bahwa usia ayah dan ibu saling bergantung satu sama
lain. Mari kita tentukan dan plot garis regresinya.


\>cs:=MS[,4:5]'; ps:=polyfit(cs[1],cs[2],1)


    MS is not a variable!
    Error in:
    cs:=MS[,4:5]'; ps:=polyfit(cs[1],cs[2],1) ...
                ^

Ini jelas merupakan model yang salah. Garis regresinya adalah
s=17+0,74t, dengan t adalah umur ibu dan s adalah umur ayah. Perbedaan
usia mungkin sedikit bergantung pada usia, tapi tidak terlalu banyak.


Sebaliknya, kami mencurigai fungsi seperti s=a+t. Maka a adalah mean
dari s-t. Ini adalah perbedaan usia rata-rata antara ayah dan ibu.


\>da:=mean(cs[2]-cs[1])


    cs is not a variable!
    Error in:
    da:=mean(cs[2]-cs[1]) ...
                  ^

Mari kita plot ini menjadi satu plot sebar.


\>plot2d(cs[1],cs[2],\>points);  ...  
\>   plot2d("evalpoly(x,ps)",color=red,style=".",\>add);  ...  
\>   plot2d("x+da",color=blue,\>add):


    cs is not a variable!
    Error in:
    plot2d(cs[1],cs[2],&gt;points);  plot2d("evalpoly(x,ps)",color=re ...
                ^

Berikut adalah plot kotak dari dua zaman tersebut. Ini hanya
menunjukkan, bahwa usianya berbeda-beda.


\>boxplot(cs,["mothers","fathers"]):


    Variable or function cs not found.
    Error in:
    boxplot(cs,["mothers","fathers"]): ...
              ^

Menariknya, perbedaan median tidak sebesar perbedaan mean.


\>median(cs[2])-median(cs[1])


    cs is not a variable!
    Error in:
    median(cs[2])-median(cs[1]) ...
                ^

Koefisien korelasi menunjukkan korelasi positif.


\>correl(cs[1],cs[2])


    cs is not a variable!
    Error in:
    correl(cs[1],cs[2]) ...
                ^

Korelasi pangkat merupakan ukuran keteraturan yang sama pada kedua
vektor. Hal ini juga cukup positif.


\>rankcorrel(cs[1],cs[2])


    cs is not a variable!
    Error in:
    rankcorrel(cs[1],cs[2]) ...
                    ^

# Membuat Fungsi baru

Tentu saja, bahasa EMT dapat digunakan untuk memprogram fungsi-fungsi
baru. Misalnya, kita mendefinisikan fungsi skewness.


dimana m adalah mean dari x.


\>function skew (x:vector) ...


    m=mean(x);
    return sqrt(cols(x))*sum((x-m)^3)/(sum((x-m)^2))^(3/2);
    endfunction
</pre>
Seperti yang Anda lihat, kita dapat dengan mudah menggunakan bahasa
matriks untuk mendapatkan implementasi yang sangat singkat dan
efisien. Mari kita coba fungsi ini.


\>data=normal(20); skew(normal(10))


    -0.500500593945

Berikut adalah fungsi lainnya, yang disebut koefisien skewness
Pearson.


\>function skew1 (x) := 3\*(mean(x)-median(x))/dev(x)

\>skew1(data)


    -0.00473573537442

# Simulasi Monte Carlo

Euler dapat digunakan untuk mensimulasikan kejadian acak. Kita telah
melihat contoh sederhana di atas. Ini satu lagi, yang mensimulasikan
1000 kali lemparan 3 dadu, dan menanyakan pembagian jumlahnya.


\>ds:=sum(intrandom(1000,3,6))';  fs=getmultiplicities(3:18,ds)


    [4,  17,  25,  40,  52,  85,  118,  145,  130,  124,  110,  70,  39,
    24,  14,  3]

Kita bisa merencanakannya sekarang.


\>columnsplot(fs,lab=3:18):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-676.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-676.png)

Untuk menentukan distribusi yang diharapkan tidaklah mudah. Kami
menggunakan rekursi tingkat lanjut untuk ini.


Fungsi berikut menghitung banyaknya cara bilangan k dapat
direpresentasikan sebagai jumlah dari n bilangan dalam rentang 1
sampai m. Ia bekerja secara rekursif dengan cara yang jelas.


\>function map countways (k; n, m) ...


      if n==1 then return k>=1 && k<=m
      else
        sum=0; 
        loop 1 to m; sum=sum+countways(k-#,n-1,m); end;
        return sum;
      end;
    endfunction
</pre>
Berikut ini hasil dari tiga kali lemparan dadu.


\>countways(5:25,5,5)


    [1,  5,  15,  35,  70,  121,  185,  255,  320,  365,  381,  365,  320,
    255,  185,  121,  70,  35,  15,  5,  1]

\>cw=countways(3:18,3,6)


    [1,  3,  6,  10,  15,  21,  25,  27,  27,  25,  21,  15,  10,  6,  3,
    1]

Kami menambahkan nilai yang diharapkan ke plot.


\>plot2d(cw/6^3\*1000,\>add); plot2d(cw/6^3\*1000,\>points,\>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-677.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-677.png)

Untuk simulasi lain, deviasi nilai rata-rata dari n variabel acak
berdistribusi normal 0-1 adalah 1/akar(n).


\>longformat; 1/sqrt(10)


    0.316227766017

Mari kita periksa ini dengan simulasi. Kita hasilkan 10000 kali 10
vektor acak.


\>M=normal(10000,10); dev(mean(M)')


    0.313795259535

\>plot2d(mean(M)',\>distribution):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-678.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-678.png)

Median dari 10 bilangan acak berdistribusi normal 0-1 memiliki deviasi
yang lebih besar.


\>dev(median(M)')


    0.368587928611

Karena kita dapat dengan mudah menghasilkan lintasan acak, kita dapat
mensimulasikan proses Wiener. Kita mengambil 1000 langkah dari 1000
proses. Kemudian kita memetakan deviasi standar dan rata-rata langkah
ke-n dari proses ini bersama dengan nilai yang diharapkan dalam warna
merah.


\>n=1000; m=1000; M=cumsum(normal(n,m)/sqrt(m)); ...  
\>   t=(1:n)/n; figure(2,1); ...  
\>   figure(1); plot2d(t,mean(M')'); plot2d(t,0,color=red,\>add); ...  
\>   figure(2); plot2d(t,dev(M')'); plot2d(t,sqrt(t),color=red,\>add); ...  
\>   figure(0):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-679.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-679.png)

# Pengujian

Pengujian merupakan alat penting dalam statistik. Dalam Euler, banyak
pengujian yang diterapkan. Semua pengujian ini menghasilkan galat yang
kita terima jika kita menolak hipotesis nol.


Sebagai contoh, kita menguji lemparan dadu untuk distribusi seragam.
Pada 600 lemparan, kita memperoleh nilai berikut, yang kita masukkan
ke dalam uji chi-kuadrat.


\>chitest([90,103,114,101,103,89],dup(100,6)')


    0.498830517952

Uji chi-square juga memiliki modus, yang menggunakan simulasi Monte
Carlo untuk menguji statistik. Hasilnya harus hampir sama. Parameter
&gt;p menginterpretasikan vektor y sebagai vektor probabilitas.


\>chitest([90,103,114,101,103,89],dup(1/6,6)',\>p,\>montecarlo)


    0.509

Kesalahan ini terlalu besar. Jadi kita tidak dapat menolak distribusi
seragam. Ini tidak membuktikan bahwa dadu kita adil. Namun, kita tidak
dapat menolak hipotesis kita.


Selanjutnya, kita menghasilkan 1000 lemparan dadu menggunakan
generator angka acak, dan melakukan pengujian yang sama.


\>n=1000; t=random([1,n\*6]); chitest(count(t\*6,6),dup(n,6)')


    0.753754444313

Mari kita uji nilai rata-rata 100 dengan uji-t.


\>s=200+normal([1,100])\*10; ...  
\>   ttest(mean(s),dev(s),100,200)


    0.275383759442

Fungsi ttest() memerlukan nilai rata-rata, deviasi, jumlah data, dan
nilai rata-rata yang akan diuji.


Sekarang mari kita periksa dua pengukuran untuk nilai rata-rata yang
sama. Kita tolak hipotesis bahwa keduanya memiliki nilai rata-rata
yang sama, jika hasilnya &lt;0,05.


\>tcomparedata(normal(1,10),normal(1,10))


    0.330456077233

Jika kita menambahkan bias pada satu distribusi, kita akan mendapatkan
lebih banyak penolakan. Ulangi simulasi ini beberapa kali untuk
melihat efeknya.


\>tcomparedata(normal(1,10),normal(1,10)+2)


    5.97533459989e-06

Pada contoh berikutnya, kita buat 20 lemparan dadu acak sebanyak 100
kali dan hitung angka-angka yang ada di dalamnya. Rata-rata harus ada
20/6=3,3 angka.


\>R=random(100,20); R=sum(R\*6<=1)'; mean(R)


    3.2

Sekarang kita bandingkan jumlah angka satu dengan distribusi binomial.
Pertama kita gambarkan distribusi angka satu.


\>plot2d(R,distribution=max(R)+1,even=1,style="\\/"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-680.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-680.png)

\>t=count(R,21);


Lalu kami hitung nilai yang diharapkan.


\>n=0:20; b=bin(20,n)\*(1/6)^n\*(5/6)^(20-n)\*100;


Kita harus mengumpulkan beberapa angka untuk mendapatkan kategori yang
cukup besar.


\>t1=sum(t[1:2])|t[3:7]|sum(t[8:21]); ...  
\>   b1=sum(b[1:2])|b[3:7]|sum(b[8:21]);


Uji chi-kuadrat menolak hipotesis bahwa distribusi kami adalah
distribusi binomial, jika hasilnya &lt; 0,05.


\>chitest(t1,b1)


    0.697496276422

Contoh berikut berisi hasil dari dua kelompok orang (misalnya pria dan
wanita) yang memilih satu dari enam partai.


\>A=[23,37,43,52,64,74;27,39,41,49,63,76];  ...  
\>     writetable(A,wc=6,labr=["m","f"],labc=1:6)


               1     2     3     4     5     6
         m    23    37    43    52    64    74
         f    27    39    41    49    63    76

Kami ingin menguji independensi suara dari jenis kelamin. Uji tabel
chi^2 melakukan hal ini. Hasilnya terlalu besar untuk menolak
independensi. Jadi, kami tidak dapat mengatakan, apakah pemungutan
suara bergantung pada jenis kelamin dari data ini.


\>tabletest(A)


    0.990701632326

Berikut ini adalah tabel yang diharapkan, jika kita mengasumsikan
frekuensi pemungutan suara yang diamati.


\>writetable(expectedtable(A),wc=6,dc=1,labr=["m","f"],labc=1:6)


               1     2     3     4     5     6
         m  24.9  37.9  41.9  50.3  63.3  74.7
         f  25.1  38.1  42.1  50.7  63.7  75.3

Kita dapat menghitung koefisien kontingensi yang dikoreksi. Karena
sangat mendekati 0, kita simpulkan bahwa pemungutan suara tidak
bergantung pada jenis kelamin.


\>contingency(A)


    0.0427225484717

# Beberapa Pengujian Lainnya

Selanjutnya, kami menggunakan analisis varians (uji F) untuk menguji
tiga sampel data berdistribusi normal untuk nilai rata-rata yang sama.
Metode ini disebut ANOVA (analisis varians). Dalam Euler, fungsi
varanalysis() digunakan.


\>x1=[109,111,98,119,91,118,109,99,115,109,94]; mean(x1),


    106.545454545

\>x2=[120,124,115,139,114,110,113,120,117]; mean(x2),


    119.111111111

\>x3=[120,112,115,110,105,134,105,130,121,111]; mean(x3)


    116.3

\>varanalysis(x1,x2,x3)


    0.0138048221371

Artinya, kita menolak hipotesis nilai rata-rata yang sama. Kita
melakukan ini dengan probabilitas kesalahan sebesar 1,3%.


Ada juga uji median, yang menolak sampel data dengan distribusi
rata-rata yang berbeda dengan menguji median sampel gabungan.


\>a=[56,66,68,49,61,53,45,58,54];

\>b=[72,81,51,73,69,78,59,67,65,71,68,71];

\>mediantest(a,b)


    0.0241724220052

Uji kesetaraan lainnya adalah uji peringkat. Uji peringkat jauh lebih
tajam daripada uji median.


\>ranktest(a,b)


    0.00199969612469

Dalam contoh berikut, kedua distribusi memiliki rata-rata yang sama.


\>ranktest(random(1,100),random(1,50)\*3-1)


    0.264378760485

Sekarang, mari kita coba simulasikan dua perawatan a dan b yang
diterapkan pada orang yang berbeda.


\>a=[8.0,7.4,5.9,9.4,8.6,8.2,7.6,8.1,6.2,8.9];

\>b=[6.8,7.1,6.8,8.3,7.9,7.2,7.4,6.8,6.8,8.1];


Uji signum memutuskan, apakah a lebih baik dari b.


\>signtest(a,b)


    0.0546875

Ini adalah kesalahan yang sangat besar. Kita tidak dapat menolak bahwa
a sama baiknya dengan b.


Uji Wilcoxon lebih tajam daripada uji ini, tetapi bergantung pada
nilai kuantitatif perbedaannya.


\>wilcoxon(a,b)


    0.0296680599405

Mari kita coba dua pengujian lagi menggunakan seri yang dihasilkan.


\>wilcoxon(normal(1,20),normal(1,20)-1)


    0.00359458419569

\>wilcoxon(normal(1,20),normal(1,20))


    0.910521943401

# Angka Acak

Berikut ini adalah pengujian untuk generator angka acak. Euler
menggunakan generator yang sangat bagus, jadi kita tidak perlu
mengharapkan masalah apa pun.


Pertama-tama kita menghasilkan sepuluh juta angka acak dalam [0,1].


\>n:=10000000; r:=random(1,n);


Berikutnya kita hitung jarak antara dua angka kurang dari 0,05.


\>a:=0.05; d:=differences(nonzeros(r<a));


Terakhir, kami memplot berapa kali setiap jarak terjadi, dan
membandingkannya dengan nilai yang diharapkan.


\>m=getmultiplicities(1:100,d); plot2d(m); ...  
\>     plot2d("n\*(1-a)^(x-1)\*a^2",color=red,\>add):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-681.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-681.png)

Hapus data.


\>remvalue n;


# Pendahuluan bagi Pengguna Proyek R

Jelas, EMT tidak bersaing dengan R sebagai paket statistik. Akan
tetapi, ada banyak prosedur dan fungsi statistik yang tersedia di EMT
juga. Jadi, EMT dapat memenuhi kebutuhan dasar. Lagi pula, EMT
dilengkapi dengan paket numerik dan sistem aljabar komputer.


Buku catatan ini ditujukan bagi Anda yang sudah familier dengan R,
tetapi perlu mengetahui perbedaan sintaksis EMT dan R. Kami mencoba
memberikan gambaran umum tentang hal-hal yang jelas dan kurang jelas
yang perlu Anda ketahui.


Selain itu, kami melihat cara untuk bertukar data antara kedua sistem.


Harap dicatat bahwa ini adalah pekerjaan yang masih dalam tahap
pengerjaan.


# Sintaksis Dasar

Hal pertama yang Anda pelajari di R adalah membuat vektor. Dalam EMT,
perbedaan utamanya adalah operator : dapat mengambil ukuran langkah.
Selain itu, operator ini memiliki daya pengikatan yang rendah.


\>n=10; 0:n/20:n-1


    [0,  0.5,  1,  1.5,  2,  2.5,  3,  3.5,  4,  4.5,  5,  5.5,  6,  6.5,
    7,  7.5,  8,  8.5,  9]

Fungsi c() tidak ada. Dimungkinkan untuk menggunakan vektor guna
menggabungkan berbagai hal.


Contoh berikut ini, seperti banyak contoh lainnya, berasal dari
"Interoduction to R" yang disertakan dalam proyek R. Jika Anda membaca
PDF ini, Anda akan menemukan bahwa saya mengikuti alurnya dalam
tutorial ini.


\>x=[10.4, 5.6, 3.1, 6.4, 21.7]; [x,0,x]


    [10.4,  5.6,  3.1,  6.4,  21.7,  0,  10.4,  5.6,  3.1,  6.4,  21.7]

Operator titik dua dengan ukuran langkah EMT digantikan oleh fungsi
seq() di R. Kita dapat menulis fungsi ini dalam EMT.


\>function seq(a,b,c) := a:b:c; ...  
\>   seq(0,-0.1,-1)


    [0,  -0.1,  -0.2,  -0.3,  -0.4,  -0.5,  -0.6,  -0.7,  -0.8,  -0.9,  -1]

Fungsi rep() dari R tidak ada dalam EMT. Untuk input vektor, dapat
ditulis sebagai berikut.


\>function rep(x:vector,n:index) := flatten(dup(x,n)); ...  
\>   rep(x,2)


    [10.4,  5.6,  3.1,  6.4,  21.7,  10.4,  5.6,  3.1,  6.4,  21.7]

Perhatikan bahwa "=" atau ":=" digunakan untuk penugasan. Operator
"-&gt;" digunakan untuk unit dalam EMT.


\>125km -\> " miles"


    77.6713990297 miles

Operator "&lt;-" untuk penugasan menyesatkan dan bukan ide yang baik
untuk R. Berikut ini akan membandingkan a dan -4 dalam EMT.


\>a=2; a<-4


    0

Dalam R, "a&lt;-4&lt;3" berfungsi, tetapi "a&lt;-4&lt;-3" tidak. Saya juga
mengalami ambiguitas serupa dalam EMT, tetapi mencoba menghilangkannya
sedikit demi sedikit.


EMT dan R memiliki vektor bertipe boolean. Namun dalam EMT, angka 0
dan 1 digunakan untuk mewakili false dan true. Dalam R, nilai true dan
false tetap dapat digunakan dalam aritmatika biasa seperti dalam EMT.


\>x<5, %\*x


    [0,  0,  1,  0,  0]
    [0,  0,  3.1,  0,  0]

EMT memunculkan kesalahan atau menghasilkan NAN, tergantung pada tanda
"kesalahan".


\>errors off; 0/0, isNAN(sqrt(-1)), errors on;


    NAN
    1

String sama di R dan EMT. Keduanya berada di lokal saat ini, bukan di
Unicode.


Di R ada paket untuk Unicode. Di EMT, string dapat berupa string
Unicode. String unicode dapat diterjemahkan ke pengodean lokal dan
sebaliknya. Selain itu, u"..." dapat berisi entitas HTML.


\>u"&#169; Ren&eacut; Grothmann"


    © René Grothmann

Berikut ini mungkin atau mungkin tidak ditampilkan dengan benar pada
sistem Anda sebagai A dengan titik dan garis di atasnya. Hal ini
bergantung pada font yang Anda gunakan.


\>chartoutf([480])


    Ǡ

Penggabungan string dilakukan dengan "+" atau "|". String dapat
menyertakan angka, yang akan dicetak dalam format saat ini.


\>"pi = "+pi


    pi = 3.14159265359

# Pengindeksan

Sering kali, ini akan berfungsi seperti di R.


Namun EMT akan menginterpretasikan indeks negatif dari belakang
vektor, sementara R menginterpretasikan x[n] sebagai x tanpa elemen
ke-n.


\>x, x[1:3], x[-2]


    [10.4,  5.6,  3.1,  6.4,  21.7]
    [10.4,  5.6,  3.1]
    6.4

Perilaku R dapat dicapai dalam EMT dengan drop().


\>drop(x,2)


    [10.4,  3.1,  6.4,  21.7]

Vektor logika tidak diperlakukan secara berbeda sebagai indeks dalam
EMT, berbeda dengan R. Anda perlu mengekstrak elemen bukan nol
terlebih dahulu dalam EMT.


\>x, x\>5, x[nonzeros(x\>5)]


    [10.4,  5.6,  3.1,  6.4,  21.7]
    [1,  1,  0,  1,  1]
    [10.4,  5.6,  6.4,  21.7]

Sama seperti di R, vektor indeks dapat berisi pengulangan.


\>x[[1,2,2,1]]


    [10.4,  5.6,  5.6,  10.4]

Namun, nama untuk indeks tidak dimungkinkan dalam EMT. Untuk paket
statistik, hal ini mungkin sering diperlukan untuk memudahkan akses ke
elemen vektor.


Untuk meniru perilaku ini, kita dapat mendefinisikan fungsi sebagai
berikut.


\>function sel (v,i,s) := v[indexof(s,i)]; ...  
\>   s=["first","second","third","fourth"]; sel(x,["first","third"],s)


    
    Trying to overwrite protected function sel!
    Error in:
    function sel (v,i,s) := v[indexof(s,i)]; ... ...
                 ^
    
    Trying to overwrite protected function sel!
    Error in:
    function sel (v,i,s) := v[indexof(s,i)]; ... ...
                 ^
    [10.4,  3.1]

# Tipe Data

EMT memiliki lebih banyak tipe data tetap daripada R. Jelas, di R
terdapat vektor yang terus bertambah. Anda dapat menetapkan vektor
numerik kosong v dan menetapkan nilai ke elemen v[17]. Hal ini tidak
mungkin dilakukan di EMT.


Berikut ini agak tidak efisien.


\>v=[]; for i=1 to 10000; v=v|i; end;


EMT sekarang akan membuat vektor dengan v dan i yang ditambahkan pada
tumpukan dan menyalin vektor itu kembali ke variabel global v.


Yang lebih efisien mendefinisikan vektor terlebih dahulu.


\>v=zeros(10000); for i=1 to 10000; v[i]=i; end;


Yang lebih efisien mendefinisikan vektor terlebih dahulu.


\>complex(1:4)


    [ 1+0i ,  2+0i ,  3+0i ,  4+0i  ]

Konversi ke string hanya dimungkinkan untuk tipe data dasar. Format
saat ini digunakan untuk penggabungan string sederhana. Namun, ada
fungsi seperti print() atau frac().


Untuk vektor, Anda dapat dengan mudah menulis fungsi Anda sendiri.


\>function tostr (v) ...


    s="[";
    loop 1 to length(v);
       s=s+print(v[#],2,0);
       if #<length(v) then s=s+","; endif;
    end;
    return s+"]";
    endfunction
</pre>
\>tostr(linspace(0,1,10))


    [0.00,0.10,0.20,0.30,0.40,0.50,0.60,0.70,0.80,0.90,1.00]

Untuk komunikasi dengan Maxima, terdapat fungsi convertmxm(), yang
juga dapat digunakan untuk memformat vektor untuk keluaran.


\>convertmxm(1:10)


    [1,2,3,4,5,6,7,8,9,10]

Untuk Latex perintah tex dapat digunakan untuk mendapatkan perintah
Latex.


\>tex(&[1,2,3])


    \left[ 1 , 2 , 3 \right] 

# Faktor dan Tabel

Dalam pengantar R terdapat contoh dengan apa yang disebut faktor.


Berikut ini adalah daftar wilayah dari 30 negara bagian.


\>austates = ["tas", "sa", "qld", "nsw", "nsw", "nt", "wa", "wa", ...  
\>   "qld", "vic", "nsw", "vic", "qld", "qld", "sa", "tas", ...  
\>   "sa", "nt", "wa", "vic", "qld", "nsw", "nsw", "wa", ...  
\>   "sa", "act", "nsw", "vic", "vic", "act"];


Asumsikan, kita memiliki pendapatan yang sesuai di setiap negara
bagian.


\>incomes = [60, 49, 40, 61, 64, 60, 59, 54, 62, 69, 70, 42, 56, ...  
\>   61, 61, 61, 58, 51, 48, 65, 49, 49, 41, 48, 52, 46, ...  
\>   59, 46, 58, 43];


Sekarang, kita ingin menghitung rata-rata pendapatan di wilayah
tersebut. Sebagai program statistik, R memiliki factor() dan tappy()
untuk ini.


EMT dapat melakukan ini dengan menemukan indeks wilayah dalam daftar
wilayah yang unik.


\>auterr=sort(unique(austates)); f=indexofsorted(auterr,austates)


    [6,  5,  4,  2,  2,  3,  8,  8,  4,  7,  2,  7,  4,  4,  5,  6,  5,  3,
    8,  7,  4,  2,  2,  8,  5,  1,  2,  7,  7,  1]

Pada titik tersebut, kita dapat menulis fungsi loop kita sendiri untuk
melakukan sesuatu hanya untuk satu faktor.


Atau kita dapat meniru fungsi tapply() dengan cara berikut.


\>function map tappl (i; f$:call, cat, x) ...


    u=sort(unique(cat));
    f=indexof(u,cat);
    return f$(x[nonzeros(f==indexof(u,i))]);
    endfunction
</pre>
Agak tidak efisien, karena menghitung wilayah unik untuk setiap i,
tetapi berhasil.


\>tappl(auterr,"mean",austates,incomes)


    [44.5,  57.3333333333,  55.5,  53.6,  55,  60.5,  56,  52.25]

Perhatikan bahwa ini berfungsi untuk setiap vektor wilayah.


\>tappl(["act","nsw"],"mean",austates,incomes)


    [44.5,  57.3333333333]

Sekarang, paket statistik EMT mendefinisikan tabel seperti di R.
Fungsi readtable() dan writetable() dapat digunakan untuk input dan
output.


Jadi kita dapat mencetak pendapatan negara rata-rata di wilayah dengan
cara yang mudah.


\>writetable(tappl(auterr,"mean",austates,incomes),labc=auterr,wc=7)


        act    nsw     nt    qld     sa    tas    vic     wa
       44.5  57.33   55.5   53.6     55   60.5     56  52.25

Kita juga dapat mencoba meniru perilaku R sepenuhnya.


Faktor-faktor tersebut harus disimpan dalam suatu koleksi dengan jenis
dan kategori (negara bagian dan teritori dalam contoh kita). Untuk
EMT, kita tambahkan indeks yang telah dihitung sebelumnya.


\>function makef (t) ...


    ## Factor data
    ## Returns a collection with data t, unique data, indices.
    ## See: tapply
    u=sort(unique(t));
    return {{t,u,indexofsorted(u,t)}};
    endfunction
</pre>
\>statef=makef(austates);


Sekarang elemen ketiga dari koleksi akan berisi indeks.


\>statef[3]


    [6,  5,  4,  2,  2,  3,  8,  8,  4,  7,  2,  7,  4,  4,  5,  6,  5,  3,
    8,  7,  4,  2,  2,  8,  5,  1,  2,  7,  7,  1]

Sekarang kita dapat meniru tapply() dengan cara berikut. Fungsi ini
akan mengembalikan tabel sebagai kumpulan data tabel dan judul kolom.


\>function tapply (t:vector,tf,f$:call) ...


    ## Makes a table of data and factors
    ## tf : output of makef()
    ## See: makef
    uf=tf[2]; f=tf[3]; x=zeros(length(uf));
    for i=1 to length(uf);
       ind=nonzeros(f==i);
       if length(ind)==0 then x[i]=NAN;
       else x[i]=f$(t[ind]);
       endif;
    end;
    return {{x,uf}};
    endfunction
</pre>
Kami tidak menambahkan banyak pemeriksaan tipe di sini. Satu-satunya
tindakan pencegahan menyangkut kategori (faktor) tanpa data. Namun,
seseorang harus memeriksa panjang t yang benar dan kebenaran koleksi
tf.


Tabel ini dapat dicetak sebagai tabel dengan writetable().


\>writetable(tapply(incomes,statef,"mean"),wc=7)


        act    nsw     nt    qld     sa    tas    vic     wa
       44.5  57.33   55.5   53.6     55   60.5     56  52.25

# Array

EMT hanya memiliki dua dimensi untuk array. Tipe data ini disebut
matriks. Akan mudah untuk menulis fungsi untuk dimensi yang lebih
tinggi atau pustaka C untuk ini.


R memiliki lebih dari dua dimensi. Dalam R, array adalah vektor dengan
bidang dimensi.


Dalam EMT, vektor adalah matriks dengan satu baris. Vektor dapat
dibuat menjadi matriks dengan redim().


\>shortformat; X=redim(1:20,4,5)


            1         2         3         4         5 
            6         7         8         9        10 
           11        12        13        14        15 
           16        17        18        19        20 

Ekstraksi baris dan kolom, atau sub-matriks, sangat mirip di R.


\>X[,2:3]


            2         3 
            7         8 
           12        13 
           17        18 

Namun, dalam R dimungkinkan untuk menetapkan daftar indeks vektor
tertentu ke suatu nilai. Hal yang sama dimungkinkan dalam EMT hanya
dengan loop.


\>function setmatrixvalue (M, i, j, v) ...


    loop 1 to max(length(i),length(j),length(v))
       M[i{#},j{#}] = v{#};
    end;
    endfunction
</pre>
Kami mendemonstrasikan ini untuk menunjukkan bahwa matriks dilewatkan
dengan referensi dalam EMT. Jika Anda tidak ingin mengubah matriks
asli M, Anda perlu menyalinnya dalam fungsi tersebut.


\>setmatrixvalue(X,1:3,3:-1:1,0); X,


            1         2         0         4         5 
            6         0         8         9        10 
            0        12        13        14        15 
           16        17        18        19        20 

Produk luar dalam EMT hanya dapat dilakukan antara vektor. Hal ini
dilakukan secara otomatis karena bahasa matriks. Satu vektor harus
berupa vektor kolom dan yang lainnya berupa vektor baris.


\>(1:5)\*(1:5)'


            1         2         3         4         5 
            2         4         6         8        10 
            3         6         9        12        15 
            4         8        12        16        20 
            5        10        15        20        25 

Dalam pengantar PDF untuk R terdapat sebuah contoh, yang menghitung
distribusi ab-cd untuk a,b,c,d yang dipilih secara acak dari 0 hingga
n. Solusi dalam R adalah membentuk matriks 4 dimensi dan menjalankan
table() di atasnya.


Tentu saja, ini dapat dicapai dengan loop. Namun, loop tidak efektif
dalam EMT atau R. Dalam EMT, kita dapat menulis loop dalam C dan itu
akan menjadi solusi tercepat.


Namun, kita ingin meniru perilaku R. Untuk ini, kita perlu meratakan
perkalian ab dan membuat matriks ab-cd.


\>a=0:6; b=a'; p=flatten(a\*b); q=flatten(p-p'); ...  
\>   u=sort(unique(q)); f=getmultiplicities(u,q); ...  
\>   statplot(u,f,"h"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-682.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-682.png)

Selain multiplisitas yang tepat, EMT dapat menghitung frekuensi dalam
vektor.


\>getfrequencies(q,-50:10:50)


    [0,  23,  132,  316,  602,  801,  333,  141,  53,  0]

Cara termudah untuk memplot ini sebagai distribusi adalah sebagai
berikut.


\>plot2d(q,distribution=11):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-683.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-683.png)

Namun, Anda juga dapat menghitung terlebih dahulu jumlah dalam
interval yang dipilih. Tentu saja, berikut ini menggunakan
getfrequencies() secara internal.


Karena fungsi histo() mengembalikan frekuensi, kita perlu
menskalakannya sehingga integral di bawah grafik batang adalah 1.


\>{x,y}=histo(q,v=-55:10:55); y=y/sum(y)/differences(x); ...  
\>   plot2d(x,y,\>bar,style="/"):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-684.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-684.png)

# Daftar

EMT memiliki dua jenis daftar. Satu adalah daftar global yang dapat
diubah, dan yang lainnya adalah jenis daftar yang tidak dapat diubah.
Kami tidak peduli dengan daftar global di sini.


Jenis daftar yang tidak dapat diubah disebut koleksi dalam EMT. Ia
berperilaku seperti struktur dalam C, tetapi elemennya hanya diberi
nomor dan tidak diberi nama.


\>L={{"Fred","Flintstone",40,[1990,1992]}}


    Fred
    Flintstone
    40
    [1990,  1992]

Saat ini unsur-unsur tersebut tidak memiliki nama, meskipun nama dapat
ditetapkan untuk tujuan khusus. Unsur-unsur tersebut diakses dengan
angka.


\>(L[4])[2]


    1992

# Input dan Output File (Membaca dan Menulis Data)

Anda sering kali ingin mengimpor matriks data dari sumber lain ke EMT.
Tutorial ini memberi tahu Anda tentang berbagai cara untuk
mencapainya. Fungsi sederhana adalah writematrix() dan readmatrix().


Mari kita tunjukkan cara membaca dan menulis vektor bilangan real ke
dalam file.


\>a=random(1,100); mean(a), dev(a),


    0.4789
    0.27521

Untuk menulis data ke dalam berkas, kami menggunakan fungsi
writematrix().


Karena pengantar ini kemungkinan besar berada di dalam direktori,
tempat pengguna tidak memiliki akses tulis, kami menulis data ke
direktori beranda pengguna. Untuk buku catatan sendiri, ini tidak
diperlukan, karena berkas data akan ditulis ke dalam direktori yang
sama.


\>filename="test.dat";


Sekarang kita tulis vektor kolom a' ke dalam berkas. Ini menghasilkan
satu angka di setiap baris berkas.


\>writematrix(a',filename);


Untuk membaca data, kita menggunakan readmatrix().


\>a=readmatrix(filename)';


Dan hapus berkasnya.


\>fileremove(filename);

\>mean(a), dev(a),


    0.4789
    0.27521

Fungsi writematrix() atau writetable() dapat dikonfigurasi untuk
bahasa lain.


Misalnya, jika Anda memiliki sistem bahasa Indonesia (titik desimal
dengan koma), Excel Anda memerlukan nilai dengan koma desimal yang
dipisahkan oleh titik koma dalam file csv (nilai default dipisahkan
dengan koma). File berikut "test.csv" akan muncul di folder Anda saat
ini.


\>filename="test.csv"; ...  
\>   writematrix(random(5,3),file=filename,separator=",");


Anda sekarang dapat membuka berkas ini langsung dengan Excel
Indonesia.


\>fileremove(filename);


Terkadang kita memiliki string dengan token seperti berikut.


\>s1:="f m m f m m m f f f m m f";  ...  
\>   s2:="f f f m m f f";


Untuk menokenisasi ini, kami mendefinisikan vektor token.


\>tok:=["f","m"]


    f
    m

Lalu kita dapat menghitung berapa kali setiap token muncul dalam
string, dan memasukkan hasilnya ke dalam tabel.


\>M:=getmultiplicities(tok,strtokens(s1))\_ ...  
\>     getmultiplicities(tok,strtokens(s2));


Tulis tabel dengan tajuk token.


\>writetable(M,labc=tok,labr=1:2,wc=8)


                   f       m
           1       6       7
           2       5       2

Untuk statika, EMT dapat membaca dan menulis tabel.


\>file="test.dat"; open(file,"w"); ...  
\>   writeln("A,B,C"); writematrix(random(3,3)); ...  
\>   close();


Berkasnya tampak seperti ini.


\>printfile(file)


    A,B,C
    0.6210691015193581,0.1861287498944177,0.1334118765499487
    0.5425891336612759,0.8541459276352096,0.5265435039793132
    0.8286381971250506,0.9319592738601091,0.9548321883942634
    

Fungsi readtable() dalam bentuk yang paling sederhana dapat membacanya
dan mengembalikan kumpulan nilai dan baris judul.


\>L=readtable(file,\>list);


Koleksi ini dapat dicetak dengan writetable() ke buku catatan, atau ke
berkas.


\>writetable(L,wc=10,dc=5)


             A         B         C
       0.62107   0.18613   0.13341
       0.54259   0.85415   0.52654
       0.82864   0.93196   0.95483

Matriks nilai adalah elemen pertama L. Perhatikan bahwa mean() dalam
EMT menghitung nilai rata-rata baris matriks.


\>mean(L[1])


      0.31354 
      0.64109 
      0.90514 

# Berkas CSV

Pertama, mari kita tulis matriks ke dalam berkas. Untuk output, kita
buat berkas di direktori kerja saat ini.


\>file="test.csv";  ...  
\>   M=random(3,3); writematrix(M,file);


Berikut ini isi berkas tersebut.


\>printfile(file)


    0.5509346722762319,0.9591222272838416,0.1515283397770994
    0.7091161391115151,0.5510213984347968,0.163059576815024
    0.3482813265192847,0.6028612820632797,0.4552416781408445
    

CVS ini dapat dibuka pada sistem bahasa Inggris ke Excel dengan
mengklik dua kali. Jika Anda mendapatkan berkas tersebut pada sistem
bahasa Jerman, Anda perlu mengimpor data ke Excel dengan memperhatikan
titik desimal.


Namun, titik desimal juga merupakan format default untuk EMT. Anda
dapat membaca matriks dari berkas dengan readmatrix().


\>readmatrix(file)


      0.55093   0.95912   0.15153 
      0.70912   0.55102   0.16306 
      0.34828   0.60286   0.45524 

Dimungkinkan untuk menulis beberapa matriks ke dalam satu berkas.
Perintah open() dapat membuka berkas untuk ditulis dengan parameter
"w". Nilai default untuk membaca adalah "r".


\>open(file,"w"); writematrix(M); writematrix(M'); close();


Matriks dipisahkan oleh baris kosong. Untuk membaca matriks, buka
berkas dan panggil readmatrix() beberapa kali.


\>open(file); A=readmatrix(); B=readmatrix(); A==B, close();


            1         0         0 
            0         1         0 
            0         0         1 

Di Excel atau lembar kerja serupa, Anda dapat mengekspor matriks
sebagai CSV (nilai yang dipisahkan koma). Di Excel 2007, gunakan
"simpan sebagai" dan "format lain", lalu pilih "CSV". Pastikan, tabel
saat ini hanya berisi data yang ingin Anda ekspor.


Berikut ini contohnya.


\>printfile("excel-data.csv")


    Could not open the file
    excel-data.csv
    for reading!
    Try "trace errors" to inspect local variables after errors.
    printfile:
        open(filename,"r");

Seperti yang Anda lihat, sistem Jerman saya menggunakan titik koma
sebagai pemisah dan koma desimal. Anda dapat mengubahnya di pengaturan
sistem atau di Excel, tetapi tidak diperlukan untuk membaca matriks ke
EMT.


Cara termudah untuk membaca ini ke Euler adalah readmatrix(). Semua
koma diganti dengan titik dengan parameter &gt;comma. Untuk CSV bahasa
Inggris, cukup abaikan parameter ini.


\>M=readmatrix("excel-data.csv",\>comma)


    Could not open the file
    excel-data.csv
    for reading!
    Try "trace errors" to inspect local variables after errors.
    readmatrix:
        if filename&lt;&gt;"" then open(filename,"r"); endif;

Mari kita plot ini.


\>plot2d(M'[1],M'[2:3],\>points,color=[red,green]'):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-685.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-685.png)

Ada cara yang lebih mendasar untuk membaca data dari sebuah berkas.
Anda dapat membuka berkas dan membaca angka baris demi baris. Fungsi
getvectorline() akan membaca angka dari sebaris data. Secara default,
fungsi ini mengharapkan titik desimal. Namun, fungsi ini juga dapat
menggunakan koma desimal, jika Anda memanggil setdecimaldot(",")
sebelum menggunakan fungsi ini.


Fungsi berikut adalah contohnya. Fungsi ini akan berhenti di akhir
berkas atau baris kosong.


\>function myload (file) ...


    open(file);
    M=[];
    repeat
       until eof();
       v=getvectorline(3);
       if length(v)>0 then M=M_v; else break; endif;
    end;
    return M;
    close(file);
    endfunction
</pre>
\>myload(file)


      0.55093         0   0.95912         0   0.15153 
      0.70912         0   0.55102         0   0.16306 
      0.34828         0   0.60286         0   0.45524 

Semua angka dalam berkas itu juga dapat dibaca dengan getvector().


\>open(file); v=getvector(10000); close(); redim(v[1:9],3,3)


      0.55093         0   0.95912 
            0   0.15153   0.70912 
            0   0.55102         0 

Jadi sangat mudah untuk menyimpan vektor nilai, satu nilai di setiap
baris dan membaca kembali vektor ini.


\>v=random(1000); mean(v)


    0.49382

\>writematrix(v',file); mean(readmatrix(file)')


    0.49382

# Menggunakan Tabel

Tabel dapat digunakan untuk membaca atau menulis data numerik.
Misalnya, kita menulis tabel dengan tajuk baris dan kolom ke dalam
sebuah berkas.


\>file="test.tab"; M=random(3,3);  ...  
\>   open(file,"w");  ...  
\>   writetable(M,separator=",",labc=["one","two","three"]);  ...  
\>   close(); ...  
\>   printfile(file)


    one,two,three
          0.04,      0.02,      0.96
          0.54,      0.09,      0.87
          0.13,      0.41,       0.9

Ini dapat diimpor ke Excel.


Untuk membaca berkas di EMT, kami menggunakan readtable().


\>{M,headings}=readtable(file,\>clabs); ...  
\>   writetable(M,labc=headings)


           one       two     three
          0.04      0.02      0.96
          0.54      0.09      0.87
          0.13      0.41       0.9

# Menganalisis Garis

Anda bahkan dapat mengevaluasi setiap garis secara manual. Misalkan,
kita memiliki garis dengan format berikut.


\>line="2020-11-03,Tue,1'114.05"


    2020-11-03,Tue,1'114.05

Pertama, kita dapat membuat token pada baris tersebut.


\>vt=strtokens(line)


    2020-11-03
    Tue
    1'114.05

Kemudian kita dapat mengevaluasi setiap elemen garis menggunakan
evaluasi yang tepat.


\>day(vt[1]),  ...  
\>   indexof(["mon","tue","wed","thu","fri","sat","sun"],tolower(vt[2])),  ...  
\>   strrepl(vt[3],"'","")()


    7.3816e+05
    2
    1114

Dengan menggunakan ekspresi reguler, dimungkinkan untuk mengekstrak
hampir semua informasi dari sebaris data.


Asumsikan kita memiliki baris berikut sebagai dokumen HTML.


\>line="<tr\><td\>1145.45</td\><td\>5.6</td\><td\>-4.5</td\><tr\>"


    &lt;tr&gt;&lt;td&gt;1145.45&lt;/td&gt;&lt;td&gt;5.6&lt;/td&gt;&lt;td&gt;-4.5&lt;/td&gt;&lt;tr&gt;

Untuk mengekstraknya, kami menggunakan ekspresi reguler, yang mencari


* 
tanda kurung tutup &gt;,

* 
string apa pun yang tidak mengandung tanda kurung dengan
* sub-kecocokan "(...)",

* 
tanda kurung buka dan tutup menggunakan solusi terpendek,

* 
lagi-lagi string apa pun yang tidak mengandung tanda kurung,

* 
dan tanda kurung buka &lt;.


Ekspresi reguler agak sulit dipelajari tetapi sangat ampuh.


\>{pos,s,vt}=strxfind(line,"\>([^<\>]+)<.+?\>([^<\>]+)<");


Hasilnya adalah posisi kecocokan, string yang cocok, dan vektor string
untuk sub-kecocokan.


\>for k=1:length(vt); vt[k](), end;


    1145.5
    5.6

Berikut adalah fungsi yang membaca semua item numerik antara &lt;td&gt; dan
&lt;/td&gt;.


\>function readtd (line) ...


    v=[]; cp=0;
    repeat
       {pos,s,vt}=strxfind(line,"<td.*?>(.+?)</td>",cp);
       until pos==0;
       if length(vt)>0 then v=v|vt[1]; endif;
       cp=pos+strlen(s);
    end;
    return v;
    endfunction
</pre>
\>readtd(line+"<td\>non-numerical</td\>")


    1145.45
    5.6
    -4.5
    non-numerical

# Membaca dari Web

Situs web atau berkas dengan URL dapat dibuka di EMT dan dapat dibaca
baris demi baris.


Dalam contoh ini, kami membaca versi terkini dari situs EMT. Kami
menggunakan ekspresi reguler untuk memindai "Versi ..." dalam judul.


\>function readversion () ...


    urlopen("http://www.euler-math-toolbox.de/Programs/Changes.html");
    repeat
      until urleof();
      s=urlgetline();
      k=strfind(s,"Version ",1);
      if k>0 then substring(s,k,strfind(s,"<",k)-1), break; endif;
    end;
    urlclose();
    endfunction
</pre>
\>readversion


    Version 2024-01-12

# Input dan Output Variabel

Anda dapat menulis variabel dalam bentuk definisi Euler ke dalam file
atau ke baris perintah.


\>writevar(pi,"mypi");


    mypi = 3.141592653589793;

Untuk pengujian, kami membuat file Euler di direktori kerja EMT.


\>file="test.e"; ...  
\>   writevar(random(2,2),"M",file); ...  
\>   printfile(file,3)


    M = [ ..
    0.4623879917445496, 0.3180836434648883;
    0.3529402068815742, 0.781744142737357];

Sekarang kita dapat memuat berkas tersebut. Berkas tersebut akan
mendefinisikan matriks M.


\>load(file); show M,


    M = 
      0.46239   0.31808 
      0.35294   0.78174 

Ngomong-ngomong, jika writevar() digunakan pada suatu variabel, ia
akan mencetak definisi variabel dengan nama variabel ini.


\>writevar(M); writevar(inch$)


    M = [ ..
    0.4623879917445496, 0.3180836434648883;
    0.3529402068815742, 0.781744142737357];
    inch$ = 0.0254;

Kita juga dapat membuka berkas baru atau menambahkannya ke berkas yang
sudah ada. Dalam contoh ini, kita menambahkannya ke berkas yang dibuat
sebelumnya.


\>open(file,"a"); ...  
\>   writevar(random(2,2),"M1"); ...  
\>   writevar(random(3,1),"M2"); ...  
\>   close();

\>load(file); show M1; show M2;


    M1 = 
      0.44086   0.37666 
      0.12362   0.26942 
    M2 = 
      0.87284 
      0.40248 
      0.78955 

Untuk menghapus file apa pun gunakan fileremove().


\>fileremove(file);


Vektor baris dalam sebuah berkas tidak memerlukan koma, jika setiap
angka berada di baris baru. Mari kita buat berkas seperti itu, tulis
setiap baris satu per satu dengan writeln().


\>open(file,"w"); writeln("M = ["); ...  
\>   for i=1 to 5; writeln(""+random()); end; ...  
\>   writeln("];"); close(); ...  
\>   printfile(file)


    M = [
    0.234994356974
    0.183264664178
    0.755219384652
    0.602458087359
    0.543445468039
    ];

\>load(file); M


    [0.23499,  0.18326,  0.75522,  0.60246,  0.54345]

catatan : ketika mengenter perintah-perintah diatas ternyata hasil
yang didapatkan berbeda-beda


# Latihan soal 

Nomor 1 Carilah rata-rata dan standar deviasi beserta plot dari data
berikut


X = 2000,2500,2700,3500,4500,5000


\>X=[2000,2500,2700,3500,4500,5000]; ...  
\>   mean(X), dev(X),


    3366.7
    1186

\>aspect(1.5); boxplot(X):


![images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-686.png](images/23030630043_Nadzwa%20Sri%20Azijzah_MatE23_LaTex%20Mardown_Pertemuan%2015&16-686.png)

Nomor 2


Misalkan diberikan data skor hasil statistika dari 20 orang mahasiswa
sebagai berikut:


70,65,79,90,60,79,86,95,100,70,60,91,68,84,59,90,88,84,86,90


Tentukan rata-rata dari data tersebut!


\>X=[70,65,79,90,60,79,86,95,100,70,60,91,68,84,59,90,88,84,86,90]


    [70,  65,  79,  90,  60,  79,  86,  95,  100,  70,  60,  91,  68,  84,
    59,  90,  88,  84,  86,  90]

\>mean(X)


    79.7

\>               


    
    
    
</pre>
\>   


    

<pre class="udf">    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
</pre>
