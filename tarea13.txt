import java.util.Scanner;

public class tarea13 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        System.out.print("Ingrese el nombre de un mes: ");
        String nombreMes = sc.nextLine().toLowerCase();
        
        int cantidadDias;
        
        switch (nombreMes) {
            case "enero":
            case "marzo":
            case "mayo":
            case "julio":
            case "agosto":
            case "octubre":
            case "diciembre":
                cantidadDias = 31;
                break;
            case "abril":
            case "junio":
            case "septiembre":
            case "noviembre":
                cantidadDias = 30;
                break;
            case "febrero":
                cantidadDias = 28;
                break;
            default:
                cantidadDias = -1; //indicativo de mes inválido
                break;
        }
        
        if (cantidadDias == -1) {
            System.out.println("Nombre de mes inválido.");
        } else {
            System.out.println("El mes de " + nombreMes + " tiene " + cantidadDias + " días.");
        }
    }
}
