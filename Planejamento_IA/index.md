# Planejamento em Inteligência Artificial

# SUMÁRIO

- **[INTRODUÇÃO](#introdução)**
- **[MODULO 1](#modulo-1)**
- **[MODULO 2](#modulo-2)**
- **[MODULO 3](#modulo-3)**
- **[MODULO 4](#modulo-4)**


# INTRODUÇÃO
Neste Módulo, tem como objetivo resumir os conceitos de Planejamento em Inteligência Artificial.<br>
**Ele será resumido em topicos simples com base em alguns conceitos e atividades que constam no Conteúdo digital.**

# MODULO 1
- **[ATIVIDADES MOD 1](#atividades-mod-1)**
- **[CONCEITOS MOD 1](#conceitos-mod-1)**

## ATIVIDADES MOD 1
![image](https://user-images.githubusercontent.com/100146657/164543259-f1c374f4-5209-4568-a82b-67569b69bd2b.png)
![image](https://user-images.githubusercontent.com/100146657/164543224-1328fbd1-2bd7-49d5-a71c-02f53dbf6b9a.png)
![image](https://user-images.githubusercontent.com/100146657/164543270-d2961cc2-9b0a-422c-9df5-4f1894624b85.png)
![image](https://user-images.githubusercontent.com/100146657/164543282-926a860b-a47d-4209-986b-d2dc41e93658.png)



## CONCEITOS MOD 1
### Sistema de transição de estado:

![image](https://user-images.githubusercontent.com/100146657/164543395-7c784dd4-adf0-428d-abbe-fea2409ebacd.png)

**Modelo conceitual para agente** – Esquema teórico que descreve de um determinado problema<br>
**Esquema teórico** – Modelo matemático que pode descrever tanto o agente quanto um ambiente ou planejamento<br>

**Sistema de Transição de Estados** - é uma tupla composta por 4 elementos
 
![image](https://user-images.githubusercontent.com/100146657/164543520-1f4fb5f2-830c-4482-89b3-b0ac5016eb0c.png)


**S** conjunto de estados possíveis <br>
**A** conjunto de ações<br>
**E** conjunto de eventos<br>
**Y** – função que leva um conjunto de estados que ao ser feita uma ação ou evento leva a outro conjunto de estados<br>
**Y = Sx(A U E) -> S**  

### Alguns tipos de Ambiente modelo Conceitual de Ambiente
**Totalmente Observável ou parcialmente** - Se o sensor de um agente tem acesso ao estado completo do ambiente em qualquer momento.<br>
**Determinístico ou estocástico** – O próximo estado ambiente é determinado pelo estado atual e ações executadas. Estocástico é o contrario<br> 
**Estático ou dinâmico** – Se o ambiente pode mudar enquanto o agente está em processo de deliberação. Dinâmico é o contrario <br>
**Discreto ou continuo** – Se há um número limitado de percepções e ações. Continuo é o contrario<br>
**Episódico ou sequencial** - Em um ambiente cuja ação do agente é episódica, a experiência do agente é dividida em episódios atômicos. Ou seja, um episódio não depende das ações tomadas no outro. Sequencial é o contrario<br>

MODELO conceitual para o planejamento

![image](https://user-images.githubusercontent.com/100146657/164543788-2f59ea85-ddb5-4df0-b14a-ea2e8fa3bae6.png)

O planejador recebe a descrição do sistema, ele tem o conhecimento do estado inicial e objetivos, e ele elabora planos que são fornecidos ao controlador que atua por meio de atuadores, que atuam no sistema, e as observações servem para caso uma ação não seja completamente realizadas, e há eventos que atuam sobre o sistema.

### Planejamento clássico

![image](https://user-images.githubusercontent.com/100146657/164543851-2b3830e5-06c2-4ec1-8a6e-66edf9bc8262.png)

# MODULO 2
- **[ATIVIDADES MOD 2](#atividades-mod-2)**
- **[CONCEITOS MOD 2](#conceitos-mod-2)**

## ATIVIDADES MOD 2
![image](https://user-images.githubusercontent.com/100146657/164544121-6ebd46d4-2c3d-4e96-a0c6-f2811819de9a.png)
![image](https://user-images.githubusercontent.com/100146657/164544130-672d9c32-3e8e-4a81-a909-c8f39f0db811.png)
![image](https://user-images.githubusercontent.com/100146657/164544136-55d40e5b-a224-4e8a-b740-4626a0bac85b.png)
![image](https://user-images.githubusercontent.com/100146657/164544145-79500237-8e89-4417-939f-2731c061d0a5.png)



## CONCEITOS MOD 2
**Heurísticas** – estratégias que diminuiem o tempo de tomada de decisão auxiliando na escolha rápida de valores para variáveis.<br>
**Busca Retroativa (Backtrancking)** – Aplicar heurística para reduzir o espaço de busca
- É estruturada em busca em profundidade
- Em cada nível da arvore um valor é atribuído a uma variável 
- Se não tiver como atribuir devido a uma restrição (heurística) ele volta um nível na arvore. (Backtraking)<br>

A verificação das restrições se chama -> Verificação prévia – **Forward Checking**<br>
O problema de achar atribuições de valores booleanos às variáveis de modo a tornar verdadeira uma fórmula é chamado de **SAT**.<br>
**SAT** é o problema de satisfação base e há diversos algoritmos que o resolvem (não de forma eficiente em relação à complexidade), aplicando diversas heurísticas.<br>



# MODULO 3 
- **[ATIVIDADES MOD 3](#atividades-mod-3)**
- **[CONCEITOS MOD 3](#conceitos-mod-3)**
- **[FUNÇÕES](#funções)**
- **[CODIGOS COMPLETOS](#codigos-completos)**

## ATIVIDADES MOD 3
![image](https://user-images.githubusercontent.com/100146657/164545029-e77d3d5b-4f31-409a-b079-2c526c8aa2f8.png)
![image](https://user-images.githubusercontent.com/100146657/164545034-cdd2dc6a-96c4-4142-ae72-e24d05b6e057.png)
![image](https://user-images.githubusercontent.com/100146657/164545046-4abb7094-a246-476d-aece-a52db92e9755.png)
![image](https://user-images.githubusercontent.com/100146657/164545055-46f507bd-79c5-4a2e-8ff2-06b99f0f91a3.png)
![image](https://user-images.githubusercontent.com/100146657/164545094-e82566a2-833e-4cf3-a53e-08a9b54c8bf9.png)

### CODIGO
```prolog
:- use_module(library(clpfd)).
puzzle([T,E,N,F,O,R,Y,S,I,X]) :-
     Variables = [T,E,N,F,O,R,Y,S,I,X],
     Variables ins 0..9, 
     all_different(Variables),
     (100*T + 10*E + N) +
     (100*T + 10*E + N) +
     (10000*F + 1000*O + 100*R + 10*T + Y) #= 
     (10000*S + 1000*I + 100*X + 10*T + Y), 
     O #\= 0, 
     label(Variables).
```

## CONCEITOS MOD 3
Impossível resumir a lógica do Prolog =(  😭 😭 😭<br>
Oque resta é rezar para ser igual ao material<br>
Vou tentar colocar os problemas da apostila e explica-los ao que parece se cair na AV1 vai ser igual a um desses problemas, ao final desse modulo colocarei os códigos por extenso.<br>
Caso queria rodar os códigos: [LINK](https://swish.swi-prolog.org/)<br>
Selecione program e rode a função no campo a direita<br>
![image](https://user-images.githubusercontent.com/100146657/164545413-4353006a-ec3e-4f1d-80df-8dd1cb7d8852.png)

## FUNÇÕES

### FUNÇÃO 1
![image](https://user-images.githubusercontent.com/100146657/164545593-2278eb0a-55bc-4e7e-b0ec-9fb26b74f0cb.png)
![image](https://user-images.githubusercontent.com/100146657/164545605-1c1c1e39-b8fc-43e4-a295-50abb48bb6ad.png)

Puzzle é só um nome aleatório criado para nomear uma função, assim como Variables que são variáveis aleatórias <br>
#### Linhas / descrição
**1** / Programa chama o modulo <br> <br>
**2** / O programa cria a função determinando algumas entradas<br> <br>
**3** / O programa cria uma variável para armazenar essas entradas<br> <br>
**4** / O programa restringe a variável que pode assumir números de 0 a 9 através da função ‘ins’ que se encontra na biblioteca declarada <br> <br>
**5** / O programa restringe a variável a cada valor ser diferente do outro através da função ‘ins’ que se encontra na biblioteca declarada<br> <br>
**6** / Agora ele começa a estruturar a formula conforme a imagem um, ele multiplica por valores de 10 e 100 para organizar em dezenas e no final insere a soma conforme a imagem 1 EX: 3*100 + 2*10 = 300 + 20 = 320<br> <br>
**7** / Continua a estruturar a formula conforme a imagem e no final ele usa o operador ‘#=’ indicando igualdade, se ele usasse o ‘=’ significaria atribuição, por isso o uso do #, essa função se encontra na biblioteca declarada<br> <br>
**8** / Finaliza a estruturação da formula conforme a imagem<br> <br>
**9** / Ele diz que S #\= 0 (S é diferente de 0) assim como o M, conforme a imagem um é perceptível o porquê dessa restrição, ao que parece a soma de S e M da eles mais algo como se fosse 5+6=11, eles acrescem mais uma casa decimal, ou seja eles tem que ser maior que 0, pois 9+0 é diferente de 10 ou valor superior<br> <br>
**10** / O label atribui o resultado as variáveis declaradas<br> <br>

### FUNÇÃO 2

Considere o seguinte exemplo de árvore genealógica

```prolog
/* Miguel é homem, etc*/
 homem(miguel).
 homem(arthur).
 homem(henrique).
 homem(pedro).
 homem(joao).
 homem(jose).
 /* Maria é mulher, etc*/
 mulher(maria).
 mulher(valentina).
 mulher(laura).
 mulher(larissa).
  
 /* Miguel é um dos pais de Laura*/
 pais_de(miguel,laura).
 pais_de(miguel,larissa).
 
 ```

Conforme a imagem ele declara um FATO que é uma espécie de objeto chamada ‘homem’, ‘mulher’ ou ‘pais_de ‘e basicamente os nomes dentro servem para quando a função for chamada mais a frente ele assumirá como verdadeiro caso o objeto assuma um valor que ele contenha <br>
**EX:** homem(Rodolfo) -> falso, pois não foi declarado o nome Rodolfo<br>
homem(miguel) -> verdadeiro, pois foi declarado o nome miguel<br>
Se for chamado homem(X) será apresentado todos os valores do conjunto<br>

```prolog
                         /* Regras */
 /* X é pai de Y, se X é homem e X é um dos pais de Y. 
  * Para isso, homem(X) deve ser verdade e pais_de(X,Y) deve ser verdade*/
 
 pai_de(X,Y):- homem(X),
     pais_de(X,Y).
 
 /* X é mãe de Y, se X é mulher e X é um dos pais de Y. 
  * Para isso, mulher(X) deve ser verdade e pais_de(X,Y) deve ser verdade*/ 
 mae_de(X,Y):- mulher(X),
     pais_de(X,Y).
 
 /* X é avô de Y, se X é homem e X é um dos pais de Z e Z é um dos pais de Y! 
  * Para isso, homem(X) deve ser verdade e pais_de(X,Z) deve ser verdade e pais_de(Z,Y) deve ser verdade*/ 
 avô_de(X,Y):- homem(X),
     pais_de(X,Z),
     pais_de(Z,Y).
 
  /* X é avó de Y, se X é mulher e X é um dos pais de Z e Z é um dos pais de Y! 
  * Para isso, mulher(X) deve ser verdade e pais_de(X,Z) deve ser verdade e pais_de(Z,Y) deve ser verdade*/ 
 avó_de(X,Y):- mulher(X),
     pais_de(X,Z),
     pais_de(Z,Y).
```
Logo em seguida é declarada as regras onde é colocado o nome da função, as entradas, o operador se e as ‘regras’ que tornam a função falsa ou verdadeira<br>


**EX:**
```
pai_de(X,Y):- homem(X),
     pais_de(X,Y).

pai_de -> função 
(X,Y) -> entradas
:- -> operador ‘se’
pais_de -> objeto (FATO)
(X,Y) -> entradas
A função pai de recebe o X que é o pai e Y que é o filho, se X é homem e X pai de Y, então pai de X, Y é verdadeiro.
A mesma lógica se aplica as outras funções.
```

### FUNÇÃO 3
Problema de coloração de mapas 
![image](https://user-images.githubusercontent.com/100146657/164546574-65874e2f-4170-4d28-a80d-9592c71583b2.png)
![image](https://user-images.githubusercontent.com/100146657/164546589-65170ca1-d4f2-4a20-acec-dd1a2b5a613b.png)

```prolog
coloring(A,B,C,D,E,F) :-
 different(A,B),
 different(A,C),
 different(B,C),
 different(B,D),
 different(C,D),
 different(C,E),
 different(C,F),
 different(D,E),
 different(E,F).
```
Nessa etapa ele já cria a função com valores de entrada de A até F<br>
E abaixo chama a função em que só retorna verdadeiro se for diferente, ele vai verificar linha a linha, <br>
Até que todas sejam satisfeitas
```prolog
different(vermelho,azul).
 different(azul,vermelho).
 different(vermelho,verde).
 different(verde,vermelho).
 different(verde,azul).
 different(azul,verde).
```
Aqui ele clara que é fato que uma cor seja diferente de outra, para que o programa entenda.<br>
Após rodar 

![image](https://user-images.githubusercontent.com/100146657/164546779-023948d0-8401-4755-b64c-d0bcffeebc68.png)

O programa irá listar todas as possibilidades que satisfazem a função de acordo com as restrições e fatos.

### FUNÇÃO 4
O problema das rainhas não entendi nada kkkk.
Se você quer entender, boa sorte. =)

### FUNÇÃO 5
Problema de restrição de domínio real

![image](https://user-images.githubusercontent.com/100146657/164546868-dd5e637b-2cf3-4054-b359-cdcd07ebe6b6.png)

```prolog
:- use_module(library(clpr)).
 sistema(X,Y,Z) :- {2*X+Y =< 16, X+2*Y =< 11,X+3*Y =< 15, Z = 30*X+50*Y}, maximize(Z).
```
O MESMO QUE
```prolog
:- use_module(library(clpr)).
 sistema(X,Y,Z) :- {2*X+Y =< 16,
                    X+2*Y =< 11,
                    X+3*Y =< 15,
                    Z = 30*X+50*Y}, maximize(Z).
```
Basicamente ele reescreveu o sistema no programa contendo as regras que ele necessitava.<br>
Caso rode o programa ele apresenta isso.

![image](https://user-images.githubusercontent.com/100146657/164547071-4c99e35f-2691-4463-949e-58d7955174e4.png)


## CODIGOS COMPLETOS
### FUNÇÃO 1

```prolog
:- use_module(library(clpfd)).
puzzle([S,E,N,D,M,O,R,Y]) :-
     Variables = [S,E,N,D,M,O,R,Y],
     Variables ins 0..9, 
     all_different(Variables),
     (1000*S + 100*E + 10*N + D) +  
     (1000*M + 100*O + 10*R + E) #= 
     (10000*M  + 1000*O + 100*N + 10*E + Y), 
     S #\= 0, M #\=0, 
     label(Variables).


```

### FUNÇÃO 2

```prolog
homem(miguel).
homem(arthur).
homem(henrique).
homem(pedro).
homem(joao).
homem(jose).

mulher(maria).
mulher(valentina).
mulher(laura).
mulher(larissa).
 
pais_de(miguel,laura).
pais_de(miguel,larissa).
pais_de(maria, laura).
pais_de(maria, larissa).
pais_de(arthur,pedro).
pais_de(valentina, pedro).
pais_de(laura, joao).
pais_de(henrique, joao).
pais_de(larissa, jose).
pais_de(pedro, jose).
 

pai_de(X,Y):- homem(X),
    pais_de(X,Y).
 
mae_de(X,Y):- mulher(X),
    pais_de(X,Y).

avô_de(X,Y):- homem(X),
    pais_de(X,Z),
    pais_de(Z,Y).

avó_de(X,Y):- mulher(X),
    pais_de(X,Z),
    pais_de(Z,Y). 
irma_de(X,Y):-
    mulher(X),
    pai_de(P, Y), pai_de(P,X),X \= Y.

irma_de(X,Y):- mulher(X),
    mae_de(M, Y), mae_de(M,X),X \= Y.

tia_de(X,Y):- mulher(X),
    pais_de(Z,Y), irma_de(Z,X),!.

irmao_de(X,Y):-
    homem(X),
    pai_de(P, Y), pai_de(P,X),X \= Y.

irmao_de(X,Y):- homem(X),
    mae_de(M, Y), mae_de(M,X),X \= Y.
   
tio_de(X,Y):-homem(X),
    pais_de(Z,Y), irmao_de(Z,X).
   
ancestral_de(X,Y):- pais_de(X,Y).

ancestral_de(X,Y):- pais_de(X,Z),
    ancestral_de(Z,Y).

```

### FUNÇÃO 3

```prolog
coloring(A,B,C,D,E,F) :-
 different(A,B),
 different(A,C),
 different(B,C),
 different(B,D),
 different(C,D),
 different(C,E),
 different(C,F),
 different(D,E),
 different(E,F).
 

 different(vermelho,azul).
 different(azul,vermelho).
 different(vermelho,verde).
 different(verde,vermelho).
 different(verde,azul).
 different(azul,verde).
            
```

### FUNÇÃO 4

```prolog
:- use_module(library(clpfd)).
n_queens(N, Qs) :-
        length(Qs, N), 
        Qs ins 1..N, 
        safe_queens(Qs),
    	label(Qs). 
safe_queens([]). 
safe_queens([Q|Qs]) :- 
        queens_not_attacking(Qs, Q, 1), 
        safe_queens(Qs). 
queens_not_attacking([], _, _).
queens_not_attacking([Q|Qs], Q0, D0) :- 
    	Q0 #\= Q, 
        abs(Q0 - Q) #\= D0, 
        D1 #= D0 + 1, 
        queens_not_attacking(Qs, Q0, D1).

```

### FUNÇÃO 5

```prolog
:- use_module(library(clpr)).
 sistema(X,Y,Z) :- {2*X+Y =< 16, X+2*Y =< 11,X+3*Y =< 15, Z = 30*X+50*Y}, maximize(Z).

```

# MODULO 4 - EM BREVE
- **[ATIVIDADES MOD 4](#atividades-mod-4)**
- **[CONCEITOS MOD 4](#conceitos-mod-4)**

## ATIVIDADES MOD 4


## CONCEITOS MOD 4






