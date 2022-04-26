# Raciocínio Automático em Situações de Incerteza e Imprecisão

# SUMÁRIO

- **[INTRODUÇÃO](#introdução)**
- **[MODULO 1](#modulo-1)**
- **[MODULO 2](#modulo-2)**
- **[MODULO 3](#modulo-3)**
- **[MODULO 4](#modulo-4)**


# INTRODUÇÃO
Neste Módulo, tem como objetivo resumir os conceitos de Representação de Conhecimento, Raciocínio Automático e Aprendizado.<br>
**Ele será resumido em topicos simples com base em alguns conceitos e atividades que constam no Conteúdo digital.**

# MODULO 1
- **[ATIVIDADES MOD 1](#atividades-mod-1)**
- **[CONCEITOS MOD 1](#conceitos-mod-1)**

## ATIVIDADES MOD 1



## CONCEITOS MOD 1
### Variaveis
- **Variaveis aleatorias bolenanas** - podem assumir o valor verdadeiro e falso.<br>
- **Variaveis aleatorias discretas** - composto por um conjunto de valores enumeráveis, uma possível variável aleatória discreta seria Tempo, em que os valores possíveis poderiam ser ensolarado, chuvoso, nublado e nevoeiro.<br>
- **Variaveis aleatorias continuas** - é formado por números reais compreendidos em um intervalo, de forma que entre quaisquer dois valores desse intervalo, há sempre uma quantidade infinita de valores.<br><br>
### Probabilidade
- **Probabilidade incondicional** - em resumo é o grau de crença (probabilidade) que se atribui a um fato, sem haver qualquer informação adicional sobre ele.<br>
- **Probabilidade condicional** - em resumo é o grau de crença (probabilidade) que se atribui a um fato e havendo alguma informação adicional (evidência) sobre ele.<br>
#### Probabilidade condicional - FORMULA
![image](https://user-images.githubusercontent.com/100146657/165290194-2b8762a3-57cc-43c5-adc7-06f50d96a131.png)

![image](https://user-images.githubusercontent.com/100146657/165290261-cfb81a23-520b-4730-8e14-44b71613b8f7.png)

**A PARTIR DESSAS EQUAÇÕES É POSSIVEL DERIVAR A EQUAÇÃO ABAIXO CONHECIDA COMO REGRA DE BAYERS**<br>
#### REGRA DE BAYERS (Regra Bayesiana) - FORMULA
![image](https://user-images.githubusercontent.com/100146657/165291391-6ad25b0a-25e5-40f6-ae0f-25af24333e7c.png)

**OBS.:** Essa formula é aplicada quando é invertida a ordem pois **b** depende de **a (a|b)**, mas no caso de inversão **b|a** é aplicada essa formula
#### INDEPENDENCIA
Para situações como essa, a probabilidade condicional é dada pela equação:

![image](https://user-images.githubusercontent.com/100146657/165291627-8f542bd3-518f-4402-8731-91a7c2b881f4.png)

**OBS.:** O sinal | significa dependencia EX: a|b - **b** depende de **a** para que ele ocorra ou assuma um valor logico (V ou F).x
Com isso, a **regra do produto** passa a ser definida conforme a equação:

![image](https://user-images.githubusercontent.com/100146657/165291644-aef5216d-ecd2-4801-ba36-e9faed4e7cd9.png)

### Inferência com distribuições conjuntas totais - EXEMPLO BASICO
Dada a tabela:

![image](https://user-images.githubusercontent.com/100146657/165291945-6eb72878-9fb5-4491-bfcf-bd18ddddf53e.png)

É possível calcular tanto probabilidades incondicionais quanto condicionais.

#### Probabilidades Incondicionais
![image](https://user-images.githubusercontent.com/100146657/165292124-a7163e1d-1f35-4631-9628-e5805e871676.png)

![image](https://user-images.githubusercontent.com/100146657/165292149-470c0270-bcca-4e01-82e7-f975a6b1fef5.png)

![image](https://user-images.githubusercontent.com/100146657/165292169-9f05a03d-04aa-4d18-8b85-960368adeb85.png)

#### Probabilidades Condicionais
![image](https://user-images.githubusercontent.com/100146657/165292266-b14715f3-c214-4722-b9e5-3b5eb37c8574.png)

### Inferência com a regra de Bayes - EXEMPLO
![image](https://user-images.githubusercontent.com/100146657/165292512-4fff10f1-6779-4dd6-b30a-df5ba15df0eb.png)

![image](https://user-images.githubusercontent.com/100146657/165292524-af0fa8d0-1abf-4d65-9c2c-3c0a33891d43.png)

![image](https://user-images.githubusercontent.com/100146657/165292536-04d6d67b-76d6-4f26-aaaa-2508a3d4c260.png)

#### Redes bayesianas (REDE DE BAYERS)
**Rede bayesiana** - é um grafo direcionado e acíclico, em que os nós representam as variáveis aleatórias tanto de evidência quanto de hipótese (diagnóstico), e as arestas representam as dependências que existem entre as variáveis.<br>


# MODULO 2
- **[ATIVIDADES MOD 2](#atividades-mod-2)**
- **[CONCEITOS MOD 2](#conceitos-mod-2)**

## ATIVIDADES MOD 2
![image](https://user-images.githubusercontent.com/100146657/164538297-2013c544-bebf-46f1-8a5f-2e23cf322f65.png)
![image](https://user-images.githubusercontent.com/100146657/164538304-27d1322e-b14e-407e-8a5e-b0fb361e2d67.png)
![image](https://user-images.githubusercontent.com/100146657/164538310-31da1eda-e8ea-4082-8787-ad27d3cdf2a5.png)
![image](https://user-images.githubusercontent.com/100146657/164538317-1a2ae9a9-eea3-471d-b7ef-378a8a514127.png)


## CONCEITOS MOD 2

**Sistemas especialistas** – Apoiam profissionais em que conhecimentos formais e adquiridos com experiência são fundamentais (pela entrada de dados por outros profissionais), o objetivo é apoiar na tomada de decisão potencializando o resultado dos profissionais com instrumentos que auxiliam aumentar a escalabilidade das soluções.
- **Componentes:**
   - **Motor de inferência**: É o mecanismo que contém as regras para resolver os problemas que fazem parte do escopo do sistema.
   - **Base de conhecimento**: É repositório de fatos, ou seja, é nele que estão todos os aspectos conhecidos e armazenados
   - **Interface de usuário**: É por meio desse componente que o usuário interage com o sistema
<br><br>

#### PROLOG:
> Primeiro é criado uma espécie de objeto (animal) em que ele recebe uma entrada (EX: cachorro) e após isso é denominada as características do objeto através de uma função nomeada pelo programador (EX: eh_fato_que()),  dentro da função é colocada as características.<br>
> **OBS.:** O símbolo **“:-”** significa o condicional **“SE”**

![image](https://user-images.githubusercontent.com/100146657/164539260-fefe2253-e627-4a1d-929f-1707077d1e5a.png)

> Após isso o programa é executado chamando a função criada em que Q é a entrada, ou seja, a característica, o format é para formatar o texto para apresentá-lo na tela e o read é apenas para continuar a perguntar.

![image](https://user-images.githubusercontent.com/100146657/164539352-ec27bdb9-bfcf-4301-8d6c-7fae28e8f8dd.png)

**Resultado:**
> Você digita **“animal(X).”**  como entrada e ele inicia o programa com as perguntas.

![image](https://user-images.githubusercontent.com/100146657/164539764-a8a07458-8f78-45da-b10e-42e2537cd3fe.png)

# MODULO 3
- **[ATIVIDADES MOD 3](#atividades-mod-3)**
- **[CONCEITOS MOD 3](#conceitos-mod-3)**

## ATIVIDADES MOD 3
![image](https://user-images.githubusercontent.com/100146657/164539986-730ae08e-f816-4962-a4a4-c4b7a9535cdd.png)
![image](https://user-images.githubusercontent.com/100146657/164539996-e7b582ca-38bf-4af4-adde-4ad5fdd606a3.png)
![image](https://user-images.githubusercontent.com/100146657/164540005-551331bb-22bb-4162-9618-54d5e171374b.png)
![image](https://user-images.githubusercontent.com/100146657/164540020-d5f0380c-206a-47fc-a274-a48122a24b99.png)


## CONCEITOS MOD 3
**Redes neurais artificiais** – são modelos computacionais baseados nos biológicos, composto por entradas e camadas no meio (camadas ocultas)<br>
**Pesos sinápticos** – importantes no processamento de entradas e reconhecimento de padrões <br>
**O bia**s – controla a rede <br>
**Junção de soma** – combina entrada e pesos através de um somatório <br>
**Função de ativação** - Produz uma determinada saída que é o que interessa.<br>
Para encontrar os pesos sinápticos é usada a **Função de Perda**:

![image](https://user-images.githubusercontent.com/100146657/164540125-a43ae6eb-e506-4771-9545-03524fa1b442.png)

Quanto mais próximo de 0 menos erros cometidos.


# MODULO 4
- **[ATIVIDADES MOD 4](#atividades-mod-4)**
- **[CONCEITOS MOD 4](#conceitos-mod-4)**

## ATIVIDADES MOD 4
![image](https://user-images.githubusercontent.com/100146657/164540318-ed8ce864-942d-413b-b676-00dbbf047fe8.png)
![image](https://user-images.githubusercontent.com/100146657/164540330-3fab40da-2c00-4d79-a19c-68ad8398105b.png)
![image](https://user-images.githubusercontent.com/100146657/164540335-cafdbc9a-ec8a-4117-9265-2948801a3254.png)
![image](https://user-images.githubusercontent.com/100146657/164540341-55a6bed0-b1c2-44d9-bf72-70bb886b82a7.png)

## CONCEITOS MOD 4
**Rede perceptron** – Objetivo de modelar como o cérebro humano processa dados visuais e aprendia a reconhecer padrões

### Regras de Aprendizado:
![image](https://user-images.githubusercontent.com/100146657/164540399-3893ccb5-a722-4428-a031-748b7be8b95c.png)
![image](https://user-images.githubusercontent.com/100146657/164540413-0632b0f5-98a8-4d17-a47b-7bd8bd3568ae.png)

> Peso já atualizado

![image](https://user-images.githubusercontent.com/100146657/164540451-58c56d22-0eba-4c84-b54c-5459aec2f3f5.png)

> Peso anterior

![image](https://user-images.githubusercontent.com/100146657/164540490-dd82967b-7de6-4c7b-9109-ff970ed62669.png)

> **regra de aprendizagem**, **Xi** – valor da entrada, **Yi** – Valor esperado obter, o **N** - taxa de aprendizagem<br><br>


![image](https://user-images.githubusercontent.com/100146657/164540684-69e3635a-11a9-4a83-9414-ec4243dddee6.png)

> O **d** é o valor obtido<br><br>

![image](https://user-images.githubusercontent.com/100146657/164540787-a0064b0e-6252-4808-9435-853579112854.png)

> Diferença do valor obtido (**d**) menos o valor Fornecido<br><br>

![image](https://user-images.githubusercontent.com/100146657/164540878-c510b2c2-d3a8-4d4b-81ca-30f3c3c2cf43.png)

> Calcula o peso fazendo além da diferença como o perceptron ele eleva ao quadrado<br><br>

**Backpropagation** – é a aplicação de todas as formulas, o principal método para treinar uma rede neural artificial de múltiplas camadas.



