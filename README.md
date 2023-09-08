# Lendo-dados-do-teclado-usando-a-classe-Scanner

Anotações de Lendo dados do teclado usando a classe Scanner

                                                              Lendo dados do teclado usando a classe Scanner

O que vamos fazer

.Como ler dados do teclado
 .Ler uma linha inteira
 .Ler tipo de dado específico

                                                                      Nosso assistente

.Classr Scanner

   Scanner scan = new Scanner(System.in);

Para a gente poder ler algum dado do teclado no java nós vamos útilizar a classe Scanner, que é da API java, e é bem simples, a gente só precisa colocar no
nosso código essa linha que tá na tela. Na parte scan da linha nós podemos dar o nome que quiser, mas vamos ficar com scan mesmo. O sinal de retribuição(=)
e o new Scanner que vai instânciar essa classe para gente, e nós vamos passar como parametro o System.in.
 A gente vai usar a classe Scanner, mas existem outras duas classes em que a gente consegue fazer leitura de dados do teclado, mas a classe Scanner é a
classe mais facil para a gente fazer isso, a API do java está organizada em várias pastas, e por causa dessa organização a gente também pricisa dizer
para o nosso programa java que a gente quer útilizar essa classe e a maneira que a gente faz isso é antes da declaração da nossa classe colocar o
import, que é a maneira que a gente vai dizer pro java "Oi java, eu quero útilizar essa classe Scanner no código", então são esses dois detales para a
gente entender Lendo dados do teclado.

Ex:

       import_java.util.Scanner;

       public class LeituraDadosTeclado {

       }



         Opção 1:Lendo uma linha inteira

A primeira maneira que a gente pode ler dados do teclado é lendo uma linha inteira, então não inporta o que você colocar nessa linha, quando você
apertar enter o java vai conseguir ler essa informação, e a gente faz desse jeito.

  String nome = scan.nextLine();

A gente vai atribuir tudo isso a uma váriavel do tipo String, e a gente vai útilizar esse nextLine da classe Scanner, e é um métoro chamado
nextLine e a gente vai conseguir ler tudo.


         Opção 1:Lendo um tipo específico

        String primeiroNome = scan.next();
        int idade = scan.nextInt();
        double altura = scan.nextDouble();

se a gente quiser ler um dado de tipo específico do teclado que é o que seria a opção 2 a gente pode útilizar outros métodos por exemplo o next
ele vai ler o que for que você vai ter colocado e ele retorna uma String então a gente tem que atribuir isso a uma String, o nextInt ele vai
conseguir ler um inteiro, o nextFouble ele retorna um Double, também existem outros métodos como o nextShort, nextByte, nextFlooat,
nextBoolean, existem os métodos prós tipos promitivos do java e além do next de retorna a String e o nextLine.

EX1 lendo a linha de uma vez:
package com.madu.LeituraDadosDoTeclado;

import java.util.Scanner;

public class LeituraDadosDoTeclado {

	public static void main(String[] args) {
		
		Scanner scan = new Scanner(System.in);
		
		System.out.println("Digite seu nome completo:");
		String nomeCompleto = scan.nextLine();
	}

}

Console:
        Digite seu nome completo:
Madu

Com esse código da para escrever no console.

EX2 lendo a linha de uma vez:

package com.madu.LeituraDadosDoTeclado;

import java.util.Scanner;

public class LeituraDadosDoTeclado {

	public static void main(String[] args) {
		
		Scanner scan = new Scanner(System.in);
		
		System.out.println("Digite seu nome completo:");
		String nomeCompleto = scan.nextLine();
		System.out.println("Seu nome completo é: " + nomeCompleto);
		
		
	}

}


Console:
        Digite seu nome completo:
Madu


package com.madu.LeituraDadosDoTeclado;

import java.util.Scanner;

public class LeituraDadosDoTeclado {

	public static void main(String[] args) {
		
		Scanner scan = new Scanner(System.in);
		
		System.out.println("Digite seu nome completo:");
		String nomeCompleto = scan.nextLine();
		System.out.println("Seu nome completo é: " + nomeCompleto);
		
		System.out.println("Digite seu primeiro nome:");
		String primeiroNome = scan.next();
		System.out.println("Seu primeiro nome é: " + primeiroNome);
		
		System.out.println("Digite a sua idade: ");
		int idade = scan.nextInt();
		System.out.println("Sua idade é: " + idade);
		
		System.out.println("Digite a sua altura: ");
		double altura = scan.nextDouble();
		System.out.println("A sua altura é: " + altura);
	}

}



NOTA: se for um nome então devemos colocar a variável String, se for.

Também podemos ler tudo en um comando


package com.madu.LeituraDadosDoTeclado;

import java.util.Scanner;

public class LeituraDadosDoTeclado {

	public static void main(String[] args) {
		
		Scanner scan = new Scanner(System.in);

		System.out.println("Digite o seu primeiro nome, idade, altura e se tem bichinho de estimação");
		String primeiroNome = scan.next();
		int idade = scan.nextInt();
		float altura = scan.nextFloat();
		boolean temPet = scan.nextBoolean();
		
		System.out.println("Você digitou os seguintes valores:");
		System.out.println("Primeiro nome: " + primeiroNome);
		System.out.println("Idade: " + idade);
		System.out.println("Altura: " + altura);
		System.out.println("Tem bichinho de estimação? " + temPet);
	}

}

Console: Digite o seu primeiro nome, idade, altura e se tem bichinho de estimação

 Maria 14 1,20 false

Você digitou os seguintes valores:

Primeiro nome:Maria
Idade:14
Altura:1,2
Tem bichinho de estimação? false

Se eu adicionar mais palavras ou números que eu não tenha feito um código então a palavra não vai aparecer.
