Duplas: Guilherme Roizentul e Henrique Vitor

Descrição do jogo:
O campo minado é um jogo simples, ao iniciar o jogo você deve clicar para abrir o primeiro campo,
se no bloco no qual você clicou aparecer o número três, significa que existem três locais ao redor 
desse bloco que você não pode clicar, o objetivo é você descobrir onde estão todas as bombas sem clicar nelas.

Codigo em português estruturado 
# Trabalho-LP-Atividade-Campo-Minado
algoritmo campominado
// Função :Jogo CampoMinado
// Autor : Guilherme Roizentul e Henrique Vitor
// Data : 17/03/2023
// Seção de Declarações 
var
mat: vetor[1..5,1..5] de inteiro
posi: inteiro
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
mat [3,5] := 2
mat [4,1] := 1
mat [4,2] := 1
mat [4,3] := 2
mat [4,4] := 1
mat [4,5] := 1
mat [5,1] := 1
mat [5,2] := 2
mat [5,3] := 1
mat [5,4] := 1
mat [5,5] := 1

repita
escreva("Digite o número da linha selecionada: ")
leia(posi)

escreva("Digite o número da coluna selecionada: ")
leia(posib)

se(mat[posi,posib] = 2) entao
escreva("Você perdeu,encontrou uma bomba ")
fimse

se(mat[posi,posib] = 1) entao
escreva("Espaço vago, digite novamente as cordenadas ")
fimse

se (score = 20) entao
escreva("Você ganhou!!! pinas paga sua pizza  ")
fimse

se (mat[posi,posib] = 1) entao
score := score + 1
fimse
ate (mat[posi,posib] = 2)

fimalgoritmo
