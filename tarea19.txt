
import java.util.Random;

public class tarea19 {
    public static void main(String[] args) {
        int contador = 0;
        int suma = 0;
        double promedio;

        Random random = new Random();

        while (contador < 10) {
            int numero = random.nextInt(100); // Generar número aleatorio entre 0 y 99
            System.out.println("Número generado: " + numero);

            suma += numero;
            contador++;
        }

        promedio = (double) suma / 10;

        System.out.println("Suma de los números: " + suma);
        System.out.println("Promedio de los números: " + promedio);
    }
}
