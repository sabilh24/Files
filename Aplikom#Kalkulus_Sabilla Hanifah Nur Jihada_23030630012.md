﻿# Aplikom#Kalkulus_Sabilla Hanifah Nur Jihada_23030630012
## Tugas Aplikasi Komputer Pekan ke 9 dan 10 :

Nama: Sabilla Hanifah Nur Jihada


NIM: 23030630012


# Kalkulus dengan EMT

Materi Kalkulus mencakup di antaranya:


1. Fungsi(fungsi aljabar, trigonometri, eksponensial, logaritma,
komposisi fungsi)


2. Limit Fungsi


3. Turunan Fungsi


4. Integral Tak Tentu


5. Integral Tentu


6. Barisan dan Deret


7. Fungsi multivariabel


EMT (bersama Maxima) dapat digunakan untuk melakukan semua perhitungan
di dalam kalkulus, baik secara numerik maupun analitik (eksak).


# 1. Fungsi

Fungsi adalah suatu relasi yang menghubungkan setiap anggota dari
suatu himpunan (domain) dengan tepat satu anggota himpunan lain
(kodomain). Secara sederhana, fungsi dapat dipandang sebagai mesin
yang menerima input (nilai x) dan menghasilkan output (nilai y).


$$f: A \to B$$## Sifat-sifat Fungsi

1. Injektif (satu-satu)


Fungsi injektif adalah fungsi degan tiap elemen kondomain tidak
memiliki lebih dari satu elemen domain. Fungsi injektif disebut juga
dengan "fungsi satu-satu" karena tiap elemen kodomain hanya boleh
berelasi satu kali.


2. Surjektif


Fungsi surjektif adalah fungsi dengan semua elemen kodomain berelasi
dengan elemen domain. Fungsi surjektif juga disebut fungsi "on-to".


3. Bijektif


Fungsi bijektif adalah fungsi yang memenuhi sifat injektif dan
surjektif. Fungsi bijektif juga disebut fungsi korespondensi
satu-satu, karena elemen domain dan kodomain semuanya berelasi
satu-satu.


## Jenis Fungsi yang akan Dielajari

1. Fungsi Aljabar


Fungsi aljabar adalah jenis fungsi matematika yang dibentuk dengan
menggunakan operasi-operasi aljabar seperti penjumlahan, pengurangan,
perkalian, pembagian, dan pangkat. Secara umum, fungsi aljabar
merupakan fungsi yang dapat dinyatakan dengan ekspresi aljabar yang
melibatkan variabel dan konstanta. Fungsi ini termasuk di dalam
kategori fungsi elementer karena bisa dinyatakan dalam bentuk dasar.


2. Fungsi Trigonometri


Fungsi trigonometri adalah fungsi yang menghubungkan sudut suatu
segitiga siku-siku dengan rasio panjang sisi-sisinya. Fungsi ini
sangat penting dalam matematika, khususnya dalam geometri, analisis,
dan aplikasi di bidang fisika, teknik, dan astronomi. Fungsi-fungsi
trigonometri yang paling umum adalah sinus, kosinus, tangen, serta
turunan dan kebalikannya seperti secan, kosekan, dan kotangen.


3. Fungsi Eksponensial


Fungsi eksponensial adalah fungsi matematika di mana variabel
independen (biasanya dilambangkan dengan x) berada di eksponen. Bentuk
umum fungsi eksponensial adalah:


$$f(x)=a^x$$* 
a adalah bilangan positif (basis) dan tidak sama dengan 1

* 
x adalah variabel eksponen


Fungsi eksponensial yang paling umum adalah fungsi eksponensial alami
dengan basis bilangan euler (e = 2.718). Fungsi ini sering digunakan
dalam berbagai aplikasi ilmiah yang dinyatakan sebagai:


$$f(x)=e^x$$4. Fungsi Logaritma


Fungsi logaritma adalah kebalikan atau invers dari fungsi
eksponensial. Fungsi logaritma dinyatakan sebagai:


$$f(x)= \log a(x)$$5. Komposisi Fungsi


Komposisi fungsi adalah operasi matematika di mana dua fungsi
digabungkan sehingga output dari satu fungsi menjadi input dari fungsi
yang lain.


Misal, diketahui f dan g dua fungsi sebarang maka fungsi komposisi f
dan g ditulis


$$g o f$$

didefinisikan sebagai:


$$(g o f)(x) = g(f(x))$$sehingga fungsi f dikerjakan terlebih dahulu daripada g.


## Mendefinisikan Fungsi

Terdapat beberapa cara mendefinisikan fungsi pada EMT, yakni:


* 
Menggunakan format nama_fungsi := rumus fungsi (fungsi numerik),

* 
Menggunakan format nama_fungsi &amp;= rumus fungsi (fungsi simbolik,
* namun dapat dihitung secara numerik),

* 
Menggunakan format nama_fungsi &amp;&amp;= rumus fungsi(fungsi simbolik
* murni, tidak dapat dihitung langsung),

* 
Fungsi sebagai program EMT (Mendefinisikan fungsi yang lebih
* kompleks dengan beberapa langkah atau percabangan)


Setiap format harus diawali dengan perintah function (bukan sebagai
ekspresi).


Berikut adalah adalah beberapa contoh cara mendefinisikan fungsi:


$$f(x)=2x^2+e^{\sin(x)}.$$\>function f(x) := 2\*x^2+exp(sin(x)) // fungsi numerik 


fungsi ini mendefinisikan nilai dari f(x) dan untuk fungsi exp(cox(x))
merupakan dua fungsi dimana:


cos(x)  digunakan untuk menghitung nilai cos di sudut x dan exp()
digunakan untuk mendefinisikan fungsi eksponensial (e pangkat)


\>f(0), f(1), f(pi)


    1
    4.31977682472
    20.7392088022

\>f(a) // tidak dapat dihitung nilainya karena bukan fungsi numerik


    288.584748804

$$f(x)=3x^3+e^{\cos(x)}.$$\>function f(x) := 3\*x^3+exp(cos(x))  

\>f(1)


    4.71652569955

\>f(2)


    24.6595834124

\>f(-2:2)


    [-23.3404,  -1.28347,  2.71828,  4.71653,  24.6596]

\>f(-2)-f(2)


    -48

\>plot2d("f(x)",-2,2):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-009.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-009.png)

plot2d : fungsi ini digunakan untuk printah membuat plot dua dimensi


"f(x)" : memanggil fungsi f(x)


-2,2   : grafik akan ditampilkan pada sb x dari rentang -2 sampai 2


Berikutnya kita definisikan fungsi:


$$g(x)=\frac{\sqrt{x^2-3x}}{x+1}$$\>function g(x) := sqrt(x^2-3\*x)/(x+1)

\>g(5)


    0.527046276695

\>g(20)


    0.878051853076

\>g(21)


    0.883737367965

\>g(20:25)


    [0.878052,  0.883737,  0.888915,  0.89365,  0.897998,  0.902003]

Silakan Anda plot grafik fungsi di atas!


\>aspect(1.5); plot2d("g(x)",20,25):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-011.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-011.png)

\>f(g(5)) // komposisi fungsi


    2.81254111152

f(g(5)) adalah notasi yang menunjukkan komposisi fungsi.


Ini berarti kita akan melakukan dua langkah perhitungan:


Hitung g(5): Pertama, kita mencari nilai dari fungsi g ketika x = 5.


Hasilnya akan kita sebut sebagai a.


Hitung f(a): Selanjutnya, kita masukkan nilai a yang kita dapatkan
dari langkah 1 ke dalam fungsi f.


Hasil akhir dari perhitungan ini adalah nilai dari f(g(5)).


\>g(f(5))


    0.993366510057

\>function h(x) := f(g(x)) // definisi komposisi fungsi 

\>h(5) // sama dengan f(g(5))


    2.81254111152

Silakan Anda plot kurva fungsi komposisi fungsi f dan g:


$$h(x)=f(g(x))$$dan


$$u(x)=g(f(x))$$bersama-sama kurva fungsi f dan g dalam satu bidang koordinat.


\>f(0:10) // nilai-nilai f(0), f(1), f(2), ..., f(10)


    [2.71828,  4.71653,  24.6596,  81.3716,  192.52,  376.328,  650.612,
    1031.13,  1536.86,  2187.4,  3000.43]

\>fmap(0:10) // sama dengan f(0:10), berlaku untuk semua fungsi


    [2.71828,  4.71653,  24.6596,  81.3716,  192.52,  376.328,  650.612,
    1031.13,  1536.86,  2187.4,  3000.43]

\>gmap(20:25)


Misalkan kita akan mendefinisikan fungsi


$$f(x) = \begin{cases} x^3 & x>0 \\ x^2 & x\le 0. \end{cases}$$Fungsi tersebut tidak dapat didefinisikan sebagai fungsi numerik
secara "inline" menggunakan format :=, melainkan didefinisikan sebagai
program. Perhatikan, kata "map" digunakan agar fungsi dapat menerima
vektor sebagai input, dan hasilnya berupa vektor. Jika tanpa kata
"map" fungsinya hanya dapat menerima input satu nilai.


\>function map f(x)


      if x>0 then return x^3
      else return x^2
      endif;
    endfunction
</pre>
\>f(4)


    64

\>f(-2)


    4

\>f(-5:5)


    [25,  16,  9,  4,  1,  0,  1,  8,  27,  64,  125]

\>aspect(1.5); plot2d("f(x)",-5,5):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-015.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-015.png)

$$f(x)=2e^x$$\>function f(x) &= 2\*E^x; // fungsi simbolik

\>$f(a) // nilai fungsi secara simbolik


$$2\,e^{a}$$\>function a:=12

\>f(a)


    325509.582838

\>f(E) // nilai fungsi berupa bilangan desimal


    30.308524483

$$g(x)=3x+1$$\>function g(x) &= 3\*x+1


    
                                   3 x + 1
    

\>g(50)


    151

\>function h(x) &= f(g(x)) // komposisi fungsi


    
                                     3 x + 1
                                  2 E
    

\>plot2d("h(x)",-1,1):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-019.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-019.png)

## Contoh Fungsi Aljabar

1.Diberikan fungsi:


$$f(x) = 6x^3+12\sqrt x$$Tentukan nilai f(1) dan f(4) kemudian cari nilai f(4)-2f(1)


Gambarkan juga grafiknya di f(1:4)!


\>function f(x) := 6\*x^3+12\*sqrt(x)

\>f(1)


    18

\>f(4)


    408

\>f(4)-2\*f(1)


    372

\>aspect(1.5); plot2d("f",1,4):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-021.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-021.png)

2. Diberikan fungsi:


$$k(x,y)= 12x^3+4y^2-3x+2$$Tentukan nilai k(1,1)+k(2,3)!


\>function k(x,y):= 12\*x^3+4\*y^2-3\*x+2

\>k(1,1)


    15

\>k(2,3)


    128

\>k(1,1)+k(2,3)


    143

3. Diketahui suatu fungsi f(x,y,z) diddefinisikan sebagai betrikut


$$f(x,y,z)=(3x-1)+\sqrt{x^3-y^2-z+6}$$Tentukan nilai f(3,4,5)!


\>function f(x,y,z):= (3\*x-1)+ sqrt(x^3-y^2-z+6)

\>f(3,4,5)


    11.4641016151

## Contoh Fungsi Trigonometri

1. Suatu fungsi trigonometri didefinisikan sebagai:


$$f(x)=\frac{tan(x)}{2x+3x^2}$$Tentukan nilai dari f(6)-f(7)!


\>function f(x):= tan(x)/2\*x+3\*x^2

\>f(6)-f(7)


    -42.9230865137

2. Diberikan fungsi:


$$f(x,y)=\frac{x^2+sin(y)}{xy}$$

Tentukan nilai f(4)!


\>function f(x,y) := x^2+sin(x)/x\*y

\>f(4,2)


    15.6215987523

\>plot3d("f",-4,4):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-026.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-026.png)

3. Diberikan suatu fungsi


$$f(x,y,z)=\frac{sin(x)}{cos(z)+sin(x)}+tan(y)$$tentukan nilai f(x,y,z) bila x=1, y=2, dan z=-3!


\>function f(x,y,z)&= sin(x)/(sin(x)+cos(z))+tan(y)


    
                               sin(x)
                           --------------- + tan(y)
                           cos(z) + sin(x)
    

\>f(1,2,-3)


    -7.85069041214

## Contoh Fungsi Eksponensial

1. Diberikan sebuah fungsi f(x) sebagai berikut:


$$f(x)=3^x$$Tentukan nilai f(x+1)-f(x)!


\>function f(x)&= 3^x;

\>$f(x+1)


$$3^{x+1}$$\>$f(x)


$$3^{x}$$\>$f(x+1)-f(x)


$$2\,3^{x}$$2. Fungsi f(m) didefinisikan sebagai:


$$f(m)=27+8^m$$Tentukan nilai dari f(3), 2f(5), dan f(3)/2f(5)


\>function f(m)&=27+8^m;

\>$f(3)


$$539$$\>$2\*f(5)


$$65590$$\>$f(3)/(2\*f(5))


$$\frac{77}{9370}$$3. Diketahui nilai y dari fungsi di bawah ini adalah 1


$$f(x)=2^{4x-12y}$$Tentukan nilai f(3), f(8), dan buat grafiknya di f(3:5)!


\>function f(x):=2^(4\*x-12\*y)

\>function y:=1

\>f(8)


    1048576

\>f(3)


    1

\>f(3:5)


    [1,  16,  256]

\>aspect(1.3); plot2d("f",3,5):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-037.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-037.png)

## Contoh Fungsi Logaritma

1. Diberikan fungsi di bawah ini:


$$f(x)=e^2 \cdot \left( \frac{1}{3+4 \log(x)}+\frac{1}{7} \right)$$Tentukan nilai f(0.6)!


\>function f(x):= E^2\*(1/(3+4\*log(x))+1/7)

\>f(0.6)


    8.77908249441

\>plot2d("f",-0.6,0.6):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-039.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-039.png)

## Contoh Komposisi Fungsi

1. Untuk fungsi:


$$f(x) = x^2-3x+2$$$$g(x)=3x+5$$cari nilai


$$fog(-2), gof(0)$$\>function f(x) :=  x^2-3\*x+2; $f(x)

\>function g(x) := 3\*x+5; $g(x)

\>f(g(-2)), g(f(0))


    6
    11

\>plot2d("(3\*x+5)^2-3\*(3\*x+5)+2",-2,2):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-043.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-043.png)

# Latihan

1. Diberikan fungsi:


$$b(x)= \frac{12x^3}{7x^2-3x}$$Cari nilai b(1), b(1:4), dan buatkan grafiknya!


\>function b(x):= (12\*x^3)/(7\*x^2-3\*x)

\>b(1)


    3

\>b(1:4)


    [3,  4.36364,  6,  7.68]

\>aspect(1.2); plot2d("b",5,25):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-045.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-045.png)

2. Diketahui suatu fungsi f(x) sebagai berikut:


$$f(x,y)=\frac{3(x-1)(y-2)}{2}+\frac{(y-2)(x-3)}{2}-2(x-1)(y-3)$$Tentukan nilai dari f(20,10) dan buat grafiknya di f(20,10:30,20)!


\>function f(x,y) &= 3\*(x-1)\*(y-2)/2+(y-2)\*(x-3)/2-2\*(x-1)\*(y-3)


    
            3 (x - 1) (y - 2)   (x - 3) (y - 2)
            ----------------- + --------------- - 2 (x - 1) (y - 3)
                    2                  2
    

\>f(20,10)


    30

\>plot3d("f(x,y)",20,10,30,20):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-047.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-047.png)

3. Sketsakan grafik fungsi dibawah ini pada[-pi,2pi]


$$y(t)=sin(5t)$$\>function y(t)&= sin(5\*t)


    
                                   sin(5 t)
    

\>y(-pi:pi)


    [0,  0.958924,  0.544021,  -0.650288,  -0.912945,  0.132352,  0.988032]

\>plot2d("y",-pi,pi):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-049.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-049.png)

4. Diketahui suatu fungsi f(x):


$$f(x)=3^x$$Tentukan nilai f(abc) jika nilai a=1, b=2, dan c=5!


\>function f(x):=3^x

\>function a:=1

\>function b:=6

\>function c:=5

\>f(a\*b\*c)


    2.05891132095e+14

5. Untuk fungsi:


$$f(x) = 2x^2-3x+20$$$$g(x)= 3x-5$$cari nilai


$$fog(5), gof(8)$$\>function g(x) := 3\*x-5

\>function f(x) := 2\*x^2-3\*x+20

\>f(g(5))


    190

\>g(f(8))


    367

# 2. Limit

## Definisi limit

Pada dasarnya, limit digunakan untuk menyatakan sesuatu yang nilainya
mendekati nilai tertentu. Limit dapat diartikan sebagai menuju suatu
batas, sesuatu yang dekat namun tidak dapat dicapai. Mengapa nilainya
hanya mendekati? Karena suatu fungsi biasanya tidak terdefinisi pada
titik-titik tertentu. Walaupun suatu fungsi seringkali tidak
terdefinisi untuk titik tertentu, namun masih dapat dicari tahu berapa
nilai yang didekati oleh fungsi tersebut apabila titik tertentu
semakin didekati yaitu dengan limit.


Bentuk umum dari limit sendiri dinotasikan dengan:


$$\lim_{x\rightarrow c}{F\left(x\right)}=L$$Notasi tersebut menyatakan bahwa f(x) untuk niai x mendekati c sama
dengan L. F(x) disini dapat berupa bermacam-macam jenis fungsi. Dan L
dapat berupa konstanta, ataupun "und" (tak terdefinisi), "ind" (tak
tentu namun terbatas), "infinity" (kompleks tak hingga). Begitupun
dengan batas c, dapat berupa sebarang nilai atau pada tak hingga
(-inf, minf, dan inf).


Sebuah fungsi dapat dikatakan memiliki limit apabila limit kanan dan
limit kiri nya memiliki nilai yang sama. Dimana, limit dari fungsi
tersebut adalah nilai dari limit kanan dan limit kiri fungsi yang
bernilai sama tadi.


## Sifat-sifat Limit

Jika f(x) dan g(x) adalah fungsi yang memiliki limit di c, n merupakan
bilangan bulat positif, dan k adalah konstanta.


1.


