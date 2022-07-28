# Soma-de-todos-os-valores-do-terceio-vetor-codigo-Java

Considere o seguinte problema:

Escreva um programa que leia dois vetores contendo números reais com 10 posições e preenche um terceiro vetor de 10 posições, contendo a multiplicação dos números presentes em cada um dos dois primeiros vetores. Por exemplo, a posição 1 do terceiro vetor conterá a multiplicação dos valores armazenados na posição 1 dos dois primeiros vetores. O programa deve mostrar então a soma dos valores de todas as posições do terceiro vetor.

Complete o programa abaixo arrastando e soltando os trechos de código nos espaços em branco, de forma que o programa implemente corretamente o problema acima.



public class ProdutoEscalar {
	public static void main(String[] args) {
		double[] vetorA = new double[10];
		double[] vetorB = new double[10];
		[double[] resultados = new double[10];]
		
		// Leitura
		for(int cont = 0; cont < vetorA.length; cont++) {
			System.out.printf("Vetor A posicao %d: ", cont);
			[vetorA[cont] = Double.parseDouble(System.console().readLine());]
		}
		for(int cont = 0; cont < vetorB.length; cont++) {
			System.out.printf("Vetor B posicao %d: ", cont);
			[vetorB[cont] = Double.parseDouble(System.console().readLine());]
		}
		
		// Processamento
		for(int cont = 0; cont < vetorA.length; cont++) {
			[resultados[cont] = vetorA[cont] * vetorB[cont];]
		}
		
		double soma = 0;
		for(int cont = 0; cont < resultados.length; cont++) {
			[soma += resultados[cont];]
		}
		
		// Saida
		System.out.printf("\nSOMA DOS PRODUTOS DOS ELEMENTOS DOS VETORES (PRODUTO ESCALAR) = %f\n", soma);
	}
}
