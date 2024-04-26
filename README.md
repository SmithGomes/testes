# Testes


1 )  Observe o trecho de código abaixo:

		int INDICE = 13, SOMA = 0, K = 0;
		
		enquanto K < INDICE faça{
		    K = K + 1;
		    SOMA = SOMA + K;
		}

		imprimir(SOMA);
		


Ao final do processamento, qual será o valor da variável SOMA?
**R = 91**

[Soma](https://github.com/SmithGomes/testes/blob/main/soma.html)


2 ) Dado a sequência de Fibonacci, onde se inicia por 0 e 1 e o próximo valor sempre será a soma dos 2 valores anteriores (exemplo: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34...), escreva um programa na linguagem que desejar onde, informado um número, ele calcule a sequência de Fibonacci e retorne uma mensagem avisando se o número informado pertence ou não a sequência.

IMPORTANTE:
Esse número pode ser informado através de qualquer entrada de sua preferência ou pode ser previamente definido no código;

[Sequência Fibonacci](https://github.com/SmithGomes/testes/blob/main/fibonacci.html)


3) Descubra a lógica e complete o próximo elemento:

a) 1, 3, 5, 7, ___ **9**

b) 2, 4, 8, 16, 32, 64, ____ **128**

c) 0, 1, 4, 9, 16, 25, 36, ____ **49**

d) 4, 16, 36, 64, ____ **100**

e) 1, 1, 2, 3, 5, 8, ____ **13**

f) 2, 10, 12, 16, 17, 18, 19, ____ 



4 ) Você está em uma sala com três interruptores, cada um conectado a uma lâmpada em uma sala diferente. Você não pode ver as lâmpadas da sala em que está, mas pode ligar e desligar os interruptores quantas vezes quiser. Seu objetivo é descobrir qual interruptor controla qual lâmpada.

Como você faria para descobrir, usando apenas duas idas até uma das salas das lâmpadas, qual interruptor controla cada lâmpada?

	- 1 interruptor e checando qualquer lampada:
		- caso esteja ligada, com apenas mais uma checagem chega-se a solução ( total 2 checagens )
		- caso esteja desligada, obrigatoriamente, devo fazer mais duas checagens ( total 3 checagens )

	 

	- 2 interruptores e checando qualquer lampada:
		- Ligar I1 e I2, checar LA
			- Se apagada, então será I3-LA, restando I1 e I2, LB e LC
				- dai, apaga I1, I2 ligado, checa-se LB ( total 2 checagens )
					- se acesa, então I2-LB e I3-LC
					- se apagada, então I3-LB e I2-LC

			- Se acesa, então I1 ou I2
				- dai, desliga I1, I2 ligado, checa-se LA
				
					- se acesa, então I2-LA, restando I1 e I3, LB e LC
						- dai, apenas I1 ligado, checa-se LB ( total 3 checagens )
							- se ligada, I1-LB e I3-LC
							- se apagada, I1-LC e I3-LB

					- se apagada, então I1-LA, restando I2 e I3, LB e LC
						- dai, apenas I2 ligado, checa-se LB ( total 3 checagens )
							- se ligada, I2-LB e I3-LC
							- se apagada, I2-LC e I3-LB

**R = 
	1 interruptor, se na primeira checagem estiver ACESA, é possivel solução com apenas 2 checagens, caso contrário com 3 checagens.
	2 interruptores, se na primeira checagem estiver APAGADA, é possivel solução com apenas 2 checagens, caso contrário com 3 checagens.
	**
	 

5 ) Escreva um programa que inverta os caracteres de um string.

[Inverte string](https://github.com/SmithGomes/testes/blob/main/inverte_string.html)
