- Nome: Pedro Henrique de Deus Vieira
- Matrícula: 190044055

# Introdução
O presente trabalho irá conter tópicos sobre o conteúdo de aprendizado de máquina, passando também por diversos exemplos de algoritmos e técnicas que aprofundam tal conhecimento, além disso, conceitos bastantes comentados hoje em dia como redes neurais e deep learning também serão devidamente conceituados.
# Apresentação do Conteúdo
## Aprendizado de Máquina
O aprendizado de máquina busca capacitar agentes a melhorarem seu desempenho por meio da observação e análise de dados. Nesse processo, um agente utiliza técnicas e algoritmos para extrair informações relevantes dos dados disponíveis, construindo um modelo que representa uma hipótese sobre o mundo e suas relações.

Para o processo de observação de dados,o agente coleta informações do ambiente em que está inserido, podendo ser dados estruturados ou não estruturados. Com base nos dados observados, o agente utiliza algoritmos e técnicas de aprendizado de máquina para construir um modelo. Esse modelo é uma representação simplificada e abstrata do mundo real, capturando os padrões e relações presentes nos dados. Uma vez que o modelo é construído, ele é utilizado como uma hipótese sobre o mundo. O agente faz uso do modelo para fazer previsões, tomar decisões ou resolver problemas.

O aprendizado de máquina desempenha um papel fundamental em nossa busca por capacitar as máquinas a aprenderem e se adaptarem em diferentes contextos. Existem várias razões pelas quais buscamos essa capacidade, e algumas delas são as seguintes:

Primeiramente, os designers não podem prever todas as possíveis situações futuras. À medida que o mundo evolui e novos desafios surgem, é difícil antecipar todas as circunstâncias que uma máquina pode enfrentar. Ao permitir que as máquinas aprendam, estamos capacitando-as a adquirir conhecimento com base em suas próprias experiências e a adaptarem-se a novas situações de forma autônoma.

Um exemplo prático disso é a utilização de robôs na bolsa de valores. O ambiente financeiro é altamente complexo e volátil, com inúmeras variáveis e interações em jogo. Ao permitir que os robôs aprendam com os dados do mercado, eles podem identificar padrões, tomar decisões rápidas e automatizadas, e otimizar as estratégias de investimento.

## Tipos de Aprendizado de Máquina
A seguir serão descritos alguns tipode aprendizado de máquina, são elas:

- Aprendizado Supervisionado: Nesse tipo de aprendizado, agente é treinado utilizando pares de entrada-saída conhecidos. O objetivo é aprender uma função que mapeie as entradas para as saídas desejadas. O agente observa os exemplos fornecidos, compreende os padrões e generaliza esse conhecimento para fazer previsões ou classificações em dados não vistos anteriormente.

- Aprendizado Não Supervisionado: O agente não recebe feedback explícito sobre as saídas desejadas. Em vez disso, ele busca identificar padrões e estruturas intrínsecas nos dados de entrada. Essa abordagem é útil para descobrir informações ocultas nos dados e segmentar conjuntos de dados complexos.

- Aprendizado por Reforço: O agente aprende a partir de um sistema de recompensas e punições. Ele interage com um ambiente dinâmico e recebe feedback em forma de recompensas ou punições com base em suas ações.

Esses três tipos de aprendizado de máquina fornecem uma base sólida para o desenvolvimento de sistemas inteligentes e adaptáveis, permitindo que as máquinas aprendam com dados e experiências para resolver problemas complexos e tomar decisões eficientes em uma variedade de contextos.

### Classificação e Regressão

No aprendizado de máquina, tanto na classificação quanto na regressão, o processo geralmente envolve etapas comuns, incluindo extração de características, pré-processamento e considerações sobre overfitting e underfitting. Seguem as etapas abaixo:

- Extração de Características: Envolve identificar e selecionar as informações relevantes dos dados de entrada que serão utilizadas para treinar o modelo. Essas características podem ser atributos específicos dos dados, como valores numéricos, categorias ou informações textuais.

