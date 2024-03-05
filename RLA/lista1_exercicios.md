# **UNIFOR**
Disciplina: **Raciocínio Lógico algorítmico**
**Orientador:** Prof. Ricardo Carubbi

## **LISTA 1 DE EXERCÍCIOS**

### **Exercício 03**
Represente em fluxograma e pseudocódigo, um algoritmo para determinar se um número inteiro e positivo é par ou ímpar. 

#### **Fluxograma**

```mermaid
flowchart TD
A([INICIO]) --> B{{Digite 1 número:}}
B --> C[/número/]
C --> D{numero > 0}
D --NÃO--> E{{O número deve ser positivo! }}
E --> J
D --SIM-->F[resto = número % 2]
F --> G{resto == 0}
G --NAO--> H{{O número é impar!}}
G --SIM--> I{{O número é par!}}
H --> J([FIM])
I --> J
E --> J
```



```
ALGORITMO verifica_par_impar
DECLARE numero, resto INTEIRO
ESCREVA "Digite um número:"
LEIA  numero
SE numero > 0 ENTAO	
    resto = numero % 2
    SE resto == 0 ENTAO
       ESCREVA  "O número é par!"
   SENAO	
       ESCREVA "O número é ímpar!"	
   SENAO 
        ESCREVA "O numero deve ser positivo!"
 FIM             

