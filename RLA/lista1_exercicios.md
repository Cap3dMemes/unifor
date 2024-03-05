

# **UNIFOR**
>**Disciplina**: Raciocínio logico algorítmico <br>
>**Orientador**: Prof. Ricardo Carubbi

## **Lista 1 Exercícios**
### Exercício 3
Represente, em fluxograma e pseudocódigo, um algoritmo para determinar se um número inteiro e positivo é par ou impar

#### Fluxograma

```mermaid
flowchart TD
A([INÍCIO]) --> B{{DIGITE UM NÚMERO:}}
B --> C[/NUMERO/]
C --> D{NUMERO > 0}
D --FALSE--> E{{O NUMERO DEVER SER POSITIVO!}}
E  --> J([FIM])
D --TRUE--> F([RESTO = NUMERO % 2])
F --> G{{RESTO == 0}}
G --NO--> H{{O NUMERO É IMPAR}}
G --YES--> I{{O NUMERO É PAR}}
H --> J
I --> J
```

```
ALGORITIMO verificar_par_ou_impar
DECLARE numero, resto INTEIRO
ESCREVA "Digite um numero"
LEIA numero 
SE numero >= 0 EANTAO
	resto = numero % 2 
	SE resto == 0 ENATO 
		ESCREVA "O numero é par!"
	SENAO 
		ESCREVA "O numero é impar!"
SENAO
	ESCREVA "O número deve ser positivo"
FIM_ALGORITIMO
```

