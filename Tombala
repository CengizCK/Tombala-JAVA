package tombala;

import java.util.Random;
import java.util.Scanner;

public class Tombala {
    public static void main(String[] args) {
        Random r=new Random();
        Scanner input=new Scanner (System.in);
        System.out.println("Made by CK");
        System.out.println("--------------------------------");
        System.out.println("Kaç oyuncu ile oynuyorsunuz:");
        int oyuncusayisi=input.nextInt();
        //diziler
        String[] isimler=new String[oyuncusayisi];
        int[][]sayi=new int[oyuncusayisi][15];
        for (int i = 0; i <oyuncusayisi; i++) {
            System.out.println((i+1)+" ci oyuncunun ismini giriniz:");
            isimler[i]=input.next();
            for (int j = 0; j < 15; j++) {
                do{
                System.out.println(isimler[i]+" isimli oyuncu "+(j+1)+" inci sayısını giriyor (1-49) arası.");
                sayi[i][j]=input.nextInt();}while(sayi[i][j]<1 || sayi[i][j]>49);
            }
        }
        for (int i = 0; i < oyuncusayisi; i++) {
            System.out.print(isimler[i]+" : ");
            for (int j = 0; j < 15; j++) {
                System.out.print(sayi[i][j]+" - ");
            }
            System.out.println("");
        }
        for (int i = 0; i < 2000; i++) {
            int cikansayi=r.nextInt(50);
            System.out.println("Torbadan çıkan sayııııı: "+cikansayi);
            for (int j = 0; j < oyuncusayisi; j++) {
                for (int k = 0; k < 15; k++) {
                    if(cikansayi==sayi[j][k]){
                        sayi[j][k]=0;
                    }
                }
            }
            for (int j = 0; j < oyuncusayisi; j++) {
                System.out.print(isimler[j]+" : ");
                for (int k = 0; k < 15; k++) {
                    System.out.print(sayi[j][k]+" - ");
                }
            System.out.println("");
            }
            System.out.println("Rastgele bir tuşu enterlayınız.");
            String b=input.next();
            }
    }
} 
    
    