- Pré-processamento: Envolve a aplicação de técnicas como limpeza dos dados, tratamento de valores ausentes, normalização, padronização e transformação de variáveis. Por exemplo, pode ser necessário remover ruídos dos dados, preencher valores faltantes ou converter dados categóricos em formatos numéricos adequados para o modelo.

- Overfitting e Underfitting: Overfitting ocorre quando um modelo se ajusta muito bem aos dados de treinamento, mas não consegue generalizar bem para novos dados. Isso pode acontecer quando o modelo é muito complexo ou quando há muito poucos dados de treinamento. Por outro lado, underfitting ocorre quando o modelo é muito simples e não consegue capturar corretamente os padrões e as relações nos dados. 

Ao passo que a extração de características e o pré-processamento são etapas comuns em vários problemas de aprendizado de máquina, o controle do overfitting e underfitting é uma consideração importante durante o treinamento do modelo, garantindo que ele seja capaz de fazer previsões precisas e confiáveis em novos dados.

## Algoritmos de Aprendizado Supervisionado

### K-Nearest Neighbors
O algoritmo K-Nearest Neighbors (k-NN) é um dos algoritmos mais simples e populares no aprendizado de máquina. Ele é frequentemente usado para problemas de classificação, mas também pode ser aplicado em problemas de regressão. O funcionamento básico do algoritmo é bastante intuitivo.

O processo de construção do modelo k-NN envolve apenas o armazenamento do conjunto de dados de treinamento. Não há uma fase explícita de treinamento como em outros algoritmos, como redes neurais ou árvores de decisão. O algoritmo memoriza todo o conjunto de dados de treinamento, que consiste em amostras com seus respectivos rótulos de classe ou valores de saída.
Ao fazer uma previsão para uma nova amostra, o algoritmo k-NN encontra os pontos mais próximos no conjunto de dados de treinamento, também conhecidos como "vizinhos mais próximos". A proximidade é determinada por uma medida de distância, geralmente a distância euclidiana. O valor de k, chamado de hiperparâmetro, determina a quantidade de vizinhos mais próximos que serão considerados.

### Modelos Lineares

Os modelos lineares são uma classe de algoritmos de aprendizado de máquina que fazem previsões utilizando uma função linear das características de entrada. Esses modelos são amplamente utilizados devido à sua simplicidade e interpretabilidade, além de serem eficazes em muitos cenários.

A forma geral dos modelos lineares é expressa pela seguinte equação:

y = w^T * x + b

Nessa equação, x[k] representa as características de uma amostra específica, w e b são parâmetros do modelo que são aprendidos durante o processo de treinamento e y é a previsão que o modelo faz para essa amostra.

A resposta prevista é calculada como uma soma ponderada das características de entrada, onde cada característica é multiplicada pelo seu peso correspondente. Os pesos, representados pelas entradas de w, determinam a importância relativa de cada característica na previsão do modelo. Esses pesos podem assumir valores positivos ou negativos, permitindo que o modelo capture tanto relações diretas quanto inversas entre as características e a variável de saída.

Além dos modelos lineares tradicionais, existem outros algoritmos de regressão que podem ser utilizados em diferentes situações. Vamos abordar dois deles: a regressão de Ridge e o Lasso.

A regressão de Ridge é uma extensão dos mínimos quadrados ordinários, em que os coeficientes (w) são escolhidos não apenas para melhor prever os dados de treinamento, mas também para minimizar a magnitude desses coeficientes. Essa abordagem visa evitar o overfitting, que ocorre quando o modelo se ajusta excessivamente aos dados de treinamento, tornando-se menos generalizável para novos dados. A regressão de Ridge utiliza a regularização L2, que adiciona uma penalidade proporcional ao quadrado da magnitude dos coeficientes. Isso tem o efeito de suavizar os coeficientes, tornando-os menores e mais estáveis. Dessa forma, a regressão de Ridge ajuda a controlar a complexidade do modelo, permitindo um equilíbrio entre ajuste aos dados de treinamento e generalização para novos dados.

