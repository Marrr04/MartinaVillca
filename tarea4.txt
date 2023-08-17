import java.util.Scanner;

public class tarea4 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        System.out.print("Ingrese la categoría (a, b o c): ");
        char categoria = sc.next().charAt(0);
        
        if (categoria == 'a') {
            System.out.println("Hijo");
        } else if (categoria == 'b') {
            System.out.println("Padres");
        } else if (categoria == 'c') {
            System.out.println("Abuelos");
        } else {
            System.out.println("Categoría inválida");
        }
    }
}
