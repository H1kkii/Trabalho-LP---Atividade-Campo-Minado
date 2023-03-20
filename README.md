# Trabalho-LP---Atividade-Campo-Minado
algoritmo campominado
// Função :Jogo CampoMinado
// Autor :
// Data : 17/03/2023
// Seção de Declarações 
var
mat: vetor[1..5,1..5] de inteiro
posia: inteiro
posib: inteiro
score: inteiro
inicio
mat [1,1] := 2
mat [1,2] := 1
mat [1,3] := 1
mat [1,4] := 2
mat [1,5] := 1
mat [2,1] := 1
mat [2,2] := 1
mat [2,3] := 1
mat [2,4] := 1
mat [2,5] := 2
mat [3,1] := 1
mat [3,2] := 1
mat [3,3] := 1
mat [3,4] := 1
mat [3,5] := 1
mat [4,1] := 1
mat [4,2] := 1
mat [4,3] := 2
mat [4,4] := 1
mat [4,5] := 1
mat [5,1] := 1
mat [5,2] := 1
mat [5,3] := 1
mat [5,4] := 1
mat [5,5] := 2
repita
escreva("Digite o número da linha selecionada: ")
leia(posia)

escreva("Digite o número da coluna selecionada: ")
leia(posib)

se(mat[posia,posib] = 2) entao
escreva("Você perdeu,encontrou uma bomba 😦 ")
fimse

se(mat[posia,posib] = 1) entao
escreva("Espaço vago, digite novamente as cordenadas ")
fimse

se (score = 20) entao
escreva("Você ganhou!!! pinas paga sua pizza 🙂  ")
fimse

se (mat[posia,posib] = 1) entao
score := score + 1
fimse
ate (mat[posia,posib] = 2)

fimalgoritmo
