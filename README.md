# SALARIO BRUTO INSS IRFF
Algoritmo "semnome"
// Disciplina   : [Linguagem e Lógica de Programação]
// Professor   : Antonio Carlos Nicolodi 
// Descrição   : Aqui você descreve o que o programa faz! (função)
// Autor(a)    : Nome do(a) aluno(a)
// Data atual  : 13/03/2024
Var
// Seção de Declarações das variáveis 
 inss: real
irrf: real
salariobruto: real
salarioliquido: real

Inicio
// Seção de Comandos, procedimento, funções, operadores, etc...
ESCREVAL("Digite seu salário bruto: ")
LEIA(salariobruto)

     SE(salariobruto <2112.01)ENTAO
         irrf <- 0
     SENAO
         SE(salariobruto <2826.66)ENTAO
           irrf <- 158.40
         SENAO
           SE(salariobruto <3751.06)ENTAO
             irrf <-  370.40
           SENAO
                SE(idade <4664.69)ENTAO
                 ENTAO irrf <- 651.73
                SENAO
                    irrf <- 884.96
                FIMSE
            FIMSE
           FIMSE
        FIMSE


     SE(salariobruto <1412.01)ENTAO
         inss <- salariobruto*0.075
     SENAO
         SE(salariobruto <2666.69)ENTAO
           inss <- salariobruto*0.09
         SENAO
           SE(salariobruto <4000.04)ENTAO
             inss <-  salariobruto*0.12
           SENAO
                inss <- salariobruto*0.14
            FIMSE
           FIMSE
      FIMSE

salarioliquido <- salariobruto - (inss + irrf)
ESCREVAL("------------------------LOADING----------------------")
ESCREVAL("Você recebe ",salarioliquido)
ESCREVAL("IRFF ",irrf)
ESCREVAL("INSS ",inss)


Fimalgoritmo
