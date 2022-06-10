package controller;

import java.util.Scanner;

public class PedraPapelTesoura {

	public static void main(String[] args) {

		int jogador, computador;
		Scanner teclado = new Scanner(System.in);
		System.out.println("_JoKenPô_");
		System.out.println("");
		System.out.println("1. Pedra");
		System.out.println("2. Papel");
		System.out.println("3. Tesoura");
		System.out.println("4. Lagarto");
		System.out.println("5. Spock");
		System.out.println("Digite a opção desejada");

		jogador = teclado.nextInt();
		System.out.println("");
		switch (jogador) {
		case 1:
			System.out.println("Jogador escolheu PEDRA");
			break;
		case 2:
			System.out.println("jogador escolheu PAPEL");
			break;
		case 3:
			System.out.println("jogador escolheu TESOURA");
			break;
		case 4:
			System.out.println("jogador escolheu LAGARTO");
			break;
		case 5:
			System.out.println("jogador escolheu SPOCK");
			break;
		default:
			System.out.println("Opção invalida");
			break;
		}
		computador = (int) (Math.random() * 5 + 1);
		teclado.close();
		switch (computador) {
		case 1:
			System.out.println("Computador escolheu PEDRA");
			break;
		case 2:
			System.out.println("Computador escolheu PAPEL");
			break;
		case 3:
			System.out.println("Computador escolheu TESOURA");
			break;
		case 4:
			System.out.println("Computador escolheu LAGARTO");
			break;
		case 5:
			System.out.println("Computador escolheu SPOCK");
			break;
		}
		System.out.println("");
		if (jogador == computador) {
			System.out.println("EMPATE");
		} else {
			if ((jogador == 1 && computador == 3) || (jogador == 2 && computador == 1)
					|| (jogador == 3 && computador == 2) || (jogador == 4 && computador == 2)
					|| (jogador == 4 && computador == 5) || (jogador == 5 && computador == 1)
					|| (jogador == 5 && computador == 3)) {

				System.out.println("JOGADOR VENCEU");
			} else {
				System.out.println("COMPUTADOR VENCEU");
			}

		}
	}

}
