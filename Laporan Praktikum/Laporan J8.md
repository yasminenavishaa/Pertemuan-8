# LAPORAN JOBSHEET 8 PRAKTIKUM STRUKTUR DATA

Dibuat oleh : <p>
Yasmine Navisha Andhani <p>
1F D4 Teknik Informatika <p>
2141720047 <p>

# 7.2 Praktikum 1
## 7.2.1 Langkah - langkah Percobaan
1. Perhatikan Diagram Class Pakaian berikut ini: <p>
<img src="J8 - 7.2.1 (1).PNG"> <p>
Berdasarkan diagram class tersebut, akan dibuat program class pakaian dalam java.
2. Buat package dengan nama Praktikum1, kemudian buat class baru dengan nama Pakaian.
3. Tambahkan atribut-atribut Pakaian seperti pada Class Diagram Pakaian, kemudian tambahkan pula konstruktornya seperti gambar berikut ini. <p>
<img src="J8 - 7.2.1 (3).PNG"> <p>
4. Setelah membuat class Pakaian, selanjutnya perlu dibuat class Stack yang berisi atribut dan method sesuai diagram Class Stack berikut ini: <P>
<img src="J8 - 7.2.1 (4).PNG"> <p>
Keterangan: Tipe data pada variabell data menyesuaikan dengan data yang akan akan disimpan di dalam Stack. Pada praktikum ini, data yang akan disimpan merupakan array of object dari Pakaian, sehingga tipe data yang digunakan adalah Pakaian.
5. Buat class baru dengan nama Stack. Kemudian tambahkan atribut dan konstruktor seperti gambar berikut ini.
<img src="J8 - 7.2.1 (5).PNG"> <p>
6. Buat method IsEmpty bertipe boolean yang digunakan untuk mengecek apakah stack kosong. <p>
<img src="J8 - 7.2.1 (6).PNG"> <p>
7. Buat method IsFull bertipe boolean yang digunakan untuk mengecek apakah stack sudah terisi penuh. <p>
<img src="J8 - 7.2.1 (7).PNG"> <p>
8. Buat method push bertipe void untuk menambahkan isi elemen stack dengan parameter pkn yang berupa object Pakaian <p>
<img src="J8 - 7.2.1 (8).PNG"> <p>
9. Buat method Pop bertipe void untuk mengeluarkan isi elemen stack. Karena satu elemen stack terdiri dari beberapa informasi (jenis, warna, merk, ukuran, dan harga), maka ketika mencetak data juga perlu ditampilkan semua informasi tersebut <p>
<img src="J8 - 7.2.1 (9).PNG"> <p>
10. Buat method peek bertipe void untuk memeriksa elemen stack pada posisi paling atas.<p>
<img src="J8 - 7.2.1 (10).PNG"> <p>
11. Buat method print bertipe void untuk menampilkan seluruh elemen pada stack. <p>
<img src="J8 - 7.2.1 (11).PNG"> <p>
12. Buat method clear bertipe void untuk menghapus seluruh isi stack. <p>
<img src="J8 - 7.2.1 (12).PNG"> <p>
13. Selanjutnya, buat class baru dengan nama StackMain. Buat fungsi main, kemudian lakukan instansiasi objek dari class Stack dengan nama stk dan nilai parameternya adalah 5. <p>
<img src="J8 - 7.2.1 (13).PNG"> <p>
14. Deklarasikan Scanner dengan nama sc
15. Tambahkan kode berikut ini untuk menerima input data Pakaian, kemudian semua informasi tersebut dimasukkan ke dalam stack <p>
<img src="J8 - 7.2.1 (15).PNG"> <p>
Catatan: sintaks sc.nextLine() sebelum sintaks st.push(p) digunakan untuk mengabaikan karakter new line
16. Lakukan pemanggilan method print, method pop, dan method peek dengan urutan sebagai berikut. <p>
<img src="J8 - 7.2.1 (16).PNG"> <p>
17. Compile dan jalankan class StackMain, kemudian amati hasilnya. <p>

