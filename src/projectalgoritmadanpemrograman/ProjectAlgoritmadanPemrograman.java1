package projectalgoritmadanpemrograman;

import java.util.Scanner;

public class ProjectAlgoritmadanPemrograman {
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner inputdata = new Scanner(System.in);
        String[] kodeBarang = {"A", "B", "C"};
        String[] namaBarang = {"LEVIS", "LEA", "LEE"};
        int[] hargaSatuan = {500000, 400000, 300000};
        
        System.out.print("Enter Kode Barang (A, B, C): ");
        String kode = inputdata.nextLine().toUpperCase();

        System.out.print("Enter Quantity: ");
        int quantity = inputdata.nextInt();
        
        String namaBarangSelected = "";
        int hargaSatuanSelected = 0;
        boolean valid = false;
        
        for (int i = 0; i < kodeBarang.length; i++) {
            if (kodeBarang[i].equals(kode)) {
                namaBarangSelected = namaBarang[i];
                hargaSatuanSelected = hargaSatuan[i];
                valid = true;
                break;
            }
        }
        if (!valid) {
            System.out.println("Invalid Kode Barang!");
            return;
        }
        int totalHarga = hargaSatuanSelected * quantity;
            double discount = 0;
            
        if (totalHarga > 2000000) {
            discount = 0.10 * totalHarga; // 10% discount
        } 
        else if (totalHarga >= 1500000) {
            discount = 0.05 * totalHarga; // 5% discount
        }
            double jumlahBayar = totalHarga - discount;
            
        System.out.println("Nama Barang: " + namaBarangSelected);
        System.out.println("Harga Satuan: Rp." + hargaSatuanSelected);
        System.out.println("Total Harga: Rp." + totalHarga);
        System.out.println("Discount: Rp." + discount);
        System.out.println("Jumlah Bayar: Rp." + jumlahBayar);
        
        }
}