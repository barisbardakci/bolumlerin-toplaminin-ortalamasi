# bolumlerin-toplaminin-ortalamasi
Java101_16 Döngüler ile 0'dan girilen sayıya kadar olan sayılardan 3 ve 4'e tam bölünen sayıların ortalamasını hesaplayan program

https://www.patika.dev/tr

/* Ödev
Java döngüler ile 0'dan girilen sayıya kadar olan sayılardan 3 ve 4'e tam bölünen sayıların ortalamasını hesaplayan programı yazınız.*/

import java.util.Scanner;
public class Main
{
	public static void main(String[] args) {
	    
	    int num, toplam=0, sayac=0 ;
	    
	    
	    Scanner input=new Scanner(System.in);
	    System.out.print("Sayı giriniz : ");
	    num=input.nextInt();
	    
	    for(int i=1 ; i<=num ; i++){
	        if(i%3==0 && i%4==0){
	            toplam+=i ;
	            sayac++;
	            System.out.print(i+" ");
	        }
	    }
	    System.out.print("\n"+num+" sayısının 3 ve 4'e bölenlerin toplamının ortalaması :"+toplam/sayac);
	}
}
