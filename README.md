# Cálculo de nps

O desafio serve para praticar algumas coisas: leitura de arquivos,  um pouco de lógica, e tem algumas formas de evoluir esse desafio

## Descrição

Você deve ler os arquivos csv, e fazer o cálculo da NPS (**Net Promoter Score**) para cada operador, e para a empresa já que no mesmo atendimento, eles recebem notas diferentes

O cálculo da NPS é dado da seguinte forma:
* Notas entre 1 até 6 são **ruins**;
* Notas 7 e 8 são **neutras**;
* Notas 9 e 10 **boas**;

total = boas + neutras + ruins
<br>
NPS = (boas)/(total)-(ruins)/(total)

## Arquivos Iniciais

Você tem 3 arquivos csv, cada um tem uma lista de notas dadas por clientes para avaliar o desempenho de um operador, bem como a organização

## Observação

No momento não temos uma forma de validar as respostas, mas quem sabe um dia

## Desafios adicionais

* "Otimizar" o tempo de execução:
  * Uma forma de verificar melhor o tempo de execução, é colocando um delays de 0.1 segundo para cada iteração
  * A solução é trabalhar com multithreading, e encontrar uma forma de reduzir o tempo de execução do programa
  * Assim que tiver conseguido optimizar o tempo de execução, retire o delay
* Separar os setores:
  * Os operadores tem uma marca no início do nome, isso indica se é um setor especial de clientes ou não
  * Ao invés de fazer o cálculo para a empresa toda, faça o cálculo para os 2 setores
