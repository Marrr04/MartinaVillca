import java.util.Random;

public class tarea20 {
    public static void main(String[] args) {
        int contador = 0;
        int maximo = Integer.MIN_VALUE; // Valor mínimo posible para un entero
        int minimo = Integer.MAX_VALUE; // Valor máximo posible para un entero

        Random random = new Random();

        do {
            int numero = random.nextInt(100); // Generar número aleatorio entre 0 y 99
            System.out.println("Número generado: " + numero);

            if (numero > maximo) {
                maximo = numero;
            }

            if (numero < minimo) {
                minimo = numero;
            }

            contador++;
        } while (contador < 10);

        System.out.println("Máximo número generado: " + maximo);
        System.out.println("Mínimo número generado: " + minimo);
    }
}
