//PROBLEMA 1
import java.util.Scanner;

public class MadLib {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Bună! Hai să jucăm Mad Libs.");
        System.out.print("Dă-mi un substantiv: ");
        String substantiv1 = scanner.nextLine();

        System.out.print("Dă-mi un alt substantiv: ");
        String substantiv2 = scanner.nextLine();

        System.out.print("Dă-mi un adjectiv: ");
        String adjectiv = scanner.nextLine();

        System.out.print("Dă-mi un verb la trecut: ");
        String verb = scanner.nextLine();

        System.out.println("Povestea ta Mad Libs:");

        System.out.println(substantiv1 + " had a little " + substantiv2);
        System.out.println("Its " + substantiv2 + " was " + adjectiv + " as snow");
        System.out.println("And everywhere that " + substantiv1 + " " + verb);
        System.out.println("The " + substantiv2 + " was sure to go.");

        scanner.close();
    }
}

//PROBLEMA 2
import java.util.Scanner;

public class CarlysEventPrice {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Bună! Bine ați venit la Carly's Catering.");
        System.out.print("Introduceți numărul de invitați: ");
        int numarInvitati = scanner.nextInt();

        int pretPePersoana = 35;
        int pretTotal = numarInvitati * pretPePersoana;
        boolean esteEvenimentMare = numarInvitati >= 50;

        System.out.println("Devisul companiei Carly's Catering:");
        printChenar('*', 40);
        System.out.println("Număr de invitați: " + numarInvitati);
        System.out.println("Preț per persoană: $" + pretPePersoana);
        System.out.println("Preț total: $" + pretTotal);
        System.out.println("Acesta este un eveniment mare: " + esteEvenimentMare);
        printChenar('*', 40);

        scanner.close();
    }

    // Metoda pentru a afișa un chenar
    public static void printChenar(char caracter, int lungime) {
        for (int i = 0; i < lungime; i++) {
            System.out.print(caracter);
        }
        System.out.println();
    }
}

//PROBLEMA 3

import java.util.Scanner;

public class SammysRentalPrice {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Bună! Bine ați venit la Sammy's Seashore Supplies.");
        System.out.print("Introduceți numărul de minute pentru închiriere: ");
        int minute = scanner.nextInt();

        int costPeOra = 40;
        int costPeMinutSuplimentar = 1;

        int ore = minute / 60;
        int minuteSuplimentare = minute % 60;

        int costTotal = (ore * costPeOra) + (minuteSuplimentare * costPeMinutSuplimentar);

        System.out.println("Deviza
