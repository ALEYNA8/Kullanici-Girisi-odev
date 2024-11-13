# Kullanici-Girisi-
import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        String userName, password;
        Scanner inp = new Scanner(System.in);

        System.out.print("Kullanıcı Adınız: ");
        userName = inp.nextLine();

        System.out.print("Şifreniz: ");
        password = inp.nextLine();

        if (userName.equals("Patika") && password.equals("java123")) {
            System.out.println("Giriş Yapınız ! ");
        } else {
            System.out.println("Bilgileriniz Yanlış !");
            System.out.print("Şifrenizi Sıfırlamak İster Misiniz? (Evet/Hayır): ");
            String sifirlaSecim = inp.nextLine();

            if (sifirlaSecim.equalsIgnoreCase("Evet")) {
                System.out.print("Yeni Şifre Giriniz: ");
                String yeniSifre = inp.nextLine();

                while (yeniSifre.equals("java123")) {
                    System.out.println("Şifre oluşturulmadı,lütfen tekrar başka şifre giriniz.");
                    System.out.print("Yeni şifre giriniz: ");
                    yeniSifre = inp.nextLine();
                }
                System.out.println("Şifre oluşturuldu");
                }
              }

        }

    }
