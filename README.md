# Furkan
// 1.SORU KULLANICI TARAFINDAN GİRİLEN BİR POZİTİF TAM SAYININ FAKTORİYELİNİ HESAPLAMA

package faktoriyelhesaplama;

import java.util.Scanner;

public class FaktoriyelHesaplama {
  
    public static void main(String[] args) {
        int  i , sayi , faktoriyel =  1 ;
        Scanner klavye = new Scanner(System.in);
       
        System.out.println("Bir sayi giriniz ");
        sayi = klavye.nextInt();
        
        for ( i=sayi ; 1<i;i--){
            faktoriyel = faktoriyel*i;
        }
        System.out.println("faktoriyel : " + faktoriyel);
    }
    
}


// 2.SORUMUZ POZİTİF SAYILARDA ÇARPMA İŞLEMİNİ TOPLAMA KULLANARAK YAPMA 

package carpma;

import java.util.Scanner;


public class Carpma {

  
    public static void main(String[] args) {
        int sayi1 , sayi2 , carpma = 0 ; 
        Scanner klavye = new Scanner (System.in);
        
        System.out.println("Birinci sayiyi girin ");
        sayi1 = klavye.nextInt();
        
        System.out.println("ikinci sayiyi giriniz");
        sayi2 = klavye.nextInt();
        int x = sayi2 ; 
        while(sayi2>0){
            carpma = carpma + sayi1;
            sayi2--;
            
        } 
        System.out.println(sayi1+ " * " + x +" : " + carpma  );
    }
    
}

//3.SORUMUZ KULLANICI TARAFINDAN GİRİLEN POZİTİF BİR SAYIYA KADAR OLAN SAYILARIN KARELERİN TOPLAMI

package karelerintoplamı;

import java.util.Scanner;

public class KarelerinToplamı {

    
    public static void main(String[] args) {
        Scanner klavye = new Scanner(System.in);
        System.out.println("bir deger giriniz");
        int i ,  sayi ,toplam =0 ;
        
        sayi = klavye.nextInt();
        
        for(i =0;i<=sayi;i++){
            int j= (int) Math.pow(i,2);
            toplam += j;
        }
        System.out.println("girdiginiz sayıya kadar olan sayıların karelerin toplamı : " + toplam);
    }
    
}

//4.SORUMUZ GİRİLEN BİR SAYININ BASAMAKLARININ KÜPLERİ TOPLAMI SAYIYA EŞİT Mİ DEĞİL Mİ 

package kuptoplamıesitmi;

import java.util.Scanner;


public class KupToplamıEsitMi {

    
    public static void main(String[] args) {
        int sayi , bas , x, top = 0 ;
        Scanner klavye = new Scanner(System.in);
        System.out.print("bir sayı girin : ");
        sayi = klavye.nextInt();
        x=sayi;
        while(sayi>9){
            bas = sayi%10;
            top +=(bas*bas*bas);
            sayi = sayi/10;
        }
        top += (sayi*sayi*sayi);
        if (top==x)
            System.out.println("esit");
        else
            System.out.println("esit degil");
    }
    
}

// 5.SORUMUZ ÇARPIM TABLOSU OLUŞTURMAK 

package carpımtablosu;


public class CarpımTablosu {

    
    public static void main(String[] args) {
        int i , j ;
        for ( i=1;i<=10;i++){
            System.out.println("************");
            for(j =1;j<=10;j++){
                System.out.println(i+" * " + j + " = " + i*j);
            }
        }
    }
    
}

// 6.SORU  DAİRENİN ALANI VE ÇEVRESİNİ BULMA 

package soru2;

import java.util.Scanner;


public class Soru2 {

    
    public static void main(String[] args) {
            Scanner scanner = new Scanner(System.in);
            double pi = 3.14;
            double r ;
            System.out.println("Lütfen dairenin yarıçapını giriniz");
            // kullanıcı r girmeli alan= pi*r^2 , çevre = 2*pi*r
             r = scanner.nextDouble();
            double alan = pi*r*r;
            double cevre = 2*pi*r;
            System.out.println("dairenin alanı : " + alan );
            System.out.println("dairenin çevresi : " + cevre);
            
            
    }
    
}

// 7. SORUMUZ GİRİLEN DECİMAL (ONLUK) BİR SAYININ BİNARY (İKİLİK) SAYIYA DÖNÜŞTÜRME

package desimalbinary;

import java.util.Scanner;

public class DesimalBinary {

   
    public static void main(String[] args) {
        int sayi , i = 0 ; 
        int top = 0 ; 
        Scanner klavye = new Scanner(System.in);
        System.out.print("decimal sayi giriniz : ");
        sayi = klavye.nextInt();
        while(sayi>2){
            top += (sayi%2)*Math.pow(10, i);
            sayi = sayi/2 ;
            i++;
            
        }
        sayi = sayi/2;
        top += sayi*Math.pow(10, i);
        System.out.println("Binariy Karsiliği : " + top );
        
    }
    
}

// 8. SORUMUZ BOY KİLO ENDEKSİ HESAPLAMA 

package bki;

