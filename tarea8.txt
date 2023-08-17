package Tarea8;

import java.util.Scanner;

public class tarea8 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("Jugador 1");
        System.out.print("Ingrese su jugada (0: piedra, 1: papel, 2: tijera): ");
        int jugada1 = sc.nextInt();
        if (jugada1<0) {
        	System.out.println("tirada invalida, reinicie");
        }
        if (jugada1>2) {
        	System.out.println("tirada invalida, reinicie");
        } 	
        System.out.println("Jugador 2");
        System.out.print("Ingrese su jugada (0: piedra, 1: papel, 2: tijera): ");
        int jugada2 = sc.nextInt();     
        if (jugada2<0) {
        	System.out.println("tirada invalida, reinicie");
        }        
        if (jugada2>3) {
        	System.out.println("tirada invalida, reinicie");
        }
        if (jugada1==jugada2) {
        	System.out.println("es un empate");
        } else if (jugada1==0) {
        	if(jugada2==1) {
        		System.out.println("ganador jugador 2");
        	}
        		else if(jugada2==2) {
        			System.out.println("ganador  Jugador 1");
        		}
        }
        		else if (jugada1==1) {
        			if(jugada2==2) {
                		System.out.println("ganador jugador 2");
                	}
                		else if(jugada2==0) {
                			System.out.println("ganador  Jugador 1");
                		}
        		}
        		else if (jugada1==2) {
        			if(jugada2==0) {
                	System.out.println("ganador jugador 2");
                	}
                		else if(jugada2==1) {
                			System.out.println("ganador  Jugador 1");
                		}
                		
        		}

    }
}
