import java.io.IOException;
import java.util.Scanner;

public class App {
    public static void main(String[] args) throws IOException  {
        Scanner scan = new Scanner(System.in);
        boolean lanjutkan = true;

        while(lanjutkan){
        //main menu
        clearscreen();
        System.out.println("database parpustakaan");
        System.out.println("1. \tlihat seluruh buku");
        System.out.println("2. \tcari data buku");
        System.out.println("3. \ttambah data buku");
        System.out.println("4. \tubah data buku");
        System.out.println("5. \thapus data buku");

        System.out.print("\n\npilihan anda: ");
        String pilihan = scan.next();

        switch(pilihan){
            case "1":
            System.out.println("list seluruh buku");
            //tampilkan data
            tampilkan_data();
            break;
            case "2":
            System.out.println("cari buku");
            //cari data
            break;
            case "3":
            System.out.println("tambah buku");
            //tambah data
            break;
            case "4":
            System.out.println("ubah buku");
            //ubah data
            break;
            case "5":
            System.out.println("hapus buku");
            //hapus data
            break;
            default:
            System.err.println("\n input tidak ditemukan\nsilahkan masukan angka 1 - 5");
            
        }
            
            lanjutkan = yesorno("apakah anda ingin melanjutkan");
        }
        
    



    }


    private static void tampilkan_data() throws IOException  {
    System.out.println("bentar");
    }


    //lanjut atau tidak
    private static boolean yesorno(String massage){
            Scanner scan = new Scanner(System.in);
            System.out.println("\n"+ massage+" yes/no?");
            String lanjutAtauTidak = scan.next();
            if(lanjutAtauTidak.equalsIgnoreCase("yes") == false && lanjutAtauTidak.equalsIgnoreCase("no") == false){
                System.out.println("pilihan anda cuma yes/no");
                yesorno("anda mau lanjut tidak");
            }
            return lanjutAtauTidak.equalsIgnoreCase("yes");
            
    }


    //clear screen
    private static void clearscreen(){
        try{
            if(System.getProperty("os.name").contains("Windows")){
                new ProcessBuilder("cmd","/c","cls").inheritIO().start().waitFor();
            }else{
                //unix
                System.out.println("\033\143");
            }
        }catch(Exception ex){
            System.err.println("gk bs clear screen");
        }
    }
}

