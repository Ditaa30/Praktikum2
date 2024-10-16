# Praktikum2

# 1. Class Person
    public class Person {
        private String nama;
        private String jenisKelamin;
        private int umur;
    
Penjelasan :
public class Person: Mendeklarasikan class Person. Class ini merupakan blueprint atau cetakan untuk objek-objek Person yang akan dibuat. Atribu dengan private :
- private String nama, private String jenisKelamin, dan private int umur adalah atribut/field milik class Person.
- private berarti atribut hanya bisa diakses dari dalam class itu sendiri.

## Setter dan Getter untuk atribut 'nama'
    public void setNama(String nama) {
        this.nama = nama;
    }

    public String getNama() {
        return nama;
    }

Penjelasan : 
- setNama: Adalah setter untuk atribut nama. Method ini menerima parameter bertipe String dan mengisi nilai ke atribut nama milik objek dengan menggunakan keyword this. **this.nama** = nama;: this merujuk ke atribut nama dalam objek yang sedang diproses.
- getNama: Adalah getter yang mengembalikan nilai dari atribut nama.

## Setter dan Getter untuk atribut 'jenisKelamin'
    public void setJenisKelamin(String jenisKelamin) {
        this.jenisKelamin = jenisKelamin;
    }

    public String getJenisKelamin() {
        return jenisKelamin;
    }

Penjelasan : 
- setJenisKelamin: Mengisi nilai atribut jenisKelamin melalui parameter.
- getJenisKelamin: Mengembalikan nilai dari atribut jenisKelamin.

## Setter dan Getter untuk atribut 'umur'
    public void setUmur(int umur) {
        this.umur = umur;
    }

        public int getUmur() {
        return umur;
        }
    }

Penjelasan : 
- setUmur: Mengisi nilai umur dengan menggunakan parameter bertipe int.
- getUmur: Mengembalikan nilai dari atribut umur.

# 2. Class 'Main' dan pembuatan objek
    public class Main {
        public static void main(String[] args) {
            Person anton = new Person();
            Person riko = new Person();

Penjelasan :
- public class Main: Mendeklarasikan class Main sebagai entry point program.
- public static void main(String[] args): Method main adalah tempat eksekusi program dimulai.
- anton dan riko: Membuat **dua objek** dari class Person.
- new Person(): Menggunakan keyword new untuk membuat objek baru.

## Mengisi atribut objek dengan 'Setter'
    anton.setNama("Anton");
    anton.setJenisKelamin("Laki-laki");
    anton.setUmur(25);

    riko.setNama("Riko");
    riko.setJenisKelamin("Laki-laki");
    riko.setUmur(30);

Penjelasan :
Method **setter** digunakan untuk **mengisi nilai** atribut setiap objek.
- anton.setNama("Anton"): Mengisi nama objek anton dengan "Anton".
- anton.setJenisKelamin("Laki-laki"): Mengisi jenis kelamin anton.
- anton.setUmur(25): Mengisi umur anton.
- Hal yang sama dilakukan untuk objek riko.

## Menampilkan data dengan 'Getter'
            System.out.println("Data Anton:");
            System.out.println("Nama: " + anton.getNama());
            System.out.println("Jenis Kelamin: " + anton.getJenisKelamin());
            System.out.println("Umur: " + anton.getUmur());
        
            System.out.println("\nData Riko:");
            System.out.println("Nama: " + riko.getNama());
            System.out.println("Jenis Kelamin: " + riko.getJenisKelamin());
            System.out.println("Umur: " + riko.getUmur());
        }    
    }

penjelasan :
- System.out.println() digunakan untuk **menampilkan informasi** ke layar.
- **Getter** dipanggil untuk **mengambil nilai** dari atribut objek.
    - anton.getNama() mengembalikan "Anton".
    - anton.getUmur() mengembalikan 25.
- Baris kosong (\n) digunakan untuk membuat jeda antara output Anton dan Riko.

# Output Program
![Output](https://github.com/user-attachments/assets/459e476c-ce0b-4298-8f8f-2b5a5141fef7)
