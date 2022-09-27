/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package percabangan;

import java.util.Scanner;

/**
 *
 * @author LENOVO CORE I5
 */
public class PernyataanSWITCH3 {
    public static void main(String[]args){
        Scanner input=new Scanner(System.in);
        int tahun, bulan, hari = 0;
        System.out.println("Masukkan Tahun : ");
        tahun=input.nextInt();
        System.out.println("Masukkan Bulan : ");
        bulan=input.nextInt();
        
        switch (bulan){
            case 1:
            case 3:
            case 5:
            case 7: 
            case 8:
            case 10:
            case 12:
                hari=31;
                break;
            case 4:
            case 6:
            case 9:
            case 11:    
                hari=30;
                break;
            case 2:
                if (((tahun%4==0)&&!(tahun%100==0)) || (tahun%400==0) )
                    hari=29;
                else 
                    hari=28;
                break;    
            default:
                System.out.println("Invalid month");
                break;
                
        }
        System.out.println("Jumalah hari pada "+tahun+" bulan "+bulan+" adalah "+hari+" hari");
    }
}
