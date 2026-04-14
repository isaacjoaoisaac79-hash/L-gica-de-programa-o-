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









