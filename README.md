# LatihanUKLSoalSulitNo1-Jasmine-Salsabila-F.-W.-XRPL2-
Fungsi dari program ini adalah untuk mengetahui rekap rata-rata nilai siswa. Lalu cara kerjanya adalah dengan cara menginputkan jumlah siswa dan total nilai masing-masing siswa oleh user.

Berikut adalah kode programnya:
    
    import java util.Scanner;
    public class SoalSulitNo1 {
    
    public static void main(String[] args) {
        Scanner inputan = new Scanner(System.in);

        System.out.println("Masukkan Jumlah Siswa: ");
        int jumlahSiswa = inputan.nextInt();
        double totalNilai = 0;

        for (int i = 1; i <= jumlahSiswa; i++) {
            System.out.println("Masukkan Nilai Siswa ke-"+ i +": ");
            double nilaiSiswa = inputan.nextDouble();
            totalNilai += nilaiSiswa;
        }

        double rataRataNilai = totalNilai / jumlahSiswa;

        System.out.println("HASIL REKAP NILAI SISWA");
        System.out.println("Jumlah Siswa = "+ jumlahSiswa);
        System.out.println("Total Nilai Siswa = "+ totalNilai);
        System.out.println("Rata-rata Nilai Siswa = "+ rataRataNilai);

        inputan.close();
        }
    }