Por outro lado, o Lasso (Least Absolute Shrinkage and Selection Operator) é um algoritmo que também restringe os coeficientes a serem próximos de zero, mas utiliza a regularização L1. Ao contrário da regressão de Ridge, o Lasso tem a capacidade de selecionar automaticamente um conjunto relevante de características, tornando alguns coeficientes exatamente iguais a zero. Isso implica em uma espécie de seleção de características automática, o que pode ser útil quando se lida com um grande número de características. O Lasso é particularmente eficaz quando há a presença de características redundantes ou irrelevantes, eliminando-as do modelo e ajudando a simplificar a interpretação.

### Classificadores Bayesianos Ingênuos
Os classificadores Bayesianos Ingênuos são uma família de classificadores que têm semelhanças com os classificadores por modelos lineares. No entanto, eles se destacam por sua eficiência no treinamento, sendo ainda mais rápidos do que os modelos lineares.
Uma das consequências dessa simplificação é que os modelos ingênuos de Bayes tendem a fornecer um desempenho de generalização inferior em comparação com os classificadores lineares. Isso ocorre porque a independência condicional nem sempre é uma suposição realista, já que características diferentes podem estar correlacionadas em muitos problemas reais. No entanto, mesmo com essa simplificação, os classificadores Bayesianos Ingênuos podem fornecer resultados satisfatórios em determinados contextos.
A eficiência dos modelos ingênuos de Bayes advém do fato de que eles aprendem parâmetros examinando cada característica individualmente e coletando estatísticas simples para cada característica, agrupadas por classe. Essas estatísticas podem incluir a contagem de ocorrências ou a média e o desvio padrão dos valores da característica em cada classe. Essas informações são usadas para calcular as probabilidades condicionais necessárias para fazer as previsões de classificação.
Existem três tipos mais comuns de classificadores Bayesianos Ingênuos, cada um adequado para diferentes tipos de dados:

- Gaussiano: É apropriado para dados contínuos, onde as características são representadas por valores numéricos. Ele assume que as características seguem uma distribuição gaussiana (também conhecida como distribuição normal).

- Bernoulli: Usado quando as características são binárias, assumindo apenas dois valores possíveis, geralmente representados por 0 e 1. Esse tipo de classificador é comumente aplicado em problemas de classificação de documentos ou análise de texto, onde as características podem representar a presença ou ausência de palavras-chave.

- Multinomial: É usado quando as características representam contagens inteiras, como a frequência de palavras em um documento ou o número de vezes que um evento ocorre. Ele assume uma distribuição multinomial, onde cada característica é modelada como uma variável aleatória discreta. 


## Redes Neurais e Deep Learning

A família de algoritmos conhecidos como redes neurais experimentou um ressurgimento significativo recentemente, especialmente sob o nome de "aprendizagem profunda" ou Deep Learning. O Deep Learning é uma abordagem poderosa e abrangente para o aprendizado de máquina, em que as hipóteses assumem a forma de circuitos algébricos complexos, conhecidos como redes neurais, com pesos de conexão ajustáveis.

Ao contrário de outros algoritmos de aprendizado de máquina, que dependem de características pré-definidas ou regras explícitas, o Deep Learning permite que a máquina aprenda automaticamente a partir dos dados brutos. As redes neurais são compostas por várias camadas de neurônios artificiais, cada uma realizando operações matemáticas simples. À medida que os dados passam pelas camadas, as informações são transformadas e refinadas, permitindo que a rede neural aprenda padrões e representações cada vez mais complexas.

Uma das principais vantagens do aprendizado profundo é sua capacidade de lidar com grandes volumes de dados e extrair características de forma automática e hierárquica. As redes neurais profundas podem aprender representações abstratas dos dados, permitindo que capturem características sutis e complexas. Isso torna o aprendizado profundo particularmente eficaz em tarefas como reconhecimento de imagens, processamento de linguagem natural, tradução automática, recomendação de conteúdo e muito mais.
No entanto, é importante notar que o aprendizado profundo geralmente requer um grande volume de dados de treinamento e poder computacional considerável. Além disso, o projeto e treinamento de redes neurais profundas exigem cuidado e atenção detalhada. Os algoritmos de aprendizado profundo são muitas vezes criados e ajustados de forma específica para cada caso de uso, levando em consideração as características dos dados, arquitetura da rede, hiperparâmetros e outras considerações.

Apesar dos desafios, o aprendizado profundo tem mostrado resultados impressionantes em uma ampla variedade de aplicações. Sua capacidade de aprender representações hierárquicas complexas e realizar tarefas sofisticadas tem impulsionado avanços significativos em áreas como visão computacional, processamento de linguagem natural, medicina, robótica e muito mais.

## Explainable Artificial Intelligence (XAI)​

O Explainable Artificial Intelligence (XAI), ou Inteligência Artificial Explicável, é um programa que busca desenvolver um conjunto de técnicas no campo do aprendizado de máquina com o objetivo de tornar os modelos mais explicáveis e compreensíveis para os usuários humanos, sem comprometer o desempenho de aprendizado.

A crescente complexidade dos algoritmos de inteligência artificial, como as redes neurais profundas, tem levado a um aumento na capacidade de previsão e tomada de decisão das máquinas. No entanto, esses modelos complexos geralmente são considerados como "caixas pretas" devido à falta de transparência em como eles chegam a suas conclusões. Isso cria um desafio para os usuários humanos que precisam entender e confiar nos resultados produzidos pelos sistemas de inteligência artificial.

## Algoritmos de Aprendizado Não Supervisionado
### K - Means Clustering

O algoritmo de clustering k-means é um dos métodos mais simples e amplamente utilizados para agrupamento de dados. Sua abordagem visa encontrar centros de cluster que sejam representativos de certas regiões dos dados.

O algoritmo pode ser dividido entre duas etapas, a primeira delas seria a atribuição, onde cada amostra do conjunto de dados é atribuída ao centro de cluster mais próximo. Os centros de cluster são representados por pontos no espaço multidimensional, sendo inicialmente definidos aleatoriamente ou usando outros métodos de inicialização. A segunda etapa consiste em atualizar os centros de cluster, nos quais cada centro é recalculado como a média das amostras atribuídas a ele na etapa anterior. Essa atualização é feita calculando a média das coordenadas de todas as amostras atribuídas ao centro de cluster específico.

O algoritmo k-means continua alternando entre essas duas etapas até que a atribuição das instâncias para os clusters não mude mais, ou seja, até que a convergência seja alcançada.

### Self-Organized Maps

Self-Organized Maps (SOM), também conhecidos como mapas auto-organizáveis ou mapas de Kohonen, foram introduzidos pelo professor finlandês Teuvo Kohonen na década de 1980. O SOM é uma técnica de aprendizado de máquina não supervisionado, que tem como objetivo mapear um conjunto de dados multidimensionais em uma grade bidimensional (2D) ou, em alguns casos, em uma grade tridimensional (3D) ou de dimensões superiores.

Para um Self-Organized Map (SOM) treinado, cada célula na grade possui um peso que representa uma função aprendida a partir de exemplos de treinamento que caíram na região. Esses pesos são ajustados durante o treinamento do SOM para capturar as características relevantes dos dados.

Uma propriedade do SOM é que células próximas umas das outras tendem a ter pesos semelhantes. Isso significa que exemplos semelhantes tendem a ser mapeados para uma vizinhança com valores de pesos similares. Essa organização topológica do SOM permite que o mapa represente as relações e padrões existentes nos dados de forma intuitiva.

Quando um novo exemplo de treinamento é inserido no SOM, é determinada a Unidade de Melhor Correspondência (BMU, do inglês Best Matching Unit). Isso é feito por meio de uma competição entre as células da grade. A BMU é a célula cujos pesos estão mais próximos do exemplo de treinamento em termos de distância euclidiana. Em outras palavras, a BMU é a célula que melhor representa ou "encaixa" o exemplo de treinamento dentro do SOM.

## Aprendizado por Reforço
### Q-Learning

O algoritmo Q-Learning é um dos algoritmos mais populares e amplamente utilizados no campo de aprendizado por reforço. Ele permite que um agente aprenda a tomar decisões em um ambiente dinâmico, visando maximizar a recompensa acumulada ao longo do tempo.

No Q-Learning, o agente aprende uma função chamada de função Q, ou função de qualidade. Essa função, denotada como Q(s,a), atribui um valor a cada par estado-ação, representando a soma das recompensas esperadas a partir do estado s se a ação a for tomada. A função Q é usada para guiar as decisões do agente, permitindo que ele escolha a ação que maximiza a recompensa futura esperada.

Durante o processo de aprendizado, o agente explora o ambiente interagindo com ele, realizando ações e observando o estado resultante e a recompensa associada. Com base nessa experiência, o agente atualiza a função Q, ajustando os valores dos pares estado-ação para melhor refletir as recompensas esperadas.


# Discussões
Um campo bastante interessante a ser discutido seria sobre Redes Neurais convolucionais e recorrentes, essas duas são arquiteturas populares de redes neurais que possuem características distintas e são adequadas para diferentes tipos de tarefas de aprendizado de máquina.

As redes neurais convolucionais são amplamente utilizadas em problemas de visão computacional, como reconhecimento de imagem e detecção de objetos. Essas redes são projetadas para extrair e aprender características hierárquicas de dados com estrutura de grade, como imagens. A arquitetura das delas inclui camadas convolucionais, que aplicam filtros de convolução para detectar padrões e características nas imagens, e camadas de pooling, que reduzem a dimensionalidade dos recursos extraídos. 

Já as redes recorrentes são projetadas para lidar com dados sequenciais ou temporais, como séries temporais, sequências de palavras ou música. A principal característica delas é que elas possuem conexões de realimentação, permitindo que informações anteriores sejam levadas em consideração ao processar dados subsequentes. Isso torna as RNNs adequadas para modelar dependências de longo prazo em sequências de dados. Essas redes possuem unidades de memória, como as células LSTM (Long Short-Term Memory) ou as células GRU (Gated Recurrent Unit), que são capazes de lembrar informações relevantes ao longo do tempo. Isso é especialmente útil em tarefas como tradução automática, geração de texto e análise de sentimento.

A diferença fundamental entre as redes convolucionais e as recorrentes está na sua capacidade de modelar dependências espaciais e temporais nos dados. As convolucionais são altamente eficazes em reconhecer padrões locais e invariantes de translação em dados estruturados em grades, enquanto as recorrentes são mais adequadas para capturar dependências de longo prazo em dados sequenciais.

No entanto, também existem casos em que essas duas arquiteturas podem ser combinadas. Essa combinação é conhecida como redes neurais convolucionais recorrentes (CRNNs), onde as camadas convolucionais extraem características espaciais das imagens, que são então fornecidas às camadas recorrentes para capturar dependências temporais em sequências de imagens ou vídeos. 
# Projetos e Problemas
Segue abaixo uma implementação de código utiliando processos de aprendizado de máquina, usando o conjunto de dados Iris para classificação.

```python
# Importar as bibliotecas necessárias
from sklearn import datasets
from sklearn.model_selection import train_test_split
from sklearn.neighbors import KNeighborsClassifier
from sklearn.metrics import accuracy_score

# Carregar um conjunto de dados para classificação (por exemplo, iris dataset)
iris = datasets.load_iris()
X = iris.data
y = iris.target

# Dividir o conjunto de dados em treinamento e teste
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

# Criar um modelo de classificação (por exemplo, K-Nearest Neighbors)
knn = KNeighborsClassifier(n_neighbors=3)

# Treinar o modelo com os dados de treinamento
knn.fit(X_train, y_train)

# Fazer previsões com os dados de teste
y_pred = knn.predict(X_test)

# Calcular a acurácia do modelo
accuracy = accuracy_score(y_test, y_pred)
print("Acurácia do modelo:", accuracy)

```
# Conclusão
Diversos conceitos foram abordados sobre o universo de aprendizado de máquina, algoritmos de classificação e análise sobre os dados foram mostrados para que se tenha um bom entendimento a cerca do conteúdo. Além disso, algoritmos a respeitos de um tópico sobre classificação para uma melhor perspectiva foram abordados. Esses e diversos outros tópicos se mostraram essenciais para um bom entendimento sobre IA's no geral para acomapnhar todo o desenvolvimento desse universo nos tempos modernos.