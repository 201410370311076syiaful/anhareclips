# anhareclips
syaifulnetbeans tools for anhar063
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package tb;
import java.util.Scanner;

public class KondisiRuangKelas {
    private int panjang;
    private int lebar;
    private int luas;
    private int jumlahkursi;
    private int rasio;
    private int pintu;
    private int jendela;

    public int getPanjang() {
        return panjang;
    }

    public void setPanjang(int panjang) {
        this.panjang = panjang;
    }

    public int getLebar() {
        return lebar;
    }

    public void setLebar(int lebar) {
        this.lebar = lebar;
    }

    public int getLuas() {
        return luas;
    }

    public void setLuas(int luas) {
        this.luas = luas;
    }

    public int getJumlahkursi() {
        return jumlahkursi;
    }

    public void setJumlahkursi(int jumlahkursi) {
        this.jumlahkursi = jumlahkursi;
    }

    public int getRasio() {
        return rasio;
    }

    public void setRasio(int rasio) {
        this.rasio = rasio;
    }

    public int getPintu() {
        return pintu;
    }

    public void setPintu(int pintu) {
        this.pintu = pintu;
    }

    public int getJendela() {
        return jendela;
    }

    public void setJendela(int jendela) {
        this.jendela = jendela;
    }
        
    Scanner scan=new Scanner(System.in);
    
    public void Luas(){
        System.out.println("\n\n==KONDISI RUANG KELAS==\n\n");
        
        System.out.println("Masukkan Panjang Kelas: ");
        setPanjang(scan.nextInt());
        System.out.println("Masukkan Lebar Kelas: ");
        setLebar(scan.nextInt());
        setLuas(getPanjang()*getLebar());
        
        System.out.println("Luas Kelas= "+getLuas());
        if(getPanjang()==getLebar()){
            System.out.println("Bentuk Ruang Persegi");
        }
        else
            if(getPanjang()!=getLebar())
        {System.out.println("Bentuk Ruang Persegi Panjang");
        }
              

}
    public void Rasio(){
         System.out.println("Masukkan Jumlah Kursi: ");
         setJumlahkursi(scan.nextInt());
                setRasio(getLuas()/getJumlahkursi());
                if(getRasio() >= 0.5){
                    System.out.println("Rasio Sesuai");
                }
                else
                    System.out.println("Rasio Tidak Sesuai");
        
                
    }
    public void pintujendela(){
        System.out.println("Masukkan Jumlah Pintu: ");
        setPintu(scan.nextInt());
        System.out.println("Masukkan Jumlah Jendela: ");
        setJendela(scan.nextInt());
        if(getPintu()>=2 && getJendela()>=1){
            System.out.println("Sesuai");
            
        }
        else {
            System.out.println("Tidak Sesuai");
        }
                
    }
    
    public void OutRuangan(){
        System.out.println("==KONDISI RUANG KELAS==");
        System.out.println("Panjang Ruang="+getPanjang());
        System.out.println("Lebar Ruang="+getLebar());
        
        System.out.println("Luas="+getLuas());
        if(getPanjang()==getLebar()){
            System.out.println("Bentuk Ruang Persegi");
        }
        else
            if(getPanjang()!=getLebar())
        {System.out.println("Bentuk Ruang Persegi Panjang");
        }
        System.out.print("Jumlah Kursi="+getJumlahkursi());
        if(getRasio() >= 0.5){
                    System.out.println("/Rasio Sesuai");
                }
                else
                    System.out.println("Rasio Tidak Sesuai");
       System.out.print("Jumlah Pintu="+getPintu());
       System.out.print("Jumlah Jendela="+getJendela());
       if(getPintu()>=2 && getJendela()>=1){
            System.out.println("/Sesuai");
            
        }
        else {
            System.out.println("/Tidak Sesuai");
        }
       
       
        
        
        
        
    }
    
}