## 7.2.2 Verifikasi Hasil Percobaan
<img src="J8 - 7.2.2.PNG"> <p>

## 7.2.3 Pertanyaan
1. Berapa banyak data pakaian yang dapat ditampung di dalam stack? Tunjukkan potongan kode program untuk mendukung jawaban Anda tersebut!
> : Ada 5 data
```java
Stack stk = new Stack(5);
```

2. Perhatikan class StackMain, pada saat memanggil fungsi push, parameter yang dikirimkan adalah p. Data apa yang tersimpan pada variabel p tersebut? <p>
<img src="J8 - 7.2.3 (2).PNG"> <p>
> : data yang dimasukkan melalu scanner

3. Apakah fungsi penggunaan do-while yang terdapat pada class StackMain?
> :  Di gunakan untuk melakukan perulangan untuk menginput atribut yang ada, dan akan terus melakukan perulangan selama while kondisi "y" dan akan berhenti jika tampungan sudah penuh atau ketika while tidak sama dengan "y".

4. Modifikasi kode program pada class StackMain sehingga pengguna dapat memilih operasi - operasi pada stack (push, pop, peek, atau print) melalui pilihan menu program dengan memanfaatkan kondisi IF-ELSE atau SWITCH-CASE! <p>
> : <img src="J8 - 7.2.3 (4).PNG"> <p>

# 7.3 Praktikum 2
## 7.3.1 Langkah - langkah Percobaan
1. Perhatikan Diagram Class berikut ini :
Berdasarkan diagram class tersebut, akan dibuat program class Postfix dalam Java.
2. Buat package dengan nama Praktikum2, kemudian buat class baru dengan nama Postfix. Tambahkan atribut n, top, dan stack sesuai diagram class Postfix tersebut.
3. Tambahkan pula konstruktor berparameter seperti gambar berikut ini.
4. Buat method push dan pop bertipe void.
5. Buat method IsOperand dengan tipe boolean yang digunakan untuk mengecek apakah elemen data berupa operand.
6. Buat method IsOperator dengan tipe boolean yang digunakan untuk mengecek apakah elemen data berupa operator.
7. Buat method derajat yang mempunyai nilai kembalian integer untuk menentukan derajat operator.
8. Buat method konversi untuk melakukan konversi notasi infix menjadi notasi postfix dengan cara mengecek satu persatu elemen data pada String Q sebagai parameter masukan.
9. Selanjutnya, buat class baru dengan nama PostfixMain tetap pada package Praktikum2. Buat class main, kemudian buat variabel P dan Q. Variabel P digunakan untuk menyimpan hasil akhir notasi postfix setelah dikonversi, sedangkan variabel Q digunakan untuk menyimpan masukan dari pengguna berupa ekspresi matematika dengan notasi infix. Deklarasikan variabel Scanner 
dengan nama sc, kemudian panggil fungsi built-in trim yang digunakan untuk menghapus adanya spasi di depan atau di belakang teks dari teks persamaan yang dimasukkan oleh pengguna.
Penambahan string “)” digunakan untuk memastikan semua simbol/karakter yang masih berada di stack setelah semua persamaan terbaca, akan dikeluarkan dan dipindahkan ke postfix.
10. Buat variabel total untuk menghitung banyaknya karaketer pada variabel Q.
11. Lakukan instansiasi objek dengan nama post dan nilai parameternya adalah total. Kemudian panggil method konversi untuk melakukan konversi notasi infix Q menjadi notasi postfix P.
12. Compile dan jalankan class PostfixMain dan amati hasilnya.
```java
public class Postfix {
    
    int n;
    int top;
    char stack[];

    public Postfix(int total) {
        n = total;
        top = -1;
        stack = new char[n];
        push('(');
    }

    public void push(char c) {
        top++;
        stack[top] = c;
    }

    public char pop() {
        char item = stack[top];
        top--;
        return item;
    }

    public boolean isOperand(char c) {
        if ((c >= 'A' && c <= 'Z') || (c >= 'a' && c <= 'z') || (c >= '0' && c <= '9') || c == ' ' || c == '.') {

            return true;
        } else {
            return false;
        }
    }

    public boolean isOperator(char c) {
        if (c == '^' || c == '%' || c == '/' || c == '*' || c == '-' || c == '+') {
            return true;
        } else {
            return false;
        }
}

    public String konversi(String q) {
        return null;
    }
}
```
```java
import java.util.Scanner;

public class PostfixMain {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String P, Q;
        System.out.println("Masukkan ekspresi matematika (infix): ");
        Q = sc.nextLine();
        Q = Q.trim();
        Q = Q + ")";

        int total = Q.length();

        Postfix post = new Postfix(total);
        P = post.konversi(Q);
        System.out.println("Postfix: " + P);
        sc.close();
    }
}
```

## 7.3.2 Verfikasi Hasil Percobaan
 <img src="J8 - 7.3.2.PNG"> <p>

## 7.3.3 Pertanyaan
1. Perhatikan class Postfix, jelaskan alur kerja method derajat!
> : saat '^' maka akan mereturn nilai 3, jika operator '%', '*' maka akan mereturn nilai 2. sedangkan '-', dan '+' akan mereturn nilai 1 menggunakan switch case.
2. Apa fungsi kode program berikut?
<img src="J8 - 7.3.2.PNG"> <p>
> : untuk menyimpan data char (i) kedalam Q dengan menggunakan charAt(i)
3. Jalankan kembali program tersebut, masukkan ekspresi 3*5^(8-6)%3. Tampilkan hasilnya!
> : <img src="J8 - 7.3.3 (3).PNG"> <p>
4. Pada soal nomor 3, mengapa tanda kurung tidak ditampilkan pada hasil konversi? Jelaskan!
> : karena apabila terdapat tanda kurung pada ekspresi matematika, maka tanda tersebut akan langsung meng-pop tanpa harus kedalam postfix.

# 7.4 Tugas
1. Perhatikan dan gunakan kembali kode program pada Praktikum 1. Tambahkan method getMin pada class Stack yang digunakan untuk mencari dan menampilkan data pakaian dengan harga terendah dari semua data pakaian yang tersimpan di dalam stack!
```java
public class Stack {
    int size;
    int top;
    Pakaian data[];

    public Stack1(int size){
        this.size = size;
        data = new Pakaian[size];
        top = -1;
    }

    public boolean IsEmpty(){
        if (top == -1) {
            return true;
        } else {
            return false;
        } 
    }

    public boolean IsFull() {
        if (top == size -1) {
            return true;
        } else {
            return false;
        }
    }

    public void push (Pakaian pkn) {
        if (!IsFull()) {
            top++;
            data[top] = pkn;
        } else {
            System.out.println("Isi stack penuh!");
        }
    }

    public void pop() {
        if (!IsEmpty()) {
            Pakaian x = data[top];
            top--;
            System.out.println("Data yang keluar: " + x.jenis + " " + x.warna + " " + x.merk + " " + x.ukuran + " " + x.harga);
        } else {
            System.out.println("Stack masih kosong");
        }
    }

    public void peek() {
        System.out.println("Elemen teratas: " + data[top].jenis + " " + data[top].warna + " " + data[top].merk + " " + data[top].merk + " " + data[top].ukuran + " " + data[top].harga);
    }

    public void print() {
        System.out.println("Isi stack: ");
        for (int i = top; i >= 0; i--) {
            System.out.println(data[i].jenis + " " + data[i].warna + " " + data[i].merk + " " + data[i].merk + " " + data[i].ukuran + " " + data[i].harga + " ");
        }
        System.out.println("");
    }

    public void Clear() {
        if(!IsEmpty()) {
            for (int i = top; i >= 0; i--) {
                top--;
            }
            System.out.println("Stack sudah dikosongkan");
        }else {
            System.out.println(" Stack masih kosong");
        }
    }
    
    public void getMin() {
        double min = data[0].harga;
        int posisi = 0;
        for (int i = top; i >= 0; i--) {
            if (data[i].harga < min){
                min = data[i].harga;
                posisi = i;
            }
        }
        System.out.println(data[posisi].jenis + " " + data[posisi].warna + " " + data[posisi].merk + " " + data[posisi].merk + " " + data[posisi].ukuran + " " + data[posisi].harga + " ");

    }
}
```
```java
import java.util.Scanner;

public class StackMain {
    public static void main(String[] args) {
        Stack stk = new Stack(5);
        Scanner sc = new Scanner(System.in);

        char opsi;
        char pilih;

        do {
            System.out.println("+---------------------------+");
            System.out.println("1. Melakukan push");
            System.out.println("2. Melakukan pop");
            System.out.println("3. Melakukan peek");
            System.out.println("4. Melakukan print");
            System.out.println("5. Mencari yang murah");
            System.out.println("6. Keluar");
            System.out.print("Silahkan pilih opsi : ");
            opsi = sc.next().charAt(0);
            sc.nextLine();
            System.out.println("+---------------------------+");
            switch(opsi){
                case '1':
                do {
                System.out.println("Menu Push");
                System.out.println("________________");
                    System.out.print("Jenis: ");
                    String jenis = sc.nextLine();
                    System.out.print("Warna: ");
                    String warna = sc.nextLine();
                    System.out.print("Merk: ");
                    String merk = sc.nextLine();
                    System.out.print("Ukuran: ");
                    String ukuran = sc.nextLine();
                    System.out.print("Harga: ");
                    double harga = sc.nextDouble();
                    Pakaian p = new Pakaian(jenis, warna, merk, ukuran, harga);
                    System.out.print("Apakah Anda akan menambahkan data baru ke stack (y/n)? ");
                    pilih = sc.next().charAt(0);
                    sc.nextLine();
                    stk.push(p);
                } while (pilih == 'y');
                break;
    
                case '2':
                System.out.println("________________");
                System.out.println("Menu Pop");
                System.out.println("________________");
                stk.pop();
                break;
    
                case '3':
                System.out.println("________________");
                System.out.println("Menu Peek");
                System.out.println("________________");
                stk.peek();
                break;
    
                case '4':
                System.out.println("________________");
                System.out.println("Menu Print");
                System.out.println("________________");
                stk.print();
                break;

                case '5':
                System.out.println("________________");
                System.out.println("Harga Termurah adalah");
                stk.getMin();
                break;

                case '6':
                System.out.println("________________");
                System.out.println("Terimakasih sudah menggunakan program kami");
                break;

                default:
                System.out.println("________________");
                System.out.println("Inputan anda salah");
                System.out.println("________________");
                break;
            }

        } while (opsi!='6');
    }
}
```
Output
<img src="J8 - t1a.PNG"> <p>
<img src="J8 - t1b.PNG"> <p>

