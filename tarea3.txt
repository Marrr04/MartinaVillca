import java.util.Scanner;

public class tarea3 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        System.out.print("Ingrese el nombre del mes: ");
        String nombreMes = sc.nextLine();
        
        if (nombreMes.equalsIgnoreCase("enero") || nombreMes.equalsIgnoreCase("marzo") ||
            nombreMes.equalsIgnoreCase("mayo") || nombreMes.equalsIgnoreCase("julio") ||
            nombreMes.equalsIgnoreCase("agosto") || nombreMes.equalsIgnoreCase("octubre") ||
            nombreMes.equalsIgnoreCase("diciembre")) {
            System.out.println(nombreMes + " tiene 31 días");
        } else if (nombreMes.equalsIgnoreCase("febrero")) {
            System.out.println(nombreMes + " tiene 28 días");
        } else if (nombreMes.equalsIgnoreCase("abril") || nombreMes.equalsIgnoreCase("junio") ||
                   nombreMes.equalsIgnoreCase("septiembre") || nombreMes.equalsIgnoreCase("noviembre")) {
            System.out.println(nombreMes + " tiene 30 días");
        } else {
            System.out.println("Nombre de mes inválido");
        }
    }
}
