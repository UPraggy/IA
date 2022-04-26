# Raciocínio Automático em Situações de Incerteza e Imprecisão

# SUMÁRIO

- **[INTRODUÇÃO](#introdução)**
- **[MODULO 1](#modulo-1)**
- **[MODULO 2](#modulo-2)**


# INTRODUÇÃO
Neste Módulo, tem como objetivo resumir os conceitos de Representação de Conhecimento, Raciocínio Automático e Aprendizado.<br>
**Ele será resumido em topicos simples com base em alguns conceitos e atividades que constam no Conteúdo digital.**

# MODULO 1
- **[ATIVIDADES MOD 1](#atividades-mod-1)**
- **[CONCEITOS MOD 1](#conceitos-mod-1)**

## ATIVIDADES MOD 1
![image](https://user-images.githubusercontent.com/100146657/165299375-48ee3ed7-a87f-4b99-b5e2-eace54184d23.png)
![image](https://user-images.githubusercontent.com/100146657/165299929-50790840-1197-4bd6-a902-fda773f33eab.png)
![image](https://user-images.githubusercontent.com/100146657/165300158-55afc623-1926-4f26-81f3-eac1a7237a59.png)
![image](https://user-images.githubusercontent.com/100146657/165300182-3ee75c42-fd81-44a2-8188-71d23f8477b8.png)

Nessa etapa ele chegou a formula em que **Grama molhada (G)** depende de **Chuva (C)**

![image](https://user-images.githubusercontent.com/100146657/165300346-d2d9db69-828c-492e-83ba-78b9fc1757a3.png)

Como o problema não cita o Regador (R), ele é "descartado" das operações<br>
Esse "descarte" ver em forma de soma como afirmação do **r** de um lado da soma e negação do **r** no outro lado.
Assim ele começa a fazer a devida analise e operações na tabela.

![image](https://user-images.githubusercontent.com/100146657/165300653-3b64d9ff-232c-4f6b-bd97-cebbac258e1a.png)
![image](https://user-images.githubusercontent.com/100146657/165300676-ad5a3dfe-a95c-4365-bc67-7180c8511ee7.png)

Assim como acima no numerador no denominador, não é diferente, a operação de "descarte" também é feita, porém com o **r** e o **c**,
pois oque queremos agora é apenas o **g**

![image](https://user-images.githubusercontent.com/100146657/165301577-ef4e61b1-bacb-49e2-9efd-ae28b3eecd64.png)
![image](https://user-images.githubusercontent.com/100146657/165301645-25db8fef-2d2e-4410-b181-c59d9badad7d.png)
![image](https://user-images.githubusercontent.com/100146657/165301675-9db6f90f-fb25-466c-9ae9-d11d4534f617.png)
![image](https://user-images.githubusercontent.com/100146657/165301716-c60878b6-64de-453a-8f0d-47cf5a87f171.png)

Ao final é verificado:

![image](https://user-images.githubusercontent.com/100146657/165301805-51ae714d-86b5-40c1-86bc-e21dbdfd0bd1.png)

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
**OBS.:**
![image](https://user-images.githubusercontent.com/100146657/165299751-dac5215f-42f6-4c6d-bf00-c4f810bede5f.png)

![image](https://user-images.githubusercontent.com/100146657/165299476-1d1d7bed-4d7c-4c40-9c78-9392846c151e.png)

A cada P é necessario verificar a condicão ex: **c|a** que valor **c** assume quando a for **V**

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