2. Setiap hari Minggu, Dewi pergi berbelanja ke salah satu supermarket yang berada di area rumahnya. Setiap kali selesai berbelanja, Dewi menyimpan struk belanjaannya di dalam laci. Setelah dua bulan, ternyata Dewi sudah mempunyai delapan struk belanja. Dewi berencana mengambil lima struk belanja untuk ditukarkan dengan voucher belanja.Buat sebuah program stack untuk menyimpan data struk belanja Dewi, kemudian lakukan juga proses pengambilan data struk belanja sesuai dengan jumlah struk yang akan ditukarkan dengan voucher. Informasi yang tersimpan pada struk belanja terdiri dari:
 Nomor transaksi
 Tanggal pembelian
 Jumlah barang yang dibeli
 Total harga bayar
Tampilkan informasi struk belanja yang masih tersimpan di dalam stack
```java
public class StrukBelanja {
    String tanggal, namaBarang;
    int noTransaksi, jmlh, total;

    StrukBelanja(int nt, String tgl, String nb, int j, int t){
    noTransaksi =nt;
    tanggal =tgl;
    namaBarang =nb;
    jmlh =j;
    total =t;
    }
}
```
```java
public class Belanja {
    int size;
    int top;
    StrukBelanja data[];

    public Belanja(int size){
        this.size = size;
        data = new StrukBelanja[size];
        top = -1;
    }
    public boolean IsEmpty(){
        if(top == -1){
            return true;
        }else{
            return false;
        }
    }
    public boolean IsFull(){
        if(top == size - 1){
            return true;
        }else{
            return false;
        }
    }

    public void push(StrukBelanja sb){
        if(!IsFull()){
            top++;
            data[top] = sb;
        }else{
            System.out.println("Isi stack penuh!");
        }
    }
    public void pop(){
        if(!IsEmpty()){
            StrukBelanja x = data[top];
            top--;
            System.out.println("Data yang keluar: " + x.noTransaksi + " " + x.tanggal + " " + x.namaBarang + " " + x.jmlh + " " + x.total);
        }else{
            System.out.println("Stock masih kosong");
        }
    }
    public void peek(){
        System.out.println("Elemen teratas: " + data[top].noTransaksi +"."+ " " + data[top].tanggal + " " + data[top].namaBarang + " " + data[top].jmlh + " " + data[top].total);
    }
    public void print(){
        System.out.println("Isi stack: ");
        for(int i = top; i >= 0; i--){
            System.out.println(data[i].noTransaksi + " " + data[i].tanggal + " " + data[i].namaBarang + " " + data[i].jmlh + " " + data[i].total);
        }
        System.out.println("");
    }
    public void clear(){
        if(!IsEmpty()){
            for(int i = top; i >= 0; i--){
                top--;
            }
            System.out.println("Stock sudah dikosongkan");
        }else{
            System.out.println("Stock masih kosong");
        }
    }
}
```
```java
public static void main(String[] args) {
    Scanner sc =new Scanner(System.in);
    Scanner sd =new Scanner(System.in);

    System.out.println("----------------------------------");
    System.out.println("          Struk Belanja           ");
    System.out.println("----------------------------------");
    System.out.println();
    System.out.print("Masukkan Banyak Struk\t: ");
    int banyak = sc.nextInt();
    System.out.println();
    belanja blj = new belanja(banyak);

    int totalHarga = 0;
    int jml, harga;
    for (int i = 0; i < banyak; i++) {
    System.out.print("Nomor Transaksi\t\t: ");
    int nt =sc.nextInt();
    System.out.print("Tanggal Pembelian\t: ");
    String tanggal =sd.nextLine();
    System.out.print("Nama Barang\t\t: ");
    String nb =sd.nextLine();
    System.out.print("Jumlah Barang\t\t: ");
    jml = sc.nextInt();
    System.out.print("Harga Barang\t\t: ");
    harga = sc.nextInt();
    totalHarga =jml * harga;
    strukBelanja sb =new strukBelanja(nt, tanggal, nb, jml,harga);
    blj.push(sb);
    System.out.print("Total Harga\t\t: "+ totalHarga);
    System.out.println("\n");
    }

char pilih;
do{
    System.out.println("------------------------------------");
    System.out.println("             PILIHAN MENU           ");
    System.out.println("------------------------------------");
    System.out.println(" 1. menampilkan struk teratas\n 2. ambil 5 struk untuk mendapatkan kupon\n 3. lihat sisa struk\n 4. keluar\n");
    
    System.out.print("Pilih Menu (masukkan angka 1-4)");
    int pilihan =sc.nextInt();
    System.out.println("------------------------------------------------");

    switch (pilihan){
        case 1:
            blj.peek();
            blj.print();
            break;
        case 2:
            blj.pop();
            blj.pop();
            blj.pop();
            blj.pop();
            blj.pop();
            break;
        case 3:
            blj.print();
            break;
        case 4:
            System.out.println("Terima Kasih");
            break;
        default:
            System.out.println("Menu yang anda masukkan salah");
            break;
    }if(pilihan == 4) {
        pilih = 't';
    }else{
        System.out.print("Kembali ke menu Utama (y/t) : ");
        pilih = sc.next().charAt(0);
    }
}while(pilih == 'y');
}
}
```