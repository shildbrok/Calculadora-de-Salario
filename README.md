# Calculadora-de-Salario
Vamos Abordar a lógica por trás de uma calculadora de salario.


## Exercício numero 3:

Possivel Solução:

``````
Algoritmo "salarioCalc"
// Disciplina   : [Linguagem e Lógica de Programação]
// Descrição   : Exercicio 3 lista 1
// Autor(a)    : José Estevan Moreira Generoso
// Data atual  : 28/02/2023
Var
//Vamos Defenir algumas Variaveis
//Vamos olhar quais infrormações devemos ter
//Horas trabalhadas = hTrabalhadas
//Valor do salario Minimo = vlrSlrMinimo
//Total do salario bruto = slrBruto
//Imposto = imposto <- 3%
//Salario liquido = slrLiquido - Imposto
//Valor da hora trabalhada = vlrHora
hTrabalhadas, vlrSlrMinimo, slrBruto, slrLiquido, vlrHora, imposto: real


//Vamos adicionar uma condição de repetição em nosso código,
//então vamos criar uma variavel chamada resposta do tipo Caractere
resposta: caractere

Inicio
//Primeiro vamos infeitar nossa tela, não é necessário!
//Porém um componemte visual é semple legal de colocar.
EscrevaL("**********************************************")
EscrevaL("------------Calculadora de Salario------------")
EscrevaL("**********************************************")


//Vamos iniciar a Atividade
//estruturas de condições são muito utilizadas para repitir uma tarefa desejada
//até a retefa ter a resposta definida para o encerramento.
//A Palavra reservada para a repição é Enquanto. Vamos Lá!
resposta <- "S"
Enquanto (resposta = "S") ou (resposta = "s") ou (resposta <> "N") e (resposta <> "n") faca
         //Estrutura Se, utilizada para fazer certa caso a receba certo tipo de resposta
         Se(resposta = "S") ou (resposta = "s") entao
                     //Se a resposta for S ou s, então fará:
                     Escreval("Digite o Numero de Horas que foi trabalhado: ")
                     Leia(hTrabalhadas)
                     Escreva(" ")
                     EscrevaL("Qual o valor do salário minimo")
                     Leia(vlrSlrMinimo)
                     Escreva(" ")
                     
                     vlrHora <- vlrSlrMinimo / 5
                     slrBruto <- hTrabalhadas * vlrHora
                     imposto <- slrBruto * 0.03
                     slrLiquido <- slrBruto - imposto
                     
                     
                     EscrevaL("------------------------------------")
                     Escreval("Seu salário mínimo é: ", vlrSlrMinimo)
                     EscrevaL("------------------------------------")
                     EscrevaL("Seu salário Bruto é: ", slrBruto)
                     EscrevaL("------------------------------------")
                     EscrevaL("Seu salário Liquido é: ", slrLiquido)
                     EscrevaL("------------------------------------")
                     EscrevaL("O Valor da sua H/Trabalho é :", vlrHora)
                     EscrevaL("------------------------------------")
                     Escreval("O valor que você pagou de imposto é", imposto)
                     EscrevaL("------------------------------------")
                     
                     //aqui vamos fazer a pergunte que muda a variavel resposta
                     //saindo da sequencia de informação
                     Escreval("Deseja Continuar S/N")
                     leia(resposta)
                     //Palavra Reservada para limpar a tela
                     LimpaTela
         senao
              Se(resposta = "N") ou (resposta = "n")
              EscrevaL("Obrigado!")
              LimpaTela
         fimSe
fimEnquanto
//Esse algoritimo foi desenvolvido pensando em uma solução da lista de exercicios
//Caso queira fazer uma sujestão de correção ou fazwer alguma pergunta,
//Pode me chamar no whatsapp
//Abraço a todos, beijo na bunda... E bons estudos!
Fimalgoritmo

```