import java.util.Scanner;


public class BKİ {

   
    public static void main(String[] args) {
        double boy , kilo ,bki  ;
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("boyunuzu giriniz : ");
        boy = scanner.nextDouble();
        
        System.out.print ("Kilonuzu giriniz : ");
        kilo = scanner.nextDouble();
        boy = boy/100;
        bki = kilo / (boy*boy);
        
       if(bki <18)
    {
       System.out.print("ZAYIF ");
    }   
    else if(bki >= 18 && bki <25)
    {
        System.out.print("NORMAL ");
    }
    else if(bki >= 25 && bki <30)
    {
        System.out.print("KİLOLU ");        
    }
    else if(bki >= 30 && bki <35)
    {
        System.out.print("OBEZ" );
    }
    else
    {
        System.out.print("CİDDİ OBEZ" );
    }     
        
        
        
    }
    
}

// 9.SORUMUZ DENKLEMİN KÖKLERİNİ 


package bki;

import java.util.Scanner;


public class BKİ {

   
    public static void main(String[] args) {
        double boy , kilo ,bki  ;
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("boyunuzu giriniz : ");
        boy = scanner.nextDouble();
        
        System.out.print ("Kilonuzu giriniz : ");
        kilo = scanner.nextDouble();
        boy = boy/100;
        bki = kilo / (boy*boy);
        
       if(bki <18)
    {
       System.out.print("ZAYIF ");
    }   
    else if(bki >= 18 && bki <25)
    {
        System.out.print("NORMAL ");
    }
    else if(bki >= 25 && bki <30)
    {
        System.out.print("KİLOLU ");        
    }
    else if(bki >= 30 && bki <35)
    {
        System.out.print("OBEZ" );
    }
    else
    {
        System.out.print("CİDDİ OBEZ" );
    }     
        
               
              
        
    }
    
}
 
 // 10.SORUMUZ TAŞ - KAĞIT - MAKAS OYUNU 
 
 package furkan;

import java.util.Scanner;


public class Furkan {

    
 public static void main(String[] args) {
 
 Scanner s = new Scanner(System.in);
 
int kul_puan =0;
int bil_puan=0;

System.out.println("************|< Tas Kagıt Makas Oyununa Hosgeldiniz >|***********");

System.out.println("1-Taş 2-Kağıt 3-Makas");

while(true) {
System.out.println("Seçiminiz: ");
int secim = s.nextInt();
int bil_secim = (int)(Math.random()*3);

if (secim == 1) {
if (bil_secim == 1) {
System.out.println("Bilgisayarın seçimi: Taş Sonuç: Berabere");
System.out.println("Puanınız: "+kul_puan+" Bilgisayarın puanı:"+bil_puan);
} else if (bil_secim == 2) {
System.out.println("Bilgisayarın seçimi: Kağıt Sonuç: Kaybettiniz");
bil_puan++;
System.out.println("Puanınız: "+kul_puan+" Bilgisayarın puanı:"+bil_puan);
} else {
System.out.println("Bilgisayarın seçimi: Makas Sonuç: Kazandınız");
kul_puan++;
System.out.println("Puanınız: " + kul_puan + " Bilgisayarın puanı:" + bil_puan);
}

} else if (secim == 2) {
if (bil_secim == 1) {
System.out.println("Bilgisayarın seçimi: Taş Sonuç: Kazandınız");
kul_puan++;
System.out.println("Puanınız: "+kul_puan+" Bilgisayarın puanı:"+bil_puan);
} else if (bil_secim == 2) {
System.out.println("Bilgisayarın seçimi: Kağıt Sonuç: Berabere");
System.out.println("Puanınız: "+kul_puan+" Bilgisayarın puanı:"+bil_puan);
} else {
System.out.println("Bilgisayarın seçimi: Makas Sonuç: Kaybettiniz");
bil_puan++;
System.out.println("Puanınız: " + kul_puan + " Bilgisayarın puanı:" + bil_puan); }
} 

else if (secim == 3) {
if (bil_secim == 1) {
System.out.println("Bilgisayarın seçimi: Taş Sonuç: Kaybettiniz");
bil_puan++;
System.out.println("Puanınız: "+kul_puan+" Bilgisayarın puanı:"+bil_puan);
} else if (bil_secim == 2) {
System.out.println("Bilgisayarın seçimi: Kağıt Sonuç: Kazandınız");
kul_puan++;
System.out.println("Puanınız: "+kul_puan+" Bilgisayarın puanı:"+bil_puan);
} else {
System.out.println("Bilgisayarın seçimi: Makas Sonuç: Berabere");
System.out.println("Puanınız: " + kul_puan + " Bilgisayarın puanı:" + bil_puan);
}
}

else{
System.out.println("Hatalı giriş yaptınız tekrar deneyin");
continue;}

if(kul_puan==3){
System.out.println("Oyunu "+kul_puan+"-"+bil_puan+" kazandınız");
break; }

else if(bil_puan==3){
System.out.println("Oyunu "+bil_puan+"-"+kul_puan+" kaybettiniz");
break; }
}
         }
    
}