$$\lim_{x \to c}k=k$$\>$showev('limit(5,x,2))


$$5=5$$$$\lim_{x \to 2}5=5$$2.


maxima: 'limit(x,x,c)=c


$$\lim_{x\rightarrow c}{x}=c$$\>$showev('limit(x,x,3))


$$\lim_{x\rightarrow 3}{x}=3$$3.


maxima: 'limit(kf(x),x,c)= k*maxima: 'limit(f(x),x,c)


$$\lim_{x\rightarrow c}{{\it kf}\left(x\right)}=k\,\left(\lim_{x  \rightarrow c}{f\left(x\right)}\right)$$\>$showev('limit(4\*x^2,x,1))


$$4\,\left(\lim_{x\rightarrow 1}{x^2}\right)=4$$4.


maxima: 'limit([g(x)+f(x)],x,c)= maxima: 'limit(g(x),x,c) + maxima: 'limit(f(x),x,c)


$$\lim_{x\rightarrow c}{\left[ g\left(x\right)+f\left(x\right)   \right] }=\lim_{x\rightarrow c}{g\left(x\right)}+\lim_{x  \rightarrow c}{f\left(x\right)}$$\>$showev('limit(x^3+2\*x,x,1))


$$\lim_{x\rightarrow 1}{x^3+2\,x}=3$$5.


maxima: 'limit([g(x)-f(x)],x,c)= maxima: 'limit(g(x),x,c) - maxima: 'limit(f(x),x,c)


$$\lim_{x\rightarrow c}{\left[ g\left(x\right)-f\left(x\right)   \right] }=\lim_{x\rightarrow c}{g\left(x\right)}-\lim_{x  \rightarrow c}{f\left(x\right)}$$\>$showev('limit(x^2-4\*x,x,5))


$$\lim_{x\rightarrow 5}{x^2-4\,x}=5$$6.


maxima: 'limit([g(x)*f(x)],x,c)= maxima: 'limit(g(x),x,c) * maxima: 'limit(f(x),x,c)


$$\lim_{x\rightarrow c}{\left[ f\left(x\right)\,g\left(x\right)   \right] }=\left(\lim_{x\rightarrow c}{f\left(x\right)}\right)\,  \left(\lim_{x\rightarrow c}{g\left(x\right)}\right)$$\>$showev('limit((x-1)\*(x+4),x,3))


$$\lim_{x\rightarrow 3}{\left(x-1\right)\,\left(x+4\right)}=14$$7.


maxima: 'limit(g(x)/f(x),x,c)= maxima: 'limit(g(x),x,c) / maxima: 'limit(f(x),x,c)


$$\lim_{x\rightarrow c}{\frac{g\left(x\right)}{f\left(x\right)}}=  \frac{\lim_{x\rightarrow c}{g\left(x\right)}}{\lim_{x\rightarrow c}{  f\left(x\right)}}$$\>$showev('limit((x+5)/(x+1),x,0))


$$\lim_{x\rightarrow 0}{\frac{x+5}{x+1}}=5$$8.


maxima: 'limit(f(x)^n,x,c)=maxima:'limit(f(x),x,c)^n


$$\lim_{x\rightarrow c}{f^{n}\left(x\right)}=\left(\lim_{x  \rightarrow c}{f\left(x\right)}\right)^{n}$$\>$showev('limit((x+3)^2,x,1))


$$\lim_{x\rightarrow 1}{\left(x+3\right)^2}=16$$9.


$$\lim_{x\rightarrow c}{f\left(x\right)^{\frac{1}{n}}}=\left(\lim_{x  \rightarrow c}{f\left(x\right)}\right)^{\frac{1}{n}}$$\>$showev('limit((x^2+3\*x+1)^(1/2),x,2))


$$\lim_{x\rightarrow 2}{\sqrt{x^2+3\,x+1}}=\sqrt{11}$$# Limit pada EMT

Pada EMT cara mendefinisikan limit yaitu dengan format :


$showev('limit(f(x),x,c))


Format tersebut akan menampilkan limit yang dimaksud dan hasilnya.
Jika kita ingin menampilkan hasilnya saja dari sebuah limit tanpa
menampilkan limitnya, kita bisa menggunakan format :


$limit(f(x),x,c)


Sedangkan, untuk limit kanan dan limit kiri seperti pada definisi
dapat ditampilkan di EMT dengan cara menambah opsi "plus" atau "minus"
:


$showev('limit(f(x),x,c, plus)) atau 'limit(f(x),x,c, minus)


\>$showev('limit(x^2+3\*x+4,x,2))


$$\lim_{x\rightarrow 2}{x^2+3\,x+4}=14$$\>$limit(x^2+3\*x+4,x,2)


$$14$$# Menghitung dan Visualisasi Limit

Perhitungan limit pada EMT dapat dilakukan dengan menggunakan fungsi
Maxima, yakni "limit". Fungsi "limit" dapat digunakan untuk menghitung
limit fungsi dalam bentuk ekspresi maupun fungsi yang sudah
didefinisikan sebelumnya. Nilai limit dapat dihitung pada sebarang
nilai atau pada tak hingga (-inf, minf, dan inf). Limit kiri dan limit
kanan juga dapat dihitung, dengan cara memberi opsi "plus" atau
"minus". Hasil limit dapat berupa nilai, "und" (tak definisi), "ind"
(tak tentu namun terbatas), "infinity" (kompleks tak hingga).


Limit dapat divisualisasikan menggunakan plot 2 dimensi. Pada EMT
sendiri, format yang bisa digunakan untuk memvisualisasikan limit
adalah :


plot2d("f(x)",-c,c):


Dengan f(x) adalah fungsi pada limit yang dicari, dan c berupa
bilangan real menyesuaikan batas dari limit itu sendiri.


## Limit Aljabar



1. Tunjukkan bahwa limit kiri dan kanan dari fungsi berikut bernilai
sama. Berapakah nilai limitnya?


$$\lim_{x\rightarrow 0}{x^2+x-1}$$\>$showev('limit(x^2+x-1,x,0,minus))


$$\lim_{x\uparrow 0}{x^2+x-1}=-1$$\>$showev('limit(x^2+x-1,x,0,plus))


$$\lim_{x\downarrow 0}{x^2+x-1}=-1$$Dapat terlihat bahwa nilai limit kiri = nilai limit kanan. Maka fungsi
tersebut memiliki nilai limit, yaitu :


\>$showev('limit(x^2+x-1,x,0))


$$\lim_{x\rightarrow 0}{x^2+x-1}=-1$$2. Tunjukkan bahwa limit kiri dan kanan dari fungsi berikut bernilai
sama. Berapakah nilai limitnya?


$$\lim_{x\rightarrow 3}{\sqrt{x^2+x-1}}$$\>$showev('limit(sqrt(x^2+x-1),x,3,minus))


$$\lim_{x\uparrow 3}{\sqrt{x^2+x-1}}=\sqrt{11}$$\>$showev('limit(sqrt(x^2+x-1),x,3,plus))


$$\lim_{x\downarrow 3}{\sqrt{x^2+x-1}}=\sqrt{11}$$Dapat terlihat bahwa nilai limit kiri = nilai limit kanan. Maka fungsi
tersebut memiliki nilai limit, yaitu :


\>$showev('limit(sqrt(x^2+x-1),x,3))


$$\lim_{x\rightarrow 3}{\sqrt{x^2+x-1}}=\sqrt{11}$$3. Tunjukkan bahwa limit kiri dan kanan dari fungsi berikut bernilai
sama. Berapakah nilai limitnya?


$$\lim_{x\rightarrow -3}{\frac{\left| x+3\right| }{x+3}}$$\>$showev('limit(abs(x+3)/(x+3),x,-3,minus))


$$\lim_{x\uparrow -3}{\frac{\left| x+3\right| }{x+3}}=-1$$\>$showev('limit(abs(x+3)/(x+3),x,-3,plus))


$$\lim_{x\downarrow -3}{\frac{\left| x+3\right| }{x+3}}=1$$Karena nilai limit kiri tidak sama dengan nilai limit kanan. Maka
fungsi diatas tidak memiliki limit di x=-3


\>$showev('limit(abs(x+3)/(x+3),x,-3))


$$\lim_{x\rightarrow -3}{\frac{\left| x+3\right| }{x+3}}={\it und}$$\>$limit(x^3+4\*x+5,x,2)


$$21$$\>plot2d("x^3+4\*x+5",1.8,2.2); plot2d(2,21,\>points,style="ow",\>add):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-089.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-089.png)

Jadi berdasarkan grafik, nilai limit tersebut adalah 21.


5. Berapakah nilai limit dari fungsi berikut? Tunjukkan dengan
menggunakan grafik!


maxima: 'limit((abs(x-5))/(x-5),x,5)


$$\lim_{x\rightarrow 5}{\frac{\left| x-5\right| }{x-5}}$$\>plot2d("abs(x-5)/(x-5)",4.9,5.1):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-091.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-091.png)

Karena nilai limit kiri tidak sama dengan limit kanan. maka nili limit
fungsi tersebut tidak ada.


6. Berapakah nilai limit dari fungsi berikut?


$$\lim_{x\rightarrow \infty }{\frac{x^5-3\,x^3+x^2-9}{4\,x^5-7\,x^4+2  \,x-1}}$$\>$showev('limit((x^5-3\*x^3+x^2-9)/(4\*x^5-7\*x^4+2\*x-1),x,inf))


$$\lim_{x\rightarrow \infty }{\frac{x^5-3\,x^3+x^2-9}{4\,x^5-7\,x^4+2  \,x-1}}=\frac{1}{4}$$7. Tunjukkan nilai limit fungsi berikut dengan grafik!


maxima:  'limit(sqrt(x^2+x)-x,x,inf)


$$\lim_{x\rightarrow \infty }{\sqrt{x^2+x}-x}$$\>plot2d("sqrt(x^2+x)-x",0,10):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-095.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-095.png)

Dengan menggunakan grafik diperlihatkan bahwa nilai limit mendekati
0.5. Mari kita buktikan di baris perintah


\>$showev('limit(sqrt(x^2+x)-x,x,inf))


$$\lim_{x\rightarrow \infty }{\sqrt{x^2+x}-x}=\frac{1}{2}$$## Limit Trigonometri

1. Tunjukkan bahwa limit kiri dan kanan dari fungsi berikut bernilai
sama. Berapakah nilai limitnya?


$$\lim_{x\rightarrow 0}{\cos x\,\sin x}$$\>$showev('limit(cos(x)\*sin(x),x,0,minus))


$$\lim_{x\uparrow 0}{\cos x\,\sin x}=0$$\>$showev('limit(cos(x)\*sin(x),x,0,plus))


$$\lim_{x\downarrow 0}{\cos x\,\sin x}=0$$Dapat terlihat bahwa nilai limit kiri = nilai limit kanan. Maka fungsi
tersebut memiliki nilai limit, yaitu :


\>$showev('limit(cos(x)\*sin(x),x,0))


$$\lim_{x\rightarrow 0}{\cos x\,\sin x}=0$$2. Berapakah nilai limit dari fungsi berikut? Tunjukkan dengan
menggunakan grafik


$$\lim_{x\rightarrow 0}{\frac{1-\cos x}{x}}$$\>plot2d("(1-cos(x))/x",-pi/4,pi/4); plot2d(0,0,\>points,style="ow",\>add):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-102.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-102.png)

3. Tunjukkan bahwa limit kiri dan kanan dari fungsi berikut bernilai
sama. Berapakah nilai limitnya?


$$\lim_{x\rightarrow 0}{\frac{\sin x}{1-\cos x}}$$\>$showev('limit(3\*sin(x)^2/(1-cos(x)),x,0,minus))


$$3\,\left(\lim_{x\uparrow 0}{\frac{\sin ^2x}{1-\cos x}}\right)=6$$\>$showev('limit(3\*sin(x)^2/(1-cos(x)),x,0,plus))


$$3\,\left(\lim_{x\downarrow 0}{\frac{\sin ^2x}{1-\cos x}}\right)=6$$Dapat terlihat bahwa nilai limit kiri = nilai limit kanan. Maka fungsi
tersebut memiliki nilai limit, yaitu


\>$showev('limit(3\*sin(x)^2/(1-cos(x)),x,0))


$$3\,\left(\lim_{x\rightarrow 0}{\frac{\sin ^2x}{1-\cos x}}\right)=6$$4. Berapakah nilai limit dari fungsi berikut? Tunjukkan dengan
menggunakan grafik!


$$\lim_{x\rightarrow 0}{\left| \sin \left(2\,x\right)\right| -\cos x}$$\>$limit(abs(sin(2\*x))-cos(x),x,0)


$$-1$$\>plot2d("abs(sin(2x))-cos(x)",-pi/2,pi/2); plot2d(0,-1,\>points,style="ow",\>add):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-109.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-109.png)

Jadi berdasarkan grafik, nilai limit tersebut adalah -1.


5. Berapakah nilai limit dari fungsi berikut? Tunjukkan dengan
menggunakan grafik!


maxima: 'limit(2*sin(x)*cos(x)-tan(x),x,pi/3)


$$\lim_{x\rightarrow \frac{\pi}{3}}{2\,\cos x\,\sin x-\tan x}$$\>$limit(2\*cos(x)\*sin(x)-tan(x),x,pi/3)


$$-\frac{\sqrt{3}}{2}$$\>plot2d("2\*cos(x)\*sin(x)-tan(x)",0,pi/2.9); plot2d(pi/3,-(3)^(1/2)/2,\>points,style="ow",\>add):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-112.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-112.png)

Jadi berdasarkan grafik, nilai limit tersebut adalah -0.866.


6. Berapakah nilai limit dari fungsi berikut? Tunjukkan dengan
menggunakan grafik!


$$2\,\left(\lim_{x\rightarrow 0}{\sec x}\right)$$\>$limit(2\*sec(x),x,0)


$$2$$\>plot2d("2\*sec(x)",-pi/3,pi/3); plot2d(0,2,\>points,style="ow",\>add):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-115.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-115.png)

Jadi berdasarkan grafik, nilai limit tersebut adalah 2.


## Latihan

1. Tunjukkan bahwa limit kiri dan kanan dari fungsi berikut bernilai
sama!


$$\lim_{x\rightarrow 3}{\frac{\left(x-3\right)\,\left| x^3+5\,x+8  \right| }{\cos x}}$$\>$limit(abs(x^3+5\*x+8)/cos(x)\*(x-3),x,3)


$$0$$2. Tunjukkan nilai limit fungsi berikut dengan menggunakan grafik!


$$\lim_{x\rightarrow 0.8}{\frac{\left(x^2+6\,x+1\right)\,\sin \left(3  \,x\right)}{\cos x}}$$\>$limit((x^2+6\*x+1)\*sin(3\*x)/cos(x),x,0.8)


$$6.243635699770241$$3. Tentukan nilai limit dari fungsi berikut


maxima: 'limit((x^2-x-6)/(4-sqrt(5*x+1)),x,3)


$$\lim_{x\rightarrow 3}{\frac{x^2-x-6}{4-\sqrt{5\,x+1}}}$$\>$limit((x^2-x-6)/(4-sqrt(5\*x+1)),x,3)


$$-8$$4. Apakah benar nilai dari limit berikut?


maxima: 'limit(4*x/sin(9*x),x,0)=9/4


$$4\,\left(\lim_{x\rightarrow 0}{\frac{x}{\sin \left(9\,x\right)}}  \right)=\frac{9}{4}$$\>$limit(4\*x/sin(9\*x),x,0)


$$\frac{4}{9}$$5. Berapa nilai limit berikut?


maxima: 'limit(sqrt(3*x-5)-sqrt(x-1),x,inf)


$$\lim_{x\rightarrow \infty }{\sqrt{3\,x-5}-\sqrt{x-1}}$$\>$limit(sqrt(3\*x-5)-sqrt(x-1),x,inf)


$$\infty $$# 3. Turunan Fungsi

  Turunan adalah pengukuran terhadap bagaimana fungsi berubah seiring  

perubahan nilai yang dimasukkan, atau secara umum turunan menunjukkan
bagaimana suatu besaran berubah akibat perubahan besaran lainnya.
Proses dalam menemukan turunan disebut diferensiasi.


Definisi turunan:


$$f'(x) = \lim_{h\to 0}\frac{f(x+h)-f(x)}{h}$$

Berikut adalah contoh-contoh menentukan turunan fungsi dengan beberapa
cara.


## Turunan fungsi Aljabar

Mencari turunan dari


$$f(x)=x^n$$\>$showev('limit(((x+h)^n-x^n)/h,h,0)) // turunan x^n


$$\lim_{h\rightarrow 0}{\frac{\left(x+h\right)^{n}-x^{n}}{h}}=n\,x^{n  -1}$$Bukti:


$$(x+h)^n= \binom{n}{0}x^{n-0}h^0+ \binom{n}{1}x^{n-1}h^1+\binom{n}{2}x^{n-2}h^2+...+\binom{n}{n}x^{n-n}h^n$$$$(x+h)^n = x^n+nx^{n-1}h+\binom{n}{2}x^{n-2}h^2+...+h^n$$$$(x+h)^n -x^n = nx^{n-1}h+\binom{n}{2}x^{n-2}h^2+...+h^n$$$$\frac{(x+h)^n -x^n}{h} = nx^{n-1}+\binom{n}{2}x^{n-2}h+...+h^{n-1}$$$$\lim_{h\to 0}\frac{(x+h)^n -x^n}{h}=nx^{n-1}$$Mencari turunan dari


$$f(x)=x^2$$\>$showev('limit(((x+h)^2-x^2)/h,h,0)) // turunan x^2


$$\lim_{h\rightarrow 0}{\frac{\left(x+h\right)^2-x^2}{h}}=2\,x$$\>p &= expand((x+h)^2-x^2)|simplify; $p //pembilang dijabarkan dan disederhanakan


$$2\,h\,x+h^2$$\>q &=ratsimp(p/h); $q // ekspresi yang akan dihitung limitnya disederhanaka


$$2\,x+h$$\>$limit(q,h,0) // nilai limit sebagai turunan


$$2\,x$$\>plot2d(["x^2", "2x"], color=[black,red]):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-139.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-139.png)

Mencari turunan dari


$$f(x)=f(x)^x$$\>$showev('limit((f(x+h)-f(x))/h,h,0)) // turunan f(x)=f(x)^x


$$\lim_{h\rightarrow 0}{\frac{\left(\lim_{h\rightarrow 0}{\frac{f  \left(x+h\right)-f\left(x\right)}{h}}\right)(x+h)-\left(\lim_{h  \rightarrow 0}{\frac{f\left(x+h\right)-f\left(x\right)}{h}}\right)(x  )}{h}}=\lim_{h\rightarrow 0}{\frac{\left(\lim_{h\rightarrow 0}{  \frac{f\left(x+h\right)-f\left(x\right)}{h}}\right)(x+h)-\left(  \lim_{h\rightarrow 0}{\frac{f\left(x+h\right)-f\left(x\right)}{h}}  \right)(x)}{h}}$$Di sini Maxima bermasalah terkait limit:


$$\lim_{h\to 0} \frac{(x+h)^{x+h}-x^x}{h}.$$Dalam hal ini diperlukan asumsi nilai x.


\>&assume(x\>0); $showev('limit((f(x+h)-f(x))/h,h,0)) // turunan f(x)=f(x)^x


$$\lim_{h\rightarrow 0}{\frac{\left(\lim_{h\rightarrow 0}{\frac{f  \left(x+h\right)-f\left(x\right)}{h}}\right)(x+h)-\left(\lim_{h  \rightarrow 0}{\frac{f\left(x+h\right)-f\left(x\right)}{h}}\right)(x  )}{h}}=\lim_{h\rightarrow 0}{\frac{\left(\lim_{h\rightarrow 0}{  \frac{f\left(x+h\right)-f\left(x\right)}{h}}\right)(x+h)-\left(  \lim_{h\rightarrow 0}{\frac{f\left(x+h\right)-f\left(x\right)}{h}}  \right)(x)}{h}}$$\>&forget(x\>0) // jangan lupa, lupakan asumsi untuk kembali ke semula


    
                                   [x &gt; 0]
    

\>&forget(x<0)


    
                                   [x &lt; 0]
    

\>&facts()


    
                                      []
    

Selain dengan showev('limit...) kita juga dapat mencari turunan dengan
menyederhanakan pembilang seperti di awal


\>p &= expand(f(x+h)-f(x))|simplify;  $p


$$f\left(x+h\right)-f\left(x\right)$$\>q &=ratsimp(p/h); $q


$$\frac{f\left(x+h\right)-f\left(x\right)}{h}$$\>$limit(q,h,0)


$$\lim_{h\rightarrow 0}{\frac{f\left(x+h\right)-f\left(x\right)}{h}}$$Mencari turunan dari


$$f(x)=\frac{1}{x}$$\>$showev('limit((1/(x+h)-1/x)/h,h,0)) // turunan 1/x


$$\lim_{h\rightarrow 0}{\frac{\frac{1}{x+h}-\frac{1}{x}}{h}}=-\frac{1  }{x^2}$$\>plot2d("-x^(-2)", color=red):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-149.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-149.png)

## Turunan fungsi trigonometri

Mencari turunan dari


\>$showev('limit((sin(x+h)-sin(x))/h,h,0)) // turunan sin(x)


$$\lim_{h\rightarrow 0}{\frac{\sin \left(x+h\right)-\sin x}{h}}=\cos   x$$Bukti:


$$sin(x+h) = sin(x)cos(h)+cos(x)sin(h)$$$$sin(x+h)-sin(x) = sin(x)cos(h)+cos(x)sin(h)-sin(x)$$$$sin(x+h)-sin(x) = cos(x)sin(h) - sin(x)+sin(x)cos(h)$$$$sin(x+h)-sin(x) = cos(x)sin(h) - sin(x)(1-cos(h))$$$$\lim_{h\to 0}\frac{sin(x+h)-sin(x)}{h}= \lim_{h\to 0}\frac{cos(x)sin(h)}{h}-\lim_{h\to 0}\frac{sin(x)(1-cos(h)}{h}$$$$\lim_{h\to 0}\frac{sin(x+h)-sin(x)}{h}=cos(x)\lim_{h\to 0}\frac{sin(h)}{h}-sin(x)\lim_{h\to 0}\frac{(1-cos(h)}{h}$$$$=cos(x)\times 1 -sin(x) \times 0 =cos(x)$$\>p &= expand((sin(x+h)-sin(x)))|simplify; $p


$$\sin \left(x+h\right)-\sin x$$\>q &=ratsimp(p/h); $q 


$$\frac{\sin \left(x+h\right)-\sin x}{h}$$\>$limit(q,h,0) // nilai limit sebagai turunan


$$\cos x$$\>plot2d(["sin(x)", "cos(x)"],0, 2\*pi, color=[blue,green]):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-161.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-161.png)

 Mencari turunan dari  
 latex: tan(x)  

\>$showev('limit((tan(x+h)-tan(x))/h,h,0)) // turunan tan(x)


$$\lim_{h\rightarrow 0}{\frac{\tan \left(x+h\right)-\tan x}{h}}=  \frac{1}{\cos ^2x}$$Bukti:


$$tan(x+h) = \frac {tan (x)+tan (h)}{1-tan(x)tan(h)}$$$$tan(x+h)-tan (x) ={\frac {tan (x)+tan (h)-tan (x)+tan^2(x)tan(h)}{1-tan(x)tan(h)}}$$$$\frac{tan(x+h)-tan (x)}{h} =\frac{\frac{tan(x)+tan(h)-tan(x)+tan^2(x)tan(h)}{1-tan(x)tan(h)}}{h}$$$$= \frac {tan(h)+tan^2(x)tan(h)}{h(1-tan(x)tan(h)}$$$$= \lim_{h\to 0} \frac{tan(h)+tan^2(x) tan(h)}{h(1-tan(x)tan(h)}$$$$= \lim_{h\to 0} \frac{1 +tan^2(x)}{1-tan (x)tan(h)}\cdot\lim_{h\to 0} \frac{tan (h)}{h}$$$$= \frac{1 +tan^2(x)}{1-tan (x)tan(0)}\cdot 1$$$$= 1+tan^2(x)$$$$1+tan^2(x)=1+\frac{sin^2(x)}{cos^2(x)}$$$$= \frac{cos^2(x) + sin^2(x)}{cos^2(x)}$$$$= \frac{1}{cos^2(x)}$$\>p &= expand((tan(x+h)-tan(x)))|simplify; $p


$$\tan \left(x+h\right)-\tan x$$\>q &=ratsimp(p/h); $q 


$$\frac{\tan \left(x+h\right)-\tan x}{h}$$\>$limit(q,h,0) // nilai limit sebagai turunan


$$\frac{1}{\cos ^2x}$$Mencari turunan dari


$$arcsin(x)$$\>$showev('limit((asin(x+h)-asin(x))/h,h,0)) // turunan arcsin(x)


$$\lim_{h\rightarrow 0}{\frac{\arcsin \left(x+h\right)-\arcsin x}{h}}=  \frac{1}{\sqrt{1-x^2}}$$Bukti:


$$f'(x)= \lim_{h\to 0} \frac {arcsin(x+h)-arcsin(x)}{h}$$Misalkan arcsin(x+h)=A dan arcsin(x)=B


Sehingga sin A= x+h dan sin B=x


Kurangkan persamaan kedua dengan persamaan pertama


$$sin(A)-sin(B)=(x+h)-x$$$$sin(A)-sin(B) = h$$karena


$$h \to 0, sin(A)-sin(B) \to 0$$

maka


$$sin(A)\to sin(B),  A \to B, A-B \to 0$$sehingga f'(x) menjadi


$$f'(x) = \lim_{A-B \to 0} \frac{A-B}{sin A- sin B}$$Identitas trigonometri


$$sin(A)-sin(B) = 2 sin[\frac{A-B}{2}]cos[\frac{A+B}{2}]$$$$f'(x) = \lim_{A-B \to 0} \frac{A-B}{2 sin [\frac{A-B}{2}] cos [\frac{A+B}{2}]}$$$$f'(x) = \lim_{A-B \to 0} \frac{\frac{2(A-B)}{2}}{2 sin [\frac{A-B}{2}] cos [\frac{A+B}{2}]}$$ingat bahwa


$$\lim_{x \to 0}\frac{x}{sin (x)}=1$$$$f'(x) = \lim_{A-B \to 0}\frac{\frac{(A-B)}{2}}{sin[\frac{A-B}{2}]} \cdot \frac{2}{2cos[\frac{A+B}{2}]}$$$$f'(x) = 1 \cdot \frac{2}{2cos[\frac{B+B}{2}]}$$$$f'(x) = \frac{1}{cos (B)}$$$$f'(x) = \frac{1}{\sqrt{(cos^2 (B)}}$$$$f'(x) = \frac{1}{\sqrt{(1- sin^2 (B)}}= \frac{1}{\sqrt{(1-x^2}}$$\>p &= expand((asin(x+h)-asin(x)))|simplify; $p //pembilang dijabarkan dan disederhanakan


$$\arcsin \left(x+h\right)-\arcsin x$$\>q &=ratsimp(p/h); $q // ekspresi yang akan dihitung limitnya disederhanakan


$$\frac{\arcsin \left(x+h\right)-\arcsin x}{h}$$\>$limit(q,h,0) // nilai limit sebagai turunan


$$\frac{1}{\sqrt{1-x^2}}$$\>plot2d(["asin(x)","1/(sqrt(1-x^2))"],-1,1,color=[blue,red]):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-197.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-197.png)

Mencari turunan dari


$$x^2+10$$

di titik x=5


\>function f(x) &= x^2+10 // definisikan f(x)=x^2+10


    
                                    2
                                   x  + 10
    

\>function df(x) &= showev('diff(f(x),x)); $df(x)


$$\frac{d}{d\,x}\,\left(x^2+10\right)=2\,x$$\>$% with x=5


$${\it \%at}\left(\frac{d}{d\,x}\,\left(x^2+10\right) , x=5\right)=10$$\>diff(f,5), diffc(f,5)


    9.99999999997
    10

diff: Diferensiasi numerik yang pada dasarnya kurang akurat untuk
fungsi umum.


diffc: Menghitung turunan pertama untuk fungsi analitik nyata dengan
menggunakan bagian imajiner dari f(x+ih)/h. Cara ini memungkinkan
untuk mengevaluasi f dengan lebih akurat.


Mencari turunan dari


\>function f(x) &= sinh(x) // definisikan f(x)=sinh(x)


    
                                   sinh(x)
    

\>function df(x) &= limit((f(x+h)-f(x))/h,h,0); $df(x) // df(x) = f'(x)


$$\frac{e^ {- x }\,\left(e^{2\,x}+1\right)}{2}$$Hasilnya adalah cosh(x), karena


$$\frac{e^x+e^{-x}}{2}=\cosh(x).$$\>plot2d(["f(x)","df(x)"],-pi,pi,color=[blue,red]):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-203.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-203.png)

\>$showev('diff(f(x),x))


$$\frac{d}{d\,x}\,\sinh x=\cosh x$$\>$% with x=3


$${\it \%at}\left(\frac{d}{d\,x}\,\sinh x , x=3\right)=\cosh 3$$\>$float(%)


$${\it \%at}\left(\frac{d^{1.0}}{d\,x^{1.0}}\,\sinh x , x=3.0\right)=  10.06766199577777$$\>plot2d(f,0,3.1):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-207.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-207.png)

Mencari turunan dari


$$f(x)=sin(3x^5+7)^2$$\>function f(x) &= sin(3\*x^5+7)^2


    
                                   2    5
                                sin (3 x  + 7)
    

\>$showev('diff(f(x),x))


$$\frac{d}{d\,x}\,\sin ^2\left(3\,x^5+7\right)=30\,x^4\,\cos \left(3  \,x^5+7\right)\,\sin \left(3\,x^5+7\right)$$\>$% with x = 2


$${\it \%at}\left(\frac{d}{d\,x}\,\sin ^2\left(3\,x^5+7\right) , x=2  \right)=480\,\cos 103\,\sin 103$$\>$float(%)


$${\it \%at}\left(\frac{d^{1.0}}{d\,x^{1.0}}\,\sin ^2\left(3.0\,x^5+  7.0\right) , x=2.0\right)=-233.9140567500984$$\>diff(f,2), diffc(f,2)


    -233.913935807
    -233.91405675

diff: Diferensiasi numerik yang pada dasarnya kurang akurat untuk
fungsi umum.


diffc: Menghitung turunan pertama untuk fungsi analitik nyata dengan
menggunakan bagian imajiner dari f(x+ih)/h. Cara ini memungkinkan
untuk mengevaluasi f dengan lebih akurat.


\>plot2d(f,0,3.1) :


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-212.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-212.png)

Mencari turunan dari


$$a(x)=5cos(2x)-2xsin(2x)$$\>function a(x) &=5\*cos(2\*x)-2\*x\*sin(2\*x) // mendifinisikan fungsi a


    
                          5 cos(2 x) - 2 x sin(2 x)
    

\>function da(x) &=diff(a(x),x); $da(x) // da(x) = a'(x)


$$-12\,\sin \left(2\,x\right)-4\,x\,\cos \left(2\,x\right)$$\>$’a(1)=a(1), $float(a(1)), $’a(2)=a(2), $float(a(2)) // nilai a(1) dan a(2)


$$-0.2410081230863468$$![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-216.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-216.png)

\>xp=solve("da(x)",1,2,0) // solusi a'(x)=0 pada interval [1, 2]


    1.35822987384

\>da(xp), a(xp) // cek bahwa a'(xp)=0 dan nilai ekstrim di titik tersebut


    0
    -5.67530133759

\>plot2d(["a(x)","da(x)"],0,2\*pi,color=[blue,red]): //grafik fungsi dan turunannya


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-217.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-217.png)

Pada titik puncak grafik a(x), nilai turunan a'(x) akan selalu sama
dengan nol. Ini karena gradien garis singgung pada titik puncak adalah
nol.


## Turunan fungsi logaritma

Mencari turunan dari


$$f(x)= log(x)$$\>$showev('limit((log(x+h)- log(x))/h,h,0)) // turunan log(x)


$$\lim_{h\rightarrow 0}{\frac{\log \left(x+h\right)-\log x}{h}}=  \frac{1}{x}$$Bukti:


$$f'(x) = \lim_{h\to 0} \frac{log(x+h)-log x}{h}$$ingat bahwa


$$log(a)-log(b)= log (\frac{a}{b})$$$$f'(x)=\lim_{h\to 0}\frac{log(\frac{x+h}{x})}{h}$$$$f'(x)=\lim_{h\to 0}\frac{log(1 + \frac{h}{x})}{h}$$misalkan h/x = n sehingga h=nx


$$f'(x)=\lim_{n\to 0}\frac{ log (1 + n)}{nx}$$$$f'(x)=\lim_{n\to 0}\frac{1}{nx} \cdot log(1+n)$$ingat bahwa


$$a log b = log b^a$$$$f'(x)=\lim_{n\to 0} \frac{1}{x} \cdot log(1+n)^\frac{1}{n}$$$$f'(x)= \frac{1}{x}log \lim_{n\to 0}(1+n)^\frac{1}{n}$$$$\lim_{n\to 0}(1+n)^\frac{1}{n} = e$$$$f'(x)= \frac{1}{x}log e$$$$f'(x)=\frac{1}{x}$$\>$showev('limit((log((x+h)/(x)))/h,h,0))//definisi logaritma


$$\lim_{h\rightarrow 0}{\frac{\log \left(\frac{x+h}{x}\right)}{h}}=  \frac{1}{x}$$\>$showev('limit(((h/x))/h,h,0))//menggunakan identitas logaritma, sisanya adalah hasil turunan


$$\frac{1}{x}=\frac{1}{x}$$## Turunan fungsi eksponensial

Mencari turunan dari


$$f(x)=e^x$$\>$showev('limit((E^(x+h)-E^x)/h,h,0)) // turunan f(x)=e^x


    Answering "Is x an integer?" with "integer"
    Answering "Is x an integer?" with "integer"
    Answering "Is x an integer?" with "integer"
    Answering "Is x an integer?" with "integer"
    Answering "Is x an integer?" with "integer"
    Maxima is asking
    Acceptable answers are: yes, y, Y, no, n, N, unknown, uk
    Is x an integer?
    
    Use assume!
    Error in:
    $showev('limit((E^(x+h)-E^x)/h,h,0)) // turunan f(x)=e^x ...
                                         ^

Maxima bermasalah dengan limit:


$$\lim_{h\to 0}\frac{e^{x+h}-e^x}{h}.$$Oleh karena itu diperlukan trik khusus agar hasilnya benar.


\>$showev('factor(E^(x+h)-E^x))


$${\it factor}\left(e^{x+h}-e^{x}\right)=\left(e^{h}-1\right)\,e^{x}$$\>$showev('limit(factor((E^(x+h)-E^x)/h),h,0)) // turunan f(x)=e^x


$$\left(\lim_{h\rightarrow 0}{\frac{e^{h}-1}{h}}\right)\,e^{x}=e^{x}$$\>$showev('limit((E^h-1)/h,h,0))


$$\lim_{h\rightarrow 0}{\frac{e^{h}-1}{h}}=1$$## Sifat- sifat Turunan

1. Jika f(x)=k dengan k suatu konstanta maka untuk sebarang x, f'x = 0


   Bukti:


$$f'(x)= \lim_{h\to 0}\frac{f(x+h)-f(x)}{h} = \lim_{h\to 0}\frac{k-k}{h} = \lim_{h\to 0}0=0$$2. Jika f(x)=x, maka f'(x)=1


   Bukti:


$$f'(x)= \lim_{h\to 0}\frac{f(x+h)-f(x)}{h} = \lim_{h\to 0}\frac{x+h-x}{h}=\lim_{h\to 0}\frac {h}{h}=1$$3. Jika k suatu konstanta dan f suatu fungsi yang terdiferensialkan,


   maka (kf)'(x)= kf'(x)


   Bukti:


   Andaikan F(x) = kf(x), maka


$$F'(x)=\lim_{h\to 0}\frac{F(x+h)-F(x)}{h}=\lim_{h\to 0}\frac{kf(x+h)-kf(x)}{h}$$$$    =\lim_{h\to 0}k \frac{f(x+h)-f(x)}{h}=k\lim_{h\to 0}\frac{f(x+h)-f(x)}{h}$$$$=kf'(x)$$4. Jika f dan g adalah fungsi-fungsi yang terdiferensial,


   maka (f+g)'(x)=f'(x)+g'(x)


   Bukti:


$$F'(x)=\lim_{h\to 0}\frac{f(x+h)+g(x+h)-f(x)+g(x)}{h}$$$$=\lim_{h\to 0}[\frac{f(x+h)-f(x)}{h}+\frac{g(x+h)-g(x)}{h}]$$$$=\lim_{h\to 0}\frac{f(x+h)-f(x)}{h}+\lim_{h\to 0}\frac{g(x+h)-g(x)}{h}=f'(x)+g'(x)$$5. Andaikan f dan g adalah fungsi yang dapat didiferensialkan,


   maka (fg)'(x)=f'(x)g(x)+ f(x)g'(x)


   Bukti:


   Andaikan F(x)=f(x)g(x)


$$F'(x)= \lim_{h\to 0}\frac{F(x+h)-F(x)}{h}$$$$= \lim_{h\to 0}\frac{f(x+h)g(x+h)-f(x)g(x)}{h}$$$$= \lim_{h\to 0}\frac{f(x+h)g(x+h)-f(x+h)g(x)+f(x+h)g(x)-f(x)g(x)}{h}$$$$=\lim_{h\to 0}[f(x+h)\frac{g(x+h)-g(x)+g(x)f(x+h)-f(x)}{h}]$$$$=\lim_{h\to 0} f(x+h)=\lim_{h \to 0}\frac{g(x+h)-g(x)}{h}+g(x)\lim_{h\to 0}\frac{f(x+h)-f(x)}{h}$$$$=f(x)g'(x)+g(x)f'(x)$$6. Andaikan f dan g adalah fungsi yang dapat didiferensialkan


   dengan g(x)tidak sama dengan 0, maka:


$$(\frac{f}{g})(x)=\frac{g(x)f'(x)-f(x)g'(x)}{g(x)^2}$$   Bukti:  
   Andaikan F(x)=f(x)/g(x)  

$$F'(x)= \lim_{h\to 0}\frac{F(x+h)-F(x)}{h}$$$$= \lim_{h\to 0}\frac{\frac{f(x+h)}{g(x+h}-\frac{f(x)}{g(x)}}{h}$$$$= \lim_{h\to 0}\frac{g(x)f(x+h)-f(x)g(x+h)}{h}\frac{1}{g(x)g(x+h)}$$$$= \lim_{h\to 0}[\frac{g(x)f(x+h)-g(x)f(x)+g(x)f(x)-f(x)g(x+h)}{h}\frac{1}{g(x)g(x+h)}]$$$$=\lim_{h\to 0} [g(x)\frac{f(x+h)-f(x)}{h}-f(x)\frac{g(x+h)-g(x)}{h}]\frac{1}{g(x)g(x+h)}$$$$=[g(x)f'(x)-f(x)g'(x)]\frac{1}{g(x)g(x)}$$$$=\frac{g(x)f'(x)-f(x)g'(x)}{g(x)^2}$$## Aplikasi turunan

1. Persamaan gerak suatu partikel dinyatakan dengan rumus


$$s=f(t)=(3t+1)^{\frac{1}{2}}$$   ( s dalam meter dan t dalam detik).  
   Kecepatan partikel tersebut pada saat t=8 adalah ... m/detik.  

   Penyelesaian:  

\>function f(t) &= (3\*t+1)^(1/2); $f(t) 


$$\sqrt{3\,t+1}$$\>function df(t) &= diff(f(t),t); $df(t)


$$\frac{3}{2\,\sqrt{3\,t+1}}$$\>$df(8); fraction %


$$\frac{3}{10}$$  Jadi, kecepatan partikel tersebut pada saat t=8 adalah 0,3 m/detik  

2. Sebuah pabrik baju memerlukan x meter kain untuk diproduksi yang
dinyatakan dengan fungsi:


$$P(x)={\frac{1}{3}}x^2-12x+150$$   (dalam juta rupiah).  
   Berapa biaya produksi minimum yang dikeluarkan oleh pabrik baju  

tersebut?


   Penyelesaian:  

\>function P(x) &= (1/3)\*x^2-12\*x+150; $P(x)


$$\frac{x^2}{3}-12\,x+150$$\>function dP(x) &= diff(P(x),x); $dP(x)


$$\frac{2\,x}{3}-12$$   P(x) akan bernilai minimum jika P'(x)=0, maka:  

\>$dP(x)=0


$$\frac{2\,x}{3}-12=0$$\>$&solve(dP(x),x)


$$\left[ x=18 \right] $$\>P(18)


    42

   Jadi, biaya produksi minimum yang dikeluarkan oleh pabrik tersebut  

adalah 42 juta rupiah.


3. Sebuah peluru ditembakkan ke atas. Jika tinggi h meter setelah t


   detik dirumuskan dengan


$$h(t)=120t-5t^2$$   maka berapa tinggi maksimum yang dicapai peluru tersebut?  

   Penyelesaian:  
   Diketahui:  

$$h(t)=120t-5t^2$$   Turunan pertama fungsi h adalah  

\>function h(t) &= 120\*t-5\*t^2; $h(t)


$$120\,t-5\,t^2$$\>function dh(t) &= diff(h(t),t); $dh(t)


$$120-10\,t$$   Ketinggian maksimum yang dapat dicapai peluru saat t=12, yaitu  

\>$h(12)


$$720$$## Soal-soal Latihan

1. Cari f'(4) dari fungsi


$$f(x) = \frac {2x-1}{x^2-x}$$\>function f(x) &= (2\*x -1)/(x^2-x); $f(x)


$$\frac{2\,x-1}{x^2-x}$$\>function df(x) &= diff(f(x), x); $df(x)


$$\frac{2}{x^2-x}-\frac{\left(2\,x-1\right)^2}{\left(x^2-x\right)^2}$$\>$df(4)


2. Cari turunan dari


$$g(x)=x^2.sin(x)$$\>function g(x) &= x^2\*sin(x)


    
                                   2
                                  x  sin(x)
    

\>function dg(x) &= diff (g(x), x)


    
                                          2
                            2 x sin(x) + x  cos(x)
    

3. Cari turunan dari


$$(4x-7)^2(2x+3)$$\>function f(x) &= (4\*x-7)^2\*(2\*x+3); $f(x)


$$\left(2\,x+3\right)\,\left(4\,x-7\right)^2$$\>function df(x) &= diff(f(x), x); $df(x)


$$2\,\left(4\,x-7\right)^2+8\,\left(2\,x+3\right)\,\left(4\,x-7  \right)$$\>F &= expand(df(x))|simplify; $F


$$96\,x^2-128\,x-70$$4. Temukan turunan dari


$$f(x)=ln(x^3+3x-4)$$\>function f(x) &= ln(x^3+3\*x-4); $f(x)


$$\log \left(x^3+3\,x-4\right)$$\>$showev('diff(f(x),x))


$$\frac{d}{d\,x}\,\log \left(x^3+3\,x-4\right)=\frac{3\,x^2+3}{x^3+3  \,x-4}$$5. Tentukan turunan dari


$$f(x)=cos(5x)+sin(2x)$$\>function f(x) &= cos(5\*x)+sin(2\*x); $f(x)


$$\cos \left(5\,x\right)+\sin \left(2\,x\right)$$\>$showev('diff(f(x),x))


$$\frac{d}{d\,x}\,\left(\cos \left(5\,x\right)+\sin \left(2\,x\right)  \right)=2\,\cos \left(2\,x\right)-5\,\sin \left(5\,x\right)$$6. Sebuah kembang api diluncurkan ke udara. Ketinggian kembang api


   h=(t) (dalam meter) pada t sekon dimodelkan dengan


$$f(t)=16t^2+200t+4$$   Tentukan kecepatan luncur kembang api saat t= 3 sekon.  

Penyelesaian:


\>function f(t) &= 16\*t^2+200\*t+4; $f(t)


$$16\,t^2+200\,t+4$$\>function df(t) &= diff(f(t),t); $df(t)


$$32\,t+200$$\>$df(3); fraction %


$$296$$jadi, kecepatan kembang api saat t=3 adalah 296 m/s


# 4. Integral Tak Tentu

EMT dapat digunakan untuk menghitung integral, baik integral tak tentu
maupun integral tentu.


Pada notebook ini akan ditunjukkan perhitungan integral tentu dengan
menggunakan Teorema Dasar Kalkulus:


Fungsi untuk menentukan integral adalah integrate. Fungsi ini dapat
digunakan untuk menentukan, baik integral tentu maupun tak tentu (jika
fungsinya memiliki antiderivatif).


## CAKUPAN PEMBAHASAN

Definisi


Cara menulis integral pada EMT


Sifat-sifat


Rumus


Kurva


## DEFINISI

Integral Tak Tentu adalah bentuk integral yang variabel integrasinya
tidak memiliki batas sehingga integrasi dari sebuah fungsi akan
menghasilkan banyak kemungkinan dan hanya dinyatakan sebagai
penyelesaian umum. Istilah tak tentu berarti bentuk fungsi F(x) memuat
konstanta real sebarang.


Misalkan diketahui suatu fungsi F(x) yang merupakan fungsi umum yang
memiliki sifat F'(x)=f(x), maka integral tak tentu merupakan himpunan
anti turunan F(x) dari f(x) pada interval negatif tak hingga sampai
positif tak hingga yang dinotasikan :


$$F(x) = \int f(x) dx+c$$## MENULIS INTEGRAL PADA LATEX



Untuk menulis dengan Latex menggunakan fungsi \int


$$f(x)= \int x^3 dx$$$$\int 15x^7 dx$$$$\int x^4 dx$$$$\int 7x^3 dx$$$$\int 5x dx$$## SIFAT INTEGRAL TAK TENTU

1. Sifat Pangkat


   Jika n adalah sembarang bilangan rasional kecuali -1, maka integral
tak tentu dari x^n ditulis :


$$\int x^n dx+c=\frac{x^{n+1}}{n+1} +c$$Contoh:


$$\int x^2 dx+c=\frac{x^{2+1}}{2+1} +c =\frac{x^3}{3} +c$$2. Penjumlahan dan Pengurangan


$$\int[g(x)+f(x)]dx = \int g(x) dx + \int f(x)dx$$$$\int [x^2+4x] dx = \int x^2 dx + \int 4x dx$$$$\int[g(x)-f(x)]dx = \int g(x) dx - \int f(x)dx$$$$\int [x^7-3x] dx = \int x^7 dx - \int 3x dx$$3. Perkalian


Bayangkan f(x) dan g(x) adalah dua fungsi yang bisa kita hitung
integral tak tentu (artinya kita mencari antiturunannya), dan anggap k
adalah suatu angka tetap (konstanta). Maka aturannya berlaku:


$$\int kf(x)dx=k \int f(x)dx$$$$\int 4x^2dx=4 \int x^2dx$$## RUMUS INTEGRAL TAK TENTU



Integral tak tentu berarti nilai atau batasannya belum pasti, sehingga
ada nilai konstanta(c) di dalamnya. Jadi rumus dasar integral tak
tentu adalah :


\>$showev('integrate(x^n,x)+c)


    Answering "Is n equal to -1?" with "no"

$$\int {x^{n}}{\;dx}+c=\frac{x^{n+1}}{n+1}+c$$\>$showev('integrate(x^-1,x)+c)


$$\int {\frac{1}{x}}{\;dx}+c=\log x+c$$Integral dari fungsi


$$f(x)=x^{-1}$$

menghasilkan fungsi ln karena berasal dari teorema kalkulus


## KURVA FUNGSI INTEGRAL/ANTITURUNAN

Kurva fungsi antiturunan adalah kurva yang menggambarkan hubungan
antara suatu fungsi dan antiturunannya. Antiturunan, juga dikenal
sebagai integral.


Jangan lupa untuk menuliskan terhadap variabel apa suatu fungsi
tersebut diintegralkan


1. kurva antiturunan dari fungsi aljabar


$$ f(x)=4x^3 dx$$\>$showev('integrate(4\*x^3,x)+c)


$$4\,\int {x^3}{\;dx}+c=x^4+c$$\>plot2d(["4\*x^3","x^4","x^4+1","x^4+2","x^4+3"]):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-312.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-312.png)

2. kurva antiderivatif fungsi trigonometri dengan


$$f(x)= cos(x)$$\>$showev('integrate(cos(x),x)+c)


$$\int {\cos x}{\;dx}+c=\sin x+c$$\>plot2d(["cos(x)","sin(x)+1","sin(x)+2","sin(x)+3","sin(x)+4"]):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-315.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-315.png)

3. kurva antiderivatif dari fungsi eksponensial dengan


$$f(x)=x e^x$$\>$showev('integrate(x\*E^x,x)+c)


$$\int {x\,e^{x}}{\;dx}+c=\left(x-1\right)\,e^{x}+c$$\>plot2d(["x\*E^x","(x-1)E^x+1","(x-1)E^x+2","(x-1)E^x+3","(x-1)E^x+4"]):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-318.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-318.png)

4. kurva antiderivatif dari fungsi logaritma dengan


$$f(x)=log(4x)$$\>$showev('integrate(log(4\*x),x)+c)


$$\int {\log \left(4\,x\right)}{\;dx}+c=\frac{4\,x\,\log \left(4\,x  \right)-4\,x}{4}+c$$\>plot2d(["log(4\*x)","(4\*x)log(4\*x)-4\*x/4 +1","(4\*x)log(4\*x)-4\*x/4 +2","(4\*x)log(4\*x)-4\*x/4 +3"]):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-321.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-321.png)

## LATIHAN SOAL

1. Tuliskan integral tak tentu dari fungsi aljabar berikut serta
buatlah grafiknya :


$$f(x)=x^5$$\> $showev('integrate(x^5,x)+c)


$$\int {x^5}{\;dx}+c=\frac{x^6}{6}+c$$\>plot2d(["x^5","x^6/6","x^6/6+1","x^6/6+2","x^6/6+3"]):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-324.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-324.png)

2. tentukan integral tak tentu dari fungsi aljabar berikut :


$$f(x)=9x^2$$\>$showev('integrate(9\*x^2,x)+c)


$$9\,\int {x^2}{\;dx}+c=3\,x^3+c$$3. tentukan integral tak tentu dari fungsi trigonometri berikut :


$$f(x)= 2 sin x$$\>$showev('integrate(2\*sin(x),x)+c)


$$2\,\int {\sin x}{\;dx}+c=c-2\,\cos x$$4. tentukan integral tak tentu dari fungsi trigonometri berikut :


$$f(x)= sin x - cos x$$\>$showev('integrate(sin(x)-cos(x),x)+c)


$$\int {\sin x-\cos x}{\;dx}+c=-\sin x-\cos x+c$$5. Tentukan integral tak tentu dari fungsi eksponensial berikut :


$$f(x)=x e^x$$\>$showev('integrate(x\*E^x,x)+c)


$$\int {x\,e^{x}}{\;dx}+c=\left(x-1\right)\,e^{x}+c$$6. Tentukan integral tak tentu dari fungsi


$$\int\frac{\sin(x)}{x}\,dx$$\>$showev('integrate(sin(x)/x, x)+c)


$$\int {\frac{\sin x}{x}}{\;dx}+c=c-\frac{i\,  {\it gamma\_\_incomplete}\left(0 , i\,x\right)-i\,  {\it gamma\_\_incomplete}\left(0 , -i\,x\right)}{2}$$Jawaban dari integral tersebut melibatkan fungsi gamma tidak lengkap
(incomplete gamma function) dengan bilangan kompleks. Hasil ini muncul
karena fungsi dari


$$\frac{sin(x)}{x}$$

tidak memiliki antiturunan dalam bentuk fungsi elementer, sehingga
pada software Euler Mat Toolbox mengembalikan solusi dalam bentuk
fungsi khusus yang lebih umum, seperti fungsi gamma tidak lengkap
dalam kasus ini.


# 5. Integral Tentu

## Pengertian Integral Tentu

Kata “tentu” di sini bermakna sudah pasti atau sudah ditentukan. Oleh
karena itu, Integral tentu adalah integral yang sudah ditentukan
batasan nilai awal dan akhirnya. Batas dari integral tentu adalah a
sampai b atau batas atas sampai batas bawah.


## Rumus Integral Tentu

$$\int_a^b f(x)\ dx = F(b)-F(a), \quad \text{ dengan  } F'(x) = f(x).$$Contoh:


carilah


$$\int_0^\pi sin(x)\ dx$$\>$showev('integrate(sin(x),x,a,b))


$$\int_{a}^{b}{\sin x\;dx}=\cos a-\cos b$$\>$showev('integrate(sin(x),x,0,pi))


$$\int_{0}^{\pi}{\sin x\;dx}=2$$\>plot2d("sin(x)",0,pi):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-340.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-340.png)

Carilah


$$\int_0^2 x^2 \sqrt{2x+1} dx$$\>$showev('integrate(x^2\*sqrt(2\*x+1),x))


$$\int {x^2\,\sqrt{2\,x+1}}{\;dx}=\frac{\left(2\,x+1\right)^{\frac{7  }{2}}}{28}-\frac{\left(2\,x+1\right)^{\frac{5}{2}}}{10}+\frac{\left(  2\,x+1\right)^{\frac{3}{2}}}{12}$$\>$showev('integrate(x^2\*sqrt(2\*x+1),x,0,2))


$$\int_{0}^{2}{x^2\,\sqrt{2\,x+1}\;dx}=\frac{2\,5^{\frac{5}{2}}}{21}-  \frac{2}{105}$$\>$ratsimp(%)


$$\int_{0}^{2}{x^2\,\sqrt{2\,x+1}\;dx}=\frac{2\,5^{\frac{7}{2}}-2}{  105}$$\>$showev('integrate((sin(sqrt(x)+a)\*E^sqrt(x))/sqrt(x),x,0,pi^2))


$$\int_{0}^{\pi^2}{\frac{\sin \left(\sqrt{x}+a\right)\,e^{\sqrt{x}}}{  \sqrt{x}}\;dx}=\left(-e^{\pi}-1\right)\,\sin a+\left(e^{\pi}+1  \right)\,\cos a$$\>$factor(%)


$$\int_{0}^{\pi^2}{\frac{\sin \left(\sqrt{x}+a\right)\,e^{\sqrt{x}}}{  \sqrt{x}}\;dx}=\left(-e^{\pi}-1\right)\,\left(\sin a-\cos a\right)$$\>function map f(x) &= E^(-x^2)


    
                                        2
                                     - x
                                    E
    

\>$showev('integrate(f(x),x))


$$\int {e^ {- x^2 }}{\;dx}=\frac{\sqrt{\pi}\,\mathrm{erf}\left(x  \right)}{2}$$Fungsi f tidak memiliki antiturunan, integralnya masih memuat integral
lain.


$$erf(x) = \int \frac{e^{-x^2}}{\sqrt{\pi}} \ dx.$$Kita tidak dapat menggunakan teorema Dasar kalkulus untuk menghitung
integral tentu fungsi tersebut jika semua batasnya berhingga. Dalam
hal ini dapat digunakan metode numerik (rumus kuadratur).


Misalkan kita akan menghitung:


$$\int_{0}^{\pi}{e^ {- x^2 }\;dx}$$\>x=0:0.1:pi-0.1; plot2d(x,f(x+0.1),\>bar); plot2d("f(x)",0,pi,\>add):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-350.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-350.png)

Integral tentu


$$\int_{0}^{\pi}{e^ {- x^2 }\;dx}$$dapat dihampiri dengan jumlah luas persegi-persegi panjang di bawah
kurva y=f(x) tersebut. Langkah-langkahnya adalah sebagai berikut.


\>t &= makelist(a,a,0,pi-0.1,0.1);


 mendefinisikan t sebagai list untuk menyimpan nilai-nilai x  

\>fx &= makelist(f(t[i]+0.1),i,1,length(t)); 


simpan nilai-nilai f(x) dan jangan menggunakan x sebagai list


Hasilnya adalah:


$$\int_{0}^{\pi}{e^ {- x^2 }\;dx}=0.1950839272901491$$Jumlah tersebut diperoleh dari hasil kali lebar sub-subinterval (=0.1)
dan jumlah nilai-nilai f(x) untuk x = 0.1, 0.2, 0.3, ..., 3.2.


\>0.1\*sum(f(x+0.1))


    0.836219610253

Untuk mendapatkan nilai integral tentu yang mendekati nilai
sebenarnya, lebar sub-intervalnya dapat diperkecil lagi, sehingga
daerah di bawah kurva tertutup semuanya, misalnya dapat digunakan
lebar subinterval 0.001.


\>x=0:0.001:pi-0.1; plot2d(x,f(x+0.1),\>bar); plot2d("f(x)",0,pi,\>add):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-353.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-353.png)

Berikut adalah contoh lain fungsi yang tidak memiliki antiderivatif,
sehingga integral tentunya hanya dapat dihitung dengan metode numerik.


\>function f(x) &= x^x


    
                                       x
                                      x
    

\>$showev('integrate(f(x),x,0,1))


$$\int_{0}^{1}{x^{x}\;dx}=\int_{0}^{1}{x^{x}\;dx}$$\>x=0:0.1:1-0.01; plot2d(x,f(x+0.01),\>bar); plot2d("f(x)",0,1,\>add):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-355.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-355.png)

Karena maxima gagal menghitung integral tentu tersebut secara langsung
menggunakan perintah integrate. Untuk mendapat hasil atau pendekatan
nilai integral tentu tersebut kita lakukan seperti contoh sebelumnya.


\>t &= makelist(a,a,0,1-0.01,0.01);

\>fx &= makelist(f(t[i]+0.01),i,1,length(t));


$$\int_{0}^{1}{x^{x}\;dx}=0.7834935879025506$$\>function f(x) &= sin(3\*x^5+7)^2; $f(x)


$$\sin ^2\left(3\,x^5+7\right)$$\>integrate(f,0,1)


    0.542581176074

## Sifat - Sifat Integral Tentu

1. Linearitas


sifat 1: Jika c adalah konstanta, maka:


$$\int_a^b c f(x) dx = c \int_a^b f(x) dx$$

Sifat 2: Jika f(x) dan g(x) adalah dua fungsi yang terintegralkan pada
interval [a, b], maka:


$$\int_a^b (f(x) + g(x)) dx = \int_a^b f(x) dx + \int_a^b g(x) dx$$2. Interval


Sifat 3: Jika a &lt; c &lt; b, maka:


$$\int_a^b f(x) dx = \int_a^c f(x) dx + \int_c^b f(x) dx$$3. Fungsi Genap dan Ganjil


Fungsi Genap: Jika f(x) adalah fungsi genap (yaitu, f(-x) = f(x)),
maka:


$$\int_{-a}^a f(x) dx = 2 \int_0^a f(x) dx$$

Fungsi Ganjil: Jika f(x) adalah fungsi ganjil (yaitu, f(-x) = -f(x)),
maka:


$$\int_{-a}^a f(x) dx = 0$$4. Batas Integral Bertukar


$$\int_b^a f(x) dx = -\int_a^b f(x) dx$$## Aplikasi Integral Tentu

## Aplikasi Integral Tentu pada Panjang Kurva

Sebuah jalan tol memiliki bentuk lengkungan yang dapat dimodelkan
dengan persamaan y = x^2 dari titik x = 0 hingga x = 2 (dalam
kilometer). Berapakah panjang jalan tol tersebut


Penyelesaian:


$$s = \int_0^2 \sqrt{1 +(2x)^2} dx ol memiliki bentuk lengkungan yang dapat dimodelkan dengan persamaan y = x^2 dari titik x = 0 hingga x = 2 (dalam kilometer). Berapakah panjang jalan tol tersebut$$Penyelesaian:


$$s = \int_0^2 \sqrt{1 +(2x)^2} dx$$\>$showev('integrate(sqrt(1 + (2\*x)^2),x,0,2))


$$\int_{0}^{2}{\sqrt{4\,x^2+1}\;dx}=\frac{{\rm asinh}\; 4+4\,\sqrt{17  }}{4}$$\>$float(%)


$$\int_{0.0}^{2.0}{\sqrt{4.0\,x^2+1.0}\;dx}=4.646783762432936$$Hitunglah panjang kurva berikut ini dan luas daerah di dalam kurva
tersebut.


$$\gamma(t) = (r(t) \cos(t), r(t) \sin(t))$$dengan


$$r(t) = 1 + \dfrac{\sin(3t)}{2},\quad 0\le t\le 2\pi.$$\>t=linspace(0,2pi,1000); r=1+sin(3\*t)/2; x=r\*cos(t); y=r\*sin(t); ...  
\>   plot2d(x,y,\>filled,fillcolor=red,style="/",r=1.5):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-370.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-370.png)

\>function r(t) &= 1+sin(3\*t)/2; $'r(t)


$$r\left(\left[ 0 , 0.01 , 0.02 , 0.03 , 0.04 , 0.05 , 0.06 , 0.07 ,   0.08 , 0.09 , 0.1 , 0.11 , 0.12 , 0.13 , 0.14 , 0.15 , 0.16 , 0.17   , 0.18 , 0.19 , 0.2 , 0.21 , 0.2200000000000001 ,   0.2300000000000001 , 0.2400000000000001 , 0.2500000000000001 ,   0.2600000000000001 , 0.2700000000000001 , 0.2800000000000001 ,   0.2900000000000001 , 0.3000000000000001 , 0.3100000000000001 ,   0.3200000000000001 , 0.3300000000000001 , 0.3400000000000001 ,   0.3500000000000001 , 0.3600000000000002 , 0.3700000000000002 ,   0.3800000000000002 , 0.3900000000000002 , 0.4000000000000002 ,   0.4100000000000002 , 0.4200000000000002 , 0.4300000000000002 ,   0.4400000000000002 , 0.4500000000000002 , 0.4600000000000002 ,   0.4700000000000003 , 0.4800000000000003 , 0.4900000000000003 ,   0.5000000000000002 , 0.5100000000000002 , 0.5200000000000002 ,   0.5300000000000002 , 0.5400000000000003 , 0.5500000000000003 ,   0.5600000000000003 , 0.5700000000000003 , 0.5800000000000003 ,   0.5900000000000003 , 0.6000000000000003 , 0.6100000000000003 ,   0.6200000000000003 , 0.6300000000000003 , 0.6400000000000003 ,   0.6500000000000004 , 0.6600000000000004 , 0.6700000000000004 ,   0.6800000000000004 , 0.6900000000000004 , 0.7000000000000004 ,   0.7100000000000004 , 0.7200000000000004 , 0.7300000000000004 ,   0.7400000000000004 , 0.7500000000000004 , 0.7600000000000005 ,   0.7700000000000005 , 0.7800000000000005 , 0.7900000000000005 ,   0.8000000000000005 , 0.8100000000000005 , 0.8200000000000005 ,   0.8300000000000005 , 0.8400000000000005 , 0.8500000000000005 ,   0.8600000000000005 , 0.8700000000000006 , 0.8800000000000006 ,   0.8900000000000006 , 0.9000000000000006 , 0.9100000000000006 ,   0.9200000000000006 , 0.9300000000000006 , 0.9400000000000006 ,   0.9500000000000006 , 0.9600000000000006 , 0.9700000000000006 ,   0.9800000000000006 , 0.9900000000000007 \right] \right)$$\>function fx(t) &= r(t)\*cos(t); $'fx(t)=fx(t)


$${\it fx}\left(\left[ 0 , 0.01 , 0.02 , 0.03 , 0.04 , 0.05 , 0.06 ,   0.07 , 0.08 , 0.09 , 0.1 , 0.11 , 0.12 , 0.13 , 0.14 , 0.15 , 0.16   , 0.17 , 0.18 , 0.19 , 0.2 , 0.21 , 0.2200000000000001 ,   0.2300000000000001 , 0.2400000000000001 , 0.2500000000000001 ,   0.2600000000000001 , 0.2700000000000001 , 0.2800000000000001 ,   0.2900000000000001 , 0.3000000000000001 , 0.3100000000000001 ,   0.3200000000000001 , 0.3300000000000001 , 0.3400000000000001 ,   0.3500000000000001 , 0.3600000000000002 , 0.3700000000000002 ,   0.3800000000000002 , 0.3900000000000002 , 0.4000000000000002 ,   0.4100000000000002 , 0.4200000000000002 , 0.4300000000000002 ,   0.4400000000000002 , 0.4500000000000002 , 0.4600000000000002 ,   0.4700000000000003 , 0.4800000000000003 , 0.4900000000000003 ,   0.5000000000000002 , 0.5100000000000002 , 0.5200000000000002 ,   0.5300000000000002 , 0.5400000000000003 , 0.5500000000000003 ,   0.5600000000000003 , 0.5700000000000003 , 0.5800000000000003 ,   0.5900000000000003 , 0.6000000000000003 , 0.6100000000000003 ,   0.6200000000000003 , 0.6300000000000003 , 0.6400000000000003 ,   0.6500000000000004 , 0.6600000000000004 , 0.6700000000000004 ,   0.6800000000000004 , 0.6900000000000004 , 0.7000000000000004 ,   0.7100000000000004 , 0.7200000000000004 , 0.7300000000000004 ,   0.7400000000000004 , 0.7500000000000004 , 0.7600000000000005 ,   0.7700000000000005 , 0.7800000000000005 , 0.7900000000000005 ,   0.8000000000000005 , 0.8100000000000005 , 0.8200000000000005 ,   0.8300000000000005 , 0.8400000000000005 , 0.8500000000000005 ,   0.8600000000000005 , 0.8700000000000006 , 0.8800000000000006 ,   0.8900000000000006 , 0.9000000000000006 , 0.9100000000000006 ,   0.9200000000000006 , 0.9300000000000006 , 0.9400000000000006 ,   0.9500000000000006 , 0.9600000000000006 , 0.9700000000000006 ,   0.9800000000000006 , 0.9900000000000007 \right] \right)=\left[ 1 ,   1.014947000636657 , 1.029776013705529 , 1.044469087191079 ,   1.059008331806833 , 1.073375947255439 , 1.087554248364218 ,   1.101525691055367 , 1.11527289811021 , 1.128778684687222 ,   1.142026083553954 , 1.154998369993414 , 1.16767908634602 ,   1.180052066148761 , 1.192101457833886 , 1.203811747950136 ,   1.215167783870255 , 1.226154795949382 , 1.236758419099762 ,   1.246964713748154 , 1.256760186143285 , 1.266131807981756 ,   1.275067035321848 , 1.283553826755846 , 1.29158066081265 ,   1.29913655256367 , 1.306211069406282 , 1.312794346000405 ,   1.318877098335118 , 1.324450636903608 , 1.329506878966172 ,   1.334038359882425 , 1.338038243495345 , 1.341500331551311 ,   1.344419072141793 , 1.346789567153917 , 1.348607578718725 ,   1.349869534647481 , 1.350572532848044 , 1.350714344714907 ,   1.350293417488142 , 1.349308875578123 , 1.347760520854542 ,   1.345648831899879 , 1.342974962229111 , 1.339740737479097 ,   1.335948651572729 , 1.331601861864506 , 1.326704183275865 ,   1.321260081430156 , 1.315274664798767 , 1.308753675871437 ,   1.301703481365363 , 1.294131061489226 , 1.286043998279732 ,   1.277450463029762 , 1.268359202828647 , 1.25877952623647 ,   1.248721288115691 , 1.238194873644713 , 1.227211181539273 ,   1.215781606508839 , 1.203918020976346 , 1.191632756090801 ,   1.17893858206338 , 1.165848687858719 , 1.152376660274093 ,   1.138536462440146 , 1.124342411777761 , 1.10980915744646 ,   1.094951657320579 , 1.079785154530145 , 1.064325153604093 ,   1.04858739625406 , 1.032587836837555 , 1.0163426175398 ,   0.999868043313951 , 0.9831805566197906 , 0.9662967120012925 ,   0.9492331505436565 , 0.932006574250646 , 0.9146337203831 ,   0.897131335799599 , 0.8795161513401855 , 0.8618048562939812 ,   0.8440140729913906 , 0.8261603315613344 , 0.8082600448937051 ,   0.7903294838468643 , 0.7723847527396025 , 0.754441765166499 ,   0.7365162201750889 , 0.7186235788426429 , 0.7007790412897039 ,   0.6829975241668103 , 0.6652936386500562 , 0.6476816689803099 ,   0.6301755515800127 , 0.6127888547805567 , 0.595534759192214 \right] $$\>function fy(t) &= r(t)\*sin(t); $'fy(t)=fy(t)


$${\it fy}\left(\left[ 0 , 0.01 , 0.02 , 0.03 , 0.04 , 0.05 , 0.06 ,   0.07 , 0.08 , 0.09 , 0.1 , 0.11 , 0.12 , 0.13 , 0.14 , 0.15 , 0.16   , 0.17 , 0.18 , 0.19 , 0.2 , 0.21 , 0.2200000000000001 ,   0.2300000000000001 , 0.2400000000000001 , 0.2500000000000001 ,   0.2600000000000001 , 0.2700000000000001 , 0.2800000000000001 ,   0.2900000000000001 , 0.3000000000000001 , 0.3100000000000001 ,   0.3200000000000001 , 0.3300000000000001 , 0.3400000000000001 ,   0.3500000000000001 , 0.3600000000000002 , 0.3700000000000002 ,   0.3800000000000002 , 0.3900000000000002 , 0.4000000000000002 ,   0.4100000000000002 , 0.4200000000000002 , 0.4300000000000002 ,   0.4400000000000002 , 0.4500000000000002 , 0.4600000000000002 ,   0.4700000000000003 , 0.4800000000000003 , 0.4900000000000003 ,   0.5000000000000002 , 0.5100000000000002 , 0.5200000000000002 ,   0.5300000000000002 , 0.5400000000000003 , 0.5500000000000003 ,   0.5600000000000003 , 0.5700000000000003 , 0.5800000000000003 ,   0.5900000000000003 , 0.6000000000000003 , 0.6100000000000003 ,   0.6200000000000003 , 0.6300000000000003 , 0.6400000000000003 ,   0.6500000000000004 , 0.6600000000000004 , 0.6700000000000004 ,   0.6800000000000004 , 0.6900000000000004 , 0.7000000000000004 ,   0.7100000000000004 , 0.7200000000000004 , 0.7300000000000004 ,   0.7400000000000004 , 0.7500000000000004 , 0.7600000000000005 ,   0.7700000000000005 , 0.7800000000000005 , 0.7900000000000005 ,   0.8000000000000005 , 0.8100000000000005 , 0.8200000000000005 ,   0.8300000000000005 , 0.8400000000000005 , 0.8500000000000005 ,   0.8600000000000005 , 0.8700000000000006 , 0.8800000000000006 ,   0.8900000000000006 , 0.9000000000000006 , 0.9100000000000006 ,   0.9200000000000006 , 0.9300000000000006 , 0.9400000000000006 ,   0.9500000000000006 , 0.9600000000000006 , 0.9700000000000006 ,   0.9800000000000006 , 0.9900000000000007 \right] \right)=\left[ 0 ,   0.01014980833556662 , 0.02059826678292271 , 0.03134347622283015 ,   0.04238293991838228 , 0.05371356612987439 , 0.06533167172990376 ,   0.07723298681299934 , 0.08941266029246918 , 0.1018652664755576 ,   0.1145848126064173 , 0.1275647473648353 , 0.1407979703071057 ,   0.1542768422339107 , 0.1679931964685752 , 0.1819383510275811 ,   0.1961031216637831 , 0.2104778357613507 , 0.2250523470600841 ,   0.2398160511854019 , 0.2547579019589912 , 0.2698664284638497 ,   0.2851297528362152 , 0.3005356087557041 , 0.3160713606038417 ,   0.3317240232600813 , 0.3474802825033731 , 0.3633265159863522 ,   0.3792488147482899 , 0.3952330052320643 , 0.411264671769591 ,   0.4273291794993832 , 0.4434116976792021 , 0.4594972233561165 ,   0.4755706053556919 , 0.4916165685515136 , 0.5076197383757777 ,   0.5235646655312819 , 0.5394358508648145 , 0.5552177703616642 ,   0.5708949002207642 , 0.5864517419698421 , 0.6018728475798654 ,   0.6171428445380648 , 0.6322464608388652 , 0.6471685498521687 ,   0.6618941150286309 , 0.6764083344018014 , 0.6906965848473219 ,   0.704744466059751 , 0.7185378242080237 , 0.7320627752310482 ,   0.7453057277355214 , 0.7582534054586558 , 0.7708928692592016 ,   0.7832115386008901 , 0.7951972124932317 , 0.8068380898554457 ,   0.8181227892702304 , 0.8290403680950348 , 0.8395803408995157 ,   0.8497326971989371 , 0.8594879184543822 , 0.8688369943118147 ,   0.877771438053233 , 0.8862833012344233 , 0.894365187485098 ,   0.9020102654485477 , 0.9092122808393135 , 0.91596556759876 ,   0.9222650581299157 , 0.9281062925943645 , 0.9334854272555032 ,   0.9383992418539865 , 0.9428451460027243 , 0.9468211845903713 ,   0.9503260421838114 , 0.9533590464217597 , 0.9559201703932094 ,   0.9580100339960551 , 0.9596299042728891 , 0.9607816947225576 ,   0.9614679635877484 , 0.9616919111204768 , 0.9614573758289937 ,   0.9607688297112769 , 0.9596313724818526 , 0.9580507248003547 ,   0.9560332205117796 , 0.9535857979100135 , 0.950715990037748 ,   0.9474319140374602 , 0.9437422595696462 , 0.9396562763159917 ,   0.9351837605866338 , 0.9303350410521015 , 0.9251209636219332 ,   0.9195528754933222 , 0.9136426083945087 , 0.9074024610488752   \right] $$\>function ds(t) &= trigreduce(radcan(sqrt(diff(fx(t),t)^2+diff(fy(t),t)^2))); $'ds(t)=ds(t)


$${\it ds}\left(t\right)=\sqrt{\left(\frac{d}{d\,t}\,{\it fy}\left(t  \right)\right)^2+\left(\frac{d}{d\,t}\,{\it fx}\left(t\right)\right)  ^2}$$\>$integrate(ds(x),x,0,2\*pi) //panjang (keliling) kurva


$$\int_{0}^{2\,\pi}{\sqrt{\left(\frac{d}{d\,x}\,{\it fy}\left(x  \right)\right)^2+\left(\frac{d}{d\,x}\,{\it fx}\left(x\right)\right)  ^2}\;dx}$$Spiral Logaritmik


\>a=0.1; plot2d("exp(a\*x)\*cos(x)","exp(a\*x)\*sin(x)",r=2,xmin=0,xmax=2\*pi)

\>&kill(a) // hapus expresi a


    
                                     done
    

\>function fx(t) &= exp(a\*t)\*cos(t); $'fx(t)=fx(t)


$${\it fx}\left(t\right)=e^{a\,t}\,\cos t$$\>function fy(t) &= exp(a\*t)\*sin(t); $'fy(t)=fy(t)


$${\it fy}\left(t\right)=e^{a\,t}\,\sin t$$\>function df(t) &= trigreduce(radcan(sqrt(diff(fx(t),t)^2+diff(fy(t),t)^2))); $'df(t)=df(t)


$${\it df}\left(t\right)=\sqrt{a^2+1}\,e^{a\,t}$$\>S &=integrate(df(t),t,0,2\*%pi); $S // panjang kurva (spiral)


$$\sqrt{a^2+1}\,\left(\frac{e^{2\,\pi\,a}}{a}-\frac{1}{a}\right)$$\>S(a=0.1) // Panjang kurva untuk a=0.1


    8.78817491636

Soal:


Tunjukkan bahwa keliling lingkaran dengan jari-jari r adalah K=2.pi.r.


Penyelesaian:


Lingkaran dalam Koordinat Kartesius: Kita dapat merepresentasikan
suatu lingkaran dengan pusat di titik asal (0,0) dan jari-jari r
dengan persamaan parametrik berikut:


$$x(t) = r \cos(t)$$$$y(t) = r \sin(t)$$

di mana t adalah parameter yang bervariasi dari 0 hingga 2p.


Panjang Kurva Parametrik: Panjang kurva parametrik (x(t), y(t)) dari
t=a hingga t=b dapat dihitung dengan integral:


$$s = \int_a^b \sqrt{\left(\frac{dx}{dt}\right)^2 + \left(\frac{dy}{dt}\right)^2} dt$$1. Mencari Turunan


$$x(t) = r \cos(t)$$\>&showev('diff(r\*cos(t),t))


    
                          d
                          -- (r cos(t)) = - r sin(t)
                          dt
    

\>&showev('diff(r\*sin(t),t))


    
                           d
                           -- (r sin(t)) = r cos(t)
                           dt
    

2. Substitusi ke Rumus Panjang Kurva:


$$s = \int_0^{2\pi} \sqrt{(-r \sin(t))^2 + (r \cos(t))^2} dt$$$$s = \int_0^{2\pi} \sqrt{r^2 (\sin^2(t) + \cos^2(t))} dt$$

Karena


$$sin^2(t) + cos^2(t) = 1,$$

maka:


$$s = \int_0^{2\pi} r dt$$3. Integral


$$s = r \int_0^{2\pi} dt = r[t]_0^{2\pi} = r(2p - 0) = 2\pi r$$Berikut adalah contoh menghitung panjang parabola.


\>plot2d("x^2",xmin=-1,xmax=1):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-389.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-389.png)

\>$showev('integrate(sqrt(1+diff(x^2,x)^2),x,-1,1))


$$\int_{-1}^{1}{\sqrt{4\,x^2+1}\;dx}=\frac{{\rm asinh}\; 2+2\,\sqrt{5  }}{2}$$\>$float(%)


$$\int_{-1.0}^{1.0}{\sqrt{4.0\,x^2+1.0}\;dx}=2.957885715089195$$\>x=-1:0.2:1; y=x^2; plot2d(x,y);  ...  
\>   plot2d(x,y,points=1,style="o#",add=1):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-392.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-392.png)

Panjang tersebut dapat dihampiri dengan menggunakan jumlah panjang
ruas-ruas garis yang menghubungkan titik-titik pada parabola tersebut.


\>i=1:cols(x)-1; sum(sqrt((x[i+1]-x[i])^2+(y[i+1]-y[i])^2))


    2.95191957027

Hasilnya mendekati panjang yang dihitung secara eksak. Untuk
mendapatkan hampiran yang cukup akurat, jarak antar titik dapat
diperkecil, misalnya 0.1, 0.05, 0.01, dan seterusnya. Cobalah Anda
ulangi perhitungannya dengan nilai-nilai tersebut.


## Koordinat Kartesius

Berikut diberikan contoh perhitungan panjang kurva menggunakan
koordinat Kartesius. Kita akan hitung panjang kurva dengan persamaan
implisit:


$$x^3+y^3-3xy=0.$$\>z &= x^3+y^3-3\*x\*y; $z


$$y^3-3\,x\,y+x^3$$\>plot2d(z,r=2,level=0,n=100):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-395.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-395.png)

Kita tertarik pada kurva di kuadran pertama.


\>plot2d(z,a=0,b=2,c=0,d=2,level=[-10;0],n=100,contourwidth=3,style="/"):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-396.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-396.png)

Kita selesaikan persamaannya untuk x.


\>$z with y=l\*x, sol &= solve(%,x); $sol


$$\left[ x=\frac{3\,l}{l^3+1} , x=0 \right] $$![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-398.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-398.png)

Kita gunakan solusi tersebut untuk mendefinisikan fungsi dengan
Maxima.


\>function f(l) &= rhs(sol[1]); $'f(l)=f(l)


$$f\left(l\right)=\frac{3\,l}{l^3+1}$$Fungsi tersebut juga dapat digunaka untuk menggambar kurvanya. Ingat,
bahwa fungsi tersebut adalah nilai x dan nilai y=l*x, yakni x=f(l) dan
y=l*f(l).


\>plot2d(&f(x),&x\*f(x),xmin=-0.5,xmax=2,a=0,b=2,c=0,d=2,r=1.5):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-400.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-400.png)

Elemen panjang kurva adalah:


$$ds=\sqrt{f'(l)^2+(lf'(l)+f(l))^2}.$$\>function ds(l) &= ratsimp(sqrt(diff(f(l),l)^2+diff(l\*f(l),l)^2)); $'ds(l)=ds(l)


$${\it ds}\left(l\right)=\frac{\sqrt{9\,l^8+36\,l^6-36\,l^5-36\,l^3+  36\,l^2+9}}{\sqrt{l^{12}+4\,l^9+6\,l^6+4\,l^3+1}}$$\>$integrate(ds(l),l,0,1)


$$\int_{0}^{1}{\frac{\sqrt{9\,l^8+36\,l^6-36\,l^5-36\,l^3+36\,l^2+9}  }{\sqrt{l^{12}+4\,l^9+6\,l^6+4\,l^3+1}}\;dl}$$Integral tersebut tidak dapat dihitung secara eksak menggunakan
Maxima. Kita hitung integral etrsebut secara numerik dengan Euler.
Karena kurva simetris, kita hitung untuk nilai variabel integrasi dari
0 sampai 1, kemudian hasilnya dikalikan 2.


\>2\*integrate("ds(x)",0,1)


    4.91748872168

\>2\*romberg(&ds(x),0,1)// perintah Euler lain untuk menghitung nilai hampiran integral 


    4.91748872168

Perhitungan di datas dapat dilakukan untuk sebarang fungsi x dan y
dengan mendefinisikan fungsi EMT, misalnya kita beri nama
panjangkurva. Fungsi ini selalu memanggil Maxima untuk menurunkan
fungsi yang diberikan.


\>function panjangkurva(fx,fy,a,b) ...


    $ds=mxm("sqrt(diff(@fx,x)^2+diff(@fy,x)^2)");
    return romberg(ds,a,b);
    $endfunction
</pre>
\>panjangkurva("x","x^2",-1,1)


    2.95788571509

Bandingkan dengan nilai eksak di atas.


\>2\*panjangkurva(mxm("f(x)"),mxm("x\*f(x)"),0,1)


    4.91748872168

Kita hitung panjang spiral Archimides berikut ini dengan fungsi
tersebut.


\>plot2d("x\*cos(x)","x\*sin(x)",xmin=0,xmax=2\*pi,square=1):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-404.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-404.png)

\>panjangkurva("x\*cos(x)","x\*sin(x)",0,2\*pi)


    21.2562941482

Berikut kita definisikan fungsi yang sama namun dengan Maxima, untuk
perhitungan eksak.


\>&kill(ds,x,fx,fy)


    
                                     done
    

\>function ds(fx,fy) &&= sqrt(diff(fx,x)^2+diff(fy,x)^2)


    
                               2              2
                      sqrt(diff (fy, x) + diff (fx, x))
    

\>sol &= ds(x\*cos(x),x\*sin(x)); $sol


$$\sqrt{\left(\cos x-x\,\sin x\right)^2+\left(\sin x+x\,\cos x\right)  ^2}$$\>$sol | trigreduce | expand, $integrate(%,x,0,2\*pi), %()


$$\frac{{\rm asinh}\; \left(2\,\pi\right)+2\,\pi\,\sqrt{4\,\pi^2+1}}{  2}$$![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-407.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-407.png)

    21.2562941482

Hasilnya sama dengan perhitungan menggunakan fungsi EMT.


Berikut adalah contoh lain penggunaan fungsi Maxima tersebut.


\>plot2d("3\*x^2-1","3\*x^3-1",xmin=-1/sqrt(3),xmax=1/sqrt(3),square=1):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-408.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-408.png)

\>sol &= radcan(ds(3\*x^2-1,3\*x^3-1)); $sol


$$3\,x\,\sqrt{9\,x^2+4}$$\>$showev('integrate(sol,x,0,1/sqrt(3))), $2\*float(%) // panjang kurva di atas


$$6.0\,\int_{0.0}^{0.5773502691896258}{x\,\sqrt{9.0\,x^2+4.0}\;dx}=  2.337835372767141$$![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-411.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-411.png)

## Sikloid

Berikut kita akan menghitung panjang kurva lintasan (sikloid) suatu
titik pada lingkaran yang berputar ke kanan pada permukaan datar.
Misalkan jari-jari lingkaran tersebut adalah r. Posisi titik pusat
lingkaran pada saat t adalah:


$$(rt,r).$$Misalkan posisi titik pada lingkaran tersebut mula-mula (0,0) dan
posisinya pada saat t adalah:


$$(r(t-\sin(t)),r(1-\cos(t))).$$Berikut kita plot lintasan tersebut dan beberapa posisi lingkaran
ketika t=0, t=pi/2, t=r*pi.


\>function x &= r\*(t-sin(t))


    
                                r (t - sin(t))
    

\>function y &= r\*(1-cos(t))


    
                                r (1 - cos(t))
    

Berikut kita gambar sikloid untuk r=1.


\>ex &= x-sin(x); ey &= 1-cos(x); aspect(1);

\>plot2d(ex,ey,xmin=0,xmax=4pi,square=1); ...  
\>   plot2d("2+cos(x)","1+sin(x)",xmin=0,xmax=2pi,\>add,color=blue); ...  
\>   plot2d([2,ex(2)],[1,ey(2)],color=red,\>add); ...  
\>   plot2d(ex(2),ey(2),\>points,\>add,color=red); ...  
\>   plot2d("2pi+cos(x)","1+sin(x)",xmin=0,xmax=2pi,\>add,color=blue); ...  
\>   plot2d([2pi,ex(2pi)],[1,ey(2pi)],color=red,\>add);  ...  
\>   plot2d(ex(2pi),ey(2pi),\>points,\>add,color=red):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-414.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-414.png)

\>ds &= radcan(sqrt(diff(ex,x)^2+diff(ey,x)^2)); $ds=trigsimp(ds) 


$$\sqrt{\sin ^2x+\cos ^2x-2\,\cos x+1}=\sqrt{2-2\,\cos x}$$\>ds &= trigsimp(ds); $ds


$$\sqrt{2-2\,\cos x}$$\>$showev('integrate(ds,x,0,2\*pi)) 


$$\int_{0}^{2\,\pi}{\sqrt{2-2\,\cos x}\;dx}=8$$\>integrate(mxm("ds"),0,2\*pi) // hitung secara numerik


    8

Perhatikan, seperti terlihat pada gambar, panjang sikloid lebih besar
daripada keliling lingkarannya, yakni:


$$2\pi.$$## Kurvatur (Kelengkungan) Kurva

![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-419.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-419.png)

Aslinya, kelengkungan kurva diferensiabel (yakni, kurva mulus yang
tidak lancip) di titik P didefinisikan melalui lingkaran oskulasi
(yaitu, lingkaran yang melalui titik P dan terbaik memperkirakan,
paling banyak menyinggung kurva di sekitar P). Pusat dan radius
kelengkungan kurva di P adalah pusat dan radius lingkaran oskulasi.
Kelengkungan adalah kebalikan dari radius kelengkungan:


$$\kappa =\frac {1}{R}$$dengan R adalah radius kelengkungan. (Setiap lingkaran memiliki
kelengkungan ini pada setiap titiknya, dapat diartikan, setiap
lingkaran berputar 2pi sejauh 2piR.)


Definisi ini sulit dimanipulasi dan dinyatakan ke dalam rumus untuk
kurva umum. Oleh karena itu digunakan definisi lain yang ekivalen.


# 6. Barisan dan Deret

Barisan adalah susunan bilangan yang memiliki pola atau karakteristik
tertentu, sedangkan deret adalah hasil penjumlahan dari
anggota-anggota dalam barian tertentu.


Barisan dapat didefinisikan dengan beberapa cara di dalam EMT, di
antaranya:


- menggunakan titik dua ":", sama seperti saat mendefinisikan vektor
dengan elemen-elemen beraturan


- menggunakan perintah "sequence" dan rumus barisan (suku ke -n);


- menggunakan perintah "iterate" atau "niterate";


- menggunakan fungsi Maxima "create_list" atau "makelist" untuk
menghasilkan barisan simbolik;


- menggunakan fungsi biasa yang inputnya vektor atau barisan;


- menggunakan fungsi rekursif.


EMT menyediakan beberapa perintah (fungsi) terkait barisan, yakni:


- sum: menghitung jumlah semua elemen suatu barisan


- cumsum: jumlah kumulatif suatu barisan


- differences: selisih antar elemen-elemen berturutan


EMT juga dapat digunakan untuk menghitung jumlah deret berhingga
maupun deret tak hingga, dengan menggunakan perintah (fungsi) "sum".
Perhitungan dapat dilakukan secara numerik maupun simbolik dan eksak.


Contoh perhitungan barisan dan deret menggunakan EMT.


## Menggunakan titik dua

\>1:15


    [1,  2,  3,  4,  5,  6,  7,  8,  9,  10,  11,  12,  13,  14,  15]

\>1:3:30


    [1,  4,  7,  10,  13,  16,  19,  22,  25,  28]

\>sum(1:3:30)


    145

\>cumsum(1:3:30)


    [1,  5,  12,  22,  35,  51,  70,  92,  117,  145]

## Menggunakan perintah "sequence" dan rumus barisan (suku ke -n)

Untuk barisan yang lebih kompleks dapat digunakan fungsi "sequence()".
Fungsi ini menghitung nilai-nilai x[n] dari semua nilai sebelumnya,
x[1],...,x[n-1] yang diketahui.


Berikut adalah contoh barisan Fibonacci.


$$x_n = x_{n-1}+x_{n-2},\quad x_1=1,\quad x_2 =1$$\>sequence("x[n-1]+x[n-2]",[1,1],15) //suku ke satu :1, suku ke dua :1


    [1,  1,  2,  3,  5,  8,  13,  21,  34,  55,  89,  144,  233,  377,  610]

\>plot2d(sequence("x[n-1]+x[n-2]",[1,1],15)):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-422.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-422.png)

\>sequence("x[n-1]+x[n-2]",[1,1],15)^(1/(1:15))


    [1,  1,  1.25992,  1.31607,  1.37973,  1.41421,  1.44256,  1.46311,
    1.47967,  1.49292,  1.50389,  1.51309,  1.52091,  1.52765,  1.53352]

\>plot2d(sequence("x[n-1]+x[n-2]",[1,1],15)^(1/(1:15))):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-423.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-423.png)

## Menggunakan perintah "iterate" atau "niterate"

Dalam ilmu matematika, iterasi dapat diartikan sebagai proses atau
metode yang digunakan secara berulang-ulang (pengulangan) dalam
menyelesaikan permasalahan matematik.


EMT menyediakan fungsi iterate("g(x)", x0, n) untuk melakukan iterasi


$$x_{k+1}=g(x_k), \ x_0=x_0, k= 1, 2, 3, ..., n.$$Berikut contoh penggunaan iterasi


Menunjukkan pertumbuhan dari nilai awal 1000 dengan laju pertambahan
5%, selama 10 periode.


\>q=1.05; iterate("x\*q",1000,n=10)'


             1000 
             1050 
           1102.5 
          1157.63 
          1215.51 
          1276.28 
           1340.1 
           1407.1 
          1477.46 
          1551.33 
          1628.89 

## Spiral Theodorus

konstruksi segitiga siku-siku yang berkesinambungan menjadi spiral
atau dalam kata lain sebuah spiral yang dibangun dari segitiga
siku-siku yang berurutan. Setiap segitiga siku-siku yang baru dibuat
dengan menghubungkan sisi miring segitiga sebelumnya dengan sisi alas
yang panjangnya 1 satuan.


Spiral Theodorus (spiral segitiga siku-siku) dapat digambar secara
rekursif. Rumus rekursifnya adalah:


$$x_n = \left( 1 + \frac{i}{\sqrt{n-1}} \right) \, x_{n-1}, \quad x_1=1,$$yang menghasilkan barisan bilangan kompleks.


\>function g(n) := 1+I/sqrt(n)


Rekursinya dapat dijalankan sebanyak 17 untuk menghasilkan barisan 17
bilangan kompleks, kemudian digambar bilangan-bilangan kompleksnya.


\>x=sequence("g(n-1)\*x[n-1]",1,17); plot2d(x,r=3.5);...  
\>   textbox(latex("Spiral\\ Theodorus"),0.4):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-426.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-426.png)

Selanjutnya dihubungan titik 0 dengan titik-titik kompleks tersebut
menggunakan loop.


\>for i=1:cols(x); plot2d([0,x[i]],\>add); end:


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-427.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-427.png)

\>function gstep (v) ...


    w=[-v[2];v[1]];
    return v+w/norm(w);
    endfunction
</pre>
\>x=iterate("gstep",[1;0],16); plot2d(x[1],x[2],r=3.5,\>points):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-428.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-428.png)

## Limit Barisan

Limit barisan melambangkan nilai mutlak untuk bilangan riil dan nilai
modulus  untuk bilangan kompleks.


Definisi formal:


$$\forall \varepsilon > 0, \exists k \in \mathbb{N} : (\forall n \in \mathbb{N}, n \geq k \implies |x_n - L| <\varepsilon)$$Dapat dinotasikan sebagai


$$\lim_{n\to\infty}x_n=L$$Contoh:


1.


$$\lim_{n \to \infty}\frac{1}{n}$$\>$showev('limit(1/n,n,inf))


$$\lim_{n\rightarrow \infty }{\frac{1}{n}}=0$$2.


$$\lim_{n\to\infty}\frac{2n^2-1}{n^2+5}$$\>$showev('limit((2\*n^2-1)/(n^2+5),n,inf))


$$\lim_{n\rightarrow \infty }{\frac{2\,n^2-1}{n^2+5}}=2$$## Kekonvergenan

Iterasi sampai konvergen merupakan proses yang terus berulang sampai
mendapat nilai yang stabil atau tidak berubah secara signifikan.
Tetapi, apabila iterasinya tidak konvergen setelah ditunggu lama, Kita
dapat menghentikannya dengan menekan tombol [ESC].


\>iterate("cos(x)",1) // iterasi x(n+1)=cos(x(n)), dengan x(0)=1.


    0.739085133216

Iterasi tersebut konvergen ke penyelesaian persamaan


$$x = \cos(x).$$Iterasi ini juga dapat dilakukan pada interval, hasilnya adalah
barisan interval yang memuat akar tersebut.


\>hasil := iterate("cos(x)",~1,2~) //iterasi x(n+1)=cos(x(n)), dengan interval awal (1, 2)


    ~0.739085133211,0.7390851332133~

Jika interval hasil tersebut sedikit diperlebar, akan terlihat bahwa
interval tersebut memuat akar persamaan x=cos(x).


\>h=expand(hasil,100), cos(h) << h


    ~0.73908513309,0.73908513333~
    1

Iterasi juga dapat digunakan pada fungsi yang didefinisikan.


 Variable Iterasi not found!


\>function f(x) := (x+2/x)/2


Iterasi x(n+1)=f(x(n)) akan konvergen ke akar kuadrat 2.


\>iterate("f",2), sqrt(2)


    1.41421356237
    1.41421356237

## Deret Taylor

Deret Taylor suatu fungsi f yang diferensiabel sampai tak hingga di
sekitar x=a adalah:


$$f(x) = \sum_{k=0}^\infty \frac{(x-a)^k f^{(k)}(a)}{k!}.$$Diberikan contoh fungsi exponensial yang didekati dengan Deret Taylor


\>$'e^x =taylor(exp(x),x,0,10)


$$e^{x}=\frac{x^{10}}{3628800}+\frac{x^9}{362880}+\frac{x^8}{40320}+  \frac{x^7}{5040}+\frac{x^6}{720}+\frac{x^5}{120}+\frac{x^4}{24}+  \frac{x^3}{6}+\frac{x^2}{2}+x+1$$Menghitung exp(x) untuk x=4 yang di potong pada k=10


\>x := 4; k := 10; hasil := round(exp(x),k)


    54.5981500331

Bukti :


$$e^x = \frac{(x)^{10}}{(3628800)} + \frac{(x)^{9}}{(362880)} + \frac{(x)^{8}}{(40320)} + \frac{(x)^{7}}{(5040)} + \frac{(x)^{6}}{(720)} + \frac{(x)^{5}}{(120)} + \frac{(x)^{4}}{(24)} + \frac{(x)^{3}}{(6)} + \frac{(x)^{2}}{(2)} + x + 1$$untuk x=4


$$e^4 = \frac{(4)^{10}}{(3628800)} + \frac{(4)^{9}}{(362880)} + \frac{(4)^{8}}{(40320)} + \frac{(4)^{7}}{(5040)} + \frac{(4)^{6}}{(720)} + \frac{(4)^{5}}{(120)} + \frac{(4)^{4}}{(24)} + \frac{(4)^{3}}{(6)} + \frac{(4)^{2}}{(2)} + 4 + 1$$$$e^4 = \frac{(4)^{10}}{(3628800)} + \frac{(4)^{9}}{(362880)} + \frac{(4)^{8}}{(40320)} + \frac{(4)^{7}}{(5040)} + \frac{(4)^{6}}{(720)} + \frac{(4)^{5}}{(120)} + \frac{(4)^{4}}{(24)} + \frac{(4)^{3}}{(6)} + \frac{(4)^{2}}{(2)} + 5$$$$e^4 = 54,4431$$## Soal Latihan

1.Tentukan barisan bilangan dengan a=5, beda tiap sukunya 3, dan
rentang sampai 25 !


\>(5:3:25)


    [5,  8,  11,  14,  17,  20,  23]

2. Tentukan jumlah seluruh elemen dan jumlah kumulatif dari barisan
bilangan no 1 !


\>sum(5:3:25)


    98

\>cumsum(5:3:25)


    [5,  13,  24,  38,  55,  75,  98]

3. Hitunglah limit barisan dari


$$\lim_{x\to\infty}\sqrt{\frac{4x+1}{x}}$$\>$showev('limit((5\*x^2+1)/(x),x,inf))


$$\lim_{x\rightarrow \infty }{\frac{5\,x^2+1}{x}}=\infty $$4. Buatlah deret taylor log(x) di sekitar x=1 yang dipotong pada k=3


\>$'log(x)=taylor(log(x),x,1,3)


$$\log x=x+\frac{\left(x-1\right)^3}{3}-\frac{\left(x-1\right)^2}{2}-  1$$5. Buatlah barisan kompleks dengan X1=1 dan X2=2 sebanyak 10 suku


\>sequence("x[n-1]+x[n-2]",[1,2],10) //suku ke satu :1, suku ke dua :1


    [1,  2,  3,  5,  8,  13,  21,  34,  55,  89]

# 7. Fungsi Multivariabel

Fungsi multivariabel adalah sebuah konsep dalam matematika yang
menggambarkan hubungan antara satu variabel output dengan dua atau
lebih variabel input. Berbeda dengan fungsi satu variabel yang hanya
melibatkan satu variabel bebas, fungsi multivariabel melibatkan
beberapa variabel bebas yang secara bersama-sama menentukan nilai dari
variabel terikat. Fungsi multivariabel biasanya digunakan untuk
menggambarkan hubungan yang kompleks dalam bidang seperti fisika,
ekonomi, teknik, dan berbagai ilmu lainnya.


Secara umum, jika f adalah sebuah fungsi multivariabel, maka bentuk
umumnya dapat dinyatakan sebagai:


$$z=f(x_1,x_2,...,x_n)$$

dimana x1,x2,...,xn adalah variabel bebas (input) menunjukkan jumlah
variabel dan z adalah variable terikat (output).


contoh :


Luas Persegi Panjang: Luas persegi panjang (L) adalah fungsi dari
panjang (p) dan lebar (l). Kita dapat menuliskannya sebagai L(p, l) =
p * l. Di sini, L adalah variabel terikat, sedangkan p dan l adalah
variabel bebas.


Diberikan fungsi:


$$x^2+2xy+y^2$$\>function f(x,y) &= x^2 + 2\*x\*y + y^2


    
                                2            2
                               y  + 2 x y + x
    

diff(f,x): Bagian ini untuk menghitung turunan numerik.


f: Merupakan representasi dari fungsi yang ingin kita turunkan. Fungsi
ini bisa berupa fungsi anonim, fungsi yang telah didefinisikan
sebelumnya, atau bahkan persamaan matematika yang kompleks.


x: Menunjukkan variabel terhadap mana kita akan menurunan fungsi f.
Artinya, kita akan mencari laju perubahan fungsi f terhadap perubahan
nilai x.


&amp;=: mendefinikan fungsi, seperti yang sudah dijelaskan kemarin


\>fx &= diff(f(x,y),x)


    
                                  2 y + 2 x
    

ini merupakan fungsi simbolik jadi harus didefinisikan dengan &amp;=


\>fy &= diff(f(x,y),y)


    
                                  2 y + 2 x
    

\>plot3d("f", -2,2, -2,2) :


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-447.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-447.png)

menggunakan fungsi f yang telah didefinisikan di atas.


## Turunan fungsi multivariabel

Diberikan fungsi:


$$\sqrt{x}+y^2+2xz$$\>function f(x,y,z)&= sqrt(x)+y^2+2\*x\*z


    
                                      2
                             2 x z + y  + sqrt(x)
    

\>fx &= diff(f(x,y,z),x)


    
                                         1
                               2 z + ---------
                                     2 sqrt(x)
    

\>fy &= diff(f(x,y,z),y)


    
                                     2 y
    

\>fz &= diff(f(x,y,z),z)


    
                                     2 x
    

1. Diberikan fungsi


$$x^3+4y^2-3x+2$$\>function g(x,y) &= x^3+4\*y^2-3\*x+2


    
                                2    3
                             4 y  + x  - 3 x + 2
    

menentukan dg/dx


\>gx &= diff(g(x,y),x)


    
                                      2
                                   3 x  - 3
    

menentukan dg/dy


\>gy &= diff(g(x,y),y)


    
                                     8 y
    

\>grad &= [diff(g(x,y),x), diff(g(x,y),y)]


    
                                   2
                               [3 x  - 3, 8 y]
    

2. Contoh Trigonometri


Diberikan fungsi:


$$\frac{2sin(x)^2}{sin(x)+cos(x)}+tan(y)^3$$\>function f(x,y,z)&= 2\*sin(x)^2/(sin(x)+cos(z))+tan(y)^3


    
                                  2
                             2 sin (x)         3
                          --------------- + tan (y)
                          cos(z) + sin(x)
    

\>$fx := diff(f(x,y,z),x)


$$\frac{4\,\cos x\,\sin x}{\cos z+\sin x}-\frac{2\,\cos x\,\sin ^2x}{
 \left(\cos z+\sin x\right)^2}$$\>$fy := diff(f(x,y,z),y)


$$3\,\sec ^2y\,\tan ^2y$$\>$fz := diff(f(x,y,z),z)


$$\frac{2\,\sin ^2x\,\sin z}{\left(\cos z+\sin x\right)^2}$$## Grafik

Grafik fungsi multivariabel adalah representasi visual dari fungsi
yang memiliki dua atau lebih variabel input. Untuk fungsi dua variabel
$f(x,y)$, grafiknya berupa permukaan dalam ruang tiga dimensi.


Bidang z = 2x + 3y


\>plot3d("2\*x + 3\*y", -2,2, -2,2):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-454.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-454.png)

\>title("Kontur z = 2x + 3y"):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-455.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-455.png)

Paraboloid 


\>plot3d("x^2 + y^2", -8,2, -8,2):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-456.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-456.png)

Hyperbolic Paraboloid


\>plot3d("x^2 - y^2", -2,2, -2,2):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-457.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-457.png)

\>plot3d("sin(x)\*cos(y)", -pi,pi, -pi,pi):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-458.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-458.png)

\>plot3d("sin(sqrt(x^2 + y^2))", -4\*pi,4\*pi, -4\*pi,4\*pi):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-459.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-459.png)

\>plot3d("sin(x)\*sin(y)", -pi,pi, -pi,pi):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-460.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-460.png)

\>plot3d("exp(-x^2-y^2)", -2,2, -2,2):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-461.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-461.png)

Distribusi normal bivariat


\>plot3d("(1/(2\*pi))\*exp(-(x^2+y^2)/2)", 1,3, 1,3)

\>title("Distribusi Normal Bivariat"):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-462.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-462.png)

Potensial elektrostatik


\>plot3d("1/sqrt(x^2+y^2+1)", -1,3, -1,3)

\>title("Potensial Elektrostatik"):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-463.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-463.png)

## Turunan 

Turunan fungsi multivariabel merupakan perluasan konsep turunan dari
fungsi satu variabel ke fungsi dengan dua atau lebih variabel.


menghitung turunan parsial


\>f &= x^4 + 6\*x\*y + y^3


    
                                3            4
                               y  + 6 x y + x
    

\>plot3d("x^4 + 6\*x\*y + y^3", -5.2, -5.2):


![images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-464.png](images/Aplikom#Kalkulus_Sabilla%20Hanifah%20Nur%20Jihada_23030630012-464.png)

\>f &= x^2 + y^2


    
                                    2    2
                                   y  + x
    

\>grad &= [diff(f,x), diff(f,y)]


    
                                  [2 x, 2 y]
    

Turunan berarah dalam arah u=(1/v2, 1/v2)


\>Dir &= grad[1]/sqrt(2) + grad[2]/sqrt(2)


    
                            sqrt(2) y + sqrt(2) x
    

Menghitung turunan parsial kedua


\>f &= x^7 + 3\*x\*y + y^4


    
                                4            7
                               y  + 3 x y + x
    

\>fxy &= diff(diff(f,x),y)


    
                                      3
    

## Integral 

Integral fungsi multivariabel adalah perluasan konsep integral dari
fungsi satu variabel ke fungsi dengan dua atau lebih variabel.


Contoh sederhana integral lipat dua


\>$showev ('integrate(integrate(x^2 + y^2, x, 0, 1), y, 0, 2))


$$\frac{\int_{0}^{2}{3\,y^2+1\;dy}}{3}=\frac{10}{3}$$ Hasil dari integral ganda ini akan memberikan nilai total area di  

bawah permukaan fungsi


$$f(x,y)=x^2+y^2$$

di daerah persegi yang ditentukan.


\>$showev('integrate(integrate(3\*x^2\*y - 2\*x\*y^2, x, 0, 1), y, 1, 2))


$$\int_{1}^{2}{y-y^2\;dy}=-\frac{5}{6}$$Contoh ini menunjukkan bagaimana integral ganda bekerja pada fungsi
multivariabel.


1. Integral Ganda Fungsi Eksponensial


\>$showev('integrate(integrate(exp(x) \* exp(y), x, 0, 1), y, 0, 2))


$$\int_{0}^{2}{e^{y+1}-e^{y}\;dy}=e^3-e^2-e+1$$2. Integral Ganda Fungsi Trigonometri


\>$showev('integrate(integrate(sin(x) \* cos(y), x, 0, pi), y, 0, pi/2))


$$2\,\int_{0}^{\frac{\pi}{2}}{\cos y\;dy}=2$$3. Integral Ganda Fungsi Kuadrat


\>$showev('integrate(integrate(x^2 + y^2, x, 0, 2), y, 1, 3))


$$\frac{\int_{1}^{3}{6\,y^2+8\;dy}}{3}=\frac{68}{3}$$4. Integral Ganda Fungsi Campuran


\>$showev('integrate(integrate(x \* y^2 - 3\*x\*y, x, 0, 2), y, 1, 2))


$$\int_{1}^{2}{2\,y^2-6\,y\;dy}=-\frac{13}{3}$$5. Integral Ganda Fungsi Logaritma


\>$showev('integrate(integrate(log(x+1) + log(y+1), x, 0, 1), y, 0, 2))


$$\int_{0}^{2}{\log \left(y+1\right)+2\,\log 2-1\;dy}=3\,\log 3+4\,  \log 2-4$$## Aplikasi Fungsi Multivariabel

1. Misalkan medan listrik di suatu daerah diberikan oleh


$$E(x,y)=x^2 - y$$

Hitung fluks medan listrik melalui permukaan persegi panjang
[0,1]×[0,2]!


\>$showev('integrate(integrate(x^2 - y, x, 0, 1), y, 0, 2))


$$-\frac{\int_{0}^{2}{3\,y-1\;dy}}{3}=-\frac{4}{3}$$