package controller;

import java.util.Scanner;

public class MatrizesDever {

	public static void main(String[] args) {
		int jogador, computador;
		Scanner teclado = new Scanner(System.in);
		System.out.println("_____JoKenPô_____");
		System.out.println("");
		System.out.println("1.Tesoura");
		System.out.println("2.Pedra");
		System.out.println("3.Papel");
		System.out.println("4.Spock");
		System.out.println("5.Lagarto");
		System.out.println("Digite a opçao que você deseja:");
		jogador = teclado.nextInt();

		switch (jogador) {
		case 1:
			System.out.println("Jogador escolheu TESOURA");
			break;
		case 2:
			System.out.println("Jogador escolheu PEDRA");
			break;
		case 3:
			System.out.println("Jogador escolheu PAPEL");
			break;
		case 4:
			System.out.println("Jogador escolheu SPOCK");
			break;
		case 5:
			System.out.println("Jogador escolheu LAGARTO");
			break;
		default:
		
			System.out.println("Opçao invalida");
			break;
		}

		teclado.close();
	}
}
