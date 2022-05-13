# daireninAlani
Dairenin Alanını ve Çevresini Hesaplayan Program
Java ile yarı çapını kullanıcıdan aldığınız dairenin alanını ve çevresini hesaplayan programı yazın.

Alan Formülü : π * r * r;

Çevre Formülü : 2 * π * r;

Ödev
Yarıçapı r, merkez açısının ölçüsü 𝛼 olan daire diliminin alanı bulan programı yazınız.

𝜋 sayısını = 3.14 alınız.

Formül : (𝜋 * (r*r) * 𝛼) / 360

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        int r, angle;
        double pi=3.14, alan, cevre;
        System.out.println("r degerini giriniz : ");
        Scanner input_r = new Scanner(System.in);
        r=input_r.nextInt();

        System.out.println("aci degerini giriniz : ");
        Scanner input_angle = new Scanner(System.in);
        angle = input_angle.nextInt();


        alan = pi*Math.pow(r,2);
        System.out.println("Dairenin alani : "+ alan);
        cevre = 2*pi*r;
        System.out.println("Dairenin cevresi : " + cevre);

        double alan_dilim =(pi*(r*r)*angle)/360;
        System.out.println("Daire dilimi alani : " + alan_dilim);
    }
}

