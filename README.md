# L-gica-de-programa-o-
Lógica de programação exercícios resolvidos 


Algoritmo "contar_numero"
Var
   vetor: Vetor[1..20] de Inteiro
   i, num, contador: Inteiro

Inicio
   // Leitura
   Para i <- 1 Ate 20 faca
      Escreva("Digite o ", i, "º número: ")
      Leia(vetor[i])
   FimPara

   // Número a buscar
   Escreva("Digite o número para buscar: ")
   Leia(num)

   // Contagem
   contador <- 0
   Para i <- 1 Ate 20 faca
      Se vetor[i] = num Entao
         contador <- contador + 1
      FimSe
   FimPara

   Escreval("O número aparece ", contador, " vezes.")
FimAlgoritmo




Algoritmo "segundo_maior"
Var
   vetor: Vetor[1..10] de Inteiro
   i, maior, segundo: Inteiro

Inicio
   Para i <- 1 Ate 10 faca
      Escreva("Digite um número: ")
      Leia(vetor[i])
   FimPara

   maior <- vetor[1]
   segundo <- vetor[1]

   Para i <- 2 Ate 10 faca
      Se vetor[i] > maior Entao
         segundo <- maior
         maior <- vetor[i]
      Senao
         Se vetor[i] > segundo e vetor[i] <> maior Entao
            segundo <- vetor[i]
         FimSe
      FimSe





Algoritmo "soma_vetores"
Var
   v1, v2, v3: Vetor[1..10] de Inteiro
   i: Inteiro

Inicio
   // Leitura vetor 1
   Para i <- 1 Ate 10 faca
      Escreva("Vetor 1 - posição ", i, ": ")
      Leia(v1[i])
   FimPara

   // Leitura vetor 2
   Para i <- 1 Ate 10 faca
      Escreva("Vetor 2 - posição ", i, ": ")
      Leia(v2[i])
   FimPara

   // Soma
   Para i <- 1 Ate 10 faca
      v3[i] <- v1[i] + v2[i]
   FimPara

   // Exibição
   Escreval("Vetor resultante:")
   Para i <- 1 Ate 10 faca
      Escre(v3[i], " ")
   FimPara
FimAlgoritmo
   FimPara

   Escreval("Segundo maior valor: ", segundo)
FimAlgoritmo







Algoritmo "deslocar_vetor"
Var
   vetor: Vetor[1..10] de Inteiro
   i, x: Inteiro

Inicio
   Para i <- 1 Ate 10 faca
      Escreva("Digite um número: ")
      Leia(vetor[i])
   FimPara

   Escreva("Digite o valor X: ")
   Leia(x)

   // Deslocamento
   Para i <- 10 Ate 2 Passo -1 faca
      vetor[i] <- vetor[i-1]
   FimPara

   vetor[1] <- x

   Escreval("Vetor atualizado:")
   Para i <- 1 Ate 10 faca
      Escre(vetor[i], " ")
   FimPara
FimAlgoritmo




Algoritmo "ordem_crescente"
Var
   vetor: Vetor[1..15] de Inteiro
   i, j, aux: Inteiro

Inicio
   Para i <- 1 Ate 15 faca
      Escreva("Digite um número: ")
      Leia(vetor[i])
   FimPara

   // Comparação simples (tipo ordenação básica)
   Para i <- 1 Ate 14 faca
      Para j <- i+1 Ate 15 faca
         Se vetor[i] > vetor[j] Entao
            aux <- vetor[i]
            vetor[i] <- vetor[j]
            vetor[j] <- aux
         FimSe
      FimPara
   FimPara

   Escreval("Vetor em ordem crescente:")
   Para i <- 1 Ate 15 faca
      Escre(vetor[i], " ")
   FimPara
FimAlgoritmo



