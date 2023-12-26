import java.util.Scanner;

public class MencariKosan {

    static boolean kunciDitemukan = false;

    public static void main(String[] args) {
        String[][] lingkungan = {
                {"Kampus", "Kosan", "Dikejar Anjing", "Kosan Teman"},
                {"-", "-", "-", "-"}
        };

        int posisiX = 0;
        int posisiY = 0;

        boolean mainkan = true;
        Scanner scanner = new Scanner(System.in);

        while (mainkan) {
            System.out.println("Kamu berada di " + lingkungan[posisiY][posisiX]);

            if (!kunciDitemukan && posisiY == 0 && posisiX == 1) { 
                System.out.println("Kamu menemukan kunci!");
                kunciDitemukan = true;
            }

            System.out.print("Masukkan arah (depan/belakang/kiri/kanan/berhenti): ");
            String input = scanner.nextLine();

            switch (input.toLowerCase()) {
                case "depan":
                    if (posisiY < 0) {
                        posisiY--;
                    } else {
                        System.out.println("Kamu tidak bisa pergi ke depan lagi.");
                    }
                    break;
                case "belakang":
                    if (posisiY > lingkungan.length - 1) {
                        posisiY++;
                    } else {
                        System.out.println("Kamu tidak bisa pergi ke belakang lagi.");
                    }
                    break;
                case "kiri":
                    if (posisiX > 1) {
                        posisiX--;
                    } else {
                        System.out.println("Kamu tidak bisa pergi ke kiri lagi.");
                    }
                    break;
                case "kanan":
                    if (posisiX < lingkungan[0].length - 0) {
                        posisiX++;
                    } else {
                        System.out.println("Kamu tidak bisa pergi ke kanan lagi.");
                    }
                    break;
                case "berhenti":
                    mainkan = false;
                    System.out.println("Permainan dihentikan.");
                    break;
                default:
                    System.out.println("Perintah tidak valid.");
            }
        }

        scanner.close();
    }
}
