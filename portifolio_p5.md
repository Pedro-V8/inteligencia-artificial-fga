- Nome: Pedro Henrique de Deus Vieira
- Matricula: 190044055

# Introdução

...

# Apresentação do Conteúdo

## Incerteza
Lidar com incertezas é uma realidade constante para os agentes que enfrentam a tarefa complexa de resolver problemas em ambientes desafiadores. Essas incertezas podem surgir de diversas fontes, como a observabilidade parcial, o não determinismo e as adversidades, e exigem que os agentes adotem estratégias adaptativas para alcançar seus objetivos.

Tentar usar a lógica pura no contexto do diagnóstico médico é uma tarefa impraticável, e isso pode ser atribuído a três razões fundamentais.

Em primeiro lugar, a complexidade envolvida é imensa. Listar todas as condições anteriores e posteriores necessárias para criar regras sem exceções é um trabalho árduo e exaustivo. Além disso, a aplicação prática dessas regras se mostra extremamente desafiadora. O processo de análise e utilização das regras de forma coerente requer habilidades e conhecimentos avançados.

Em segundo lugar, a falta de uma teoria médica completa é uma barreira significativa. A ciência médica ainda não possui uma teoria abrangente que englobe todos os aspectos e nuances do campo. Existem lacunas de conhecimento e incertezas que dificultam a criação de um sistema lógico abrangente. Portanto, a aplicação de uma abordagem puramente lógica para o diagnóstico médico é limitada pelas próprias limitações do conhecimento científico atual.

Além disso, a ignorância prática é um fator que contribui para a inviabilidade de uma abordagem lógica estrita. Mesmo se tivermos conhecimento de todas as regras estabelecidas, ainda podemos estar incertos em relação a um paciente específico devido à falta de realização de todos os testes necessários ou à impossibilidade de realizá-los. Essa incerteza prática impede a aplicação de uma lógica pura e infalível no processo de diagnóstico médico.

Um exemplo ilustrativo dessa problemática é a relação entre dores de dente e cáries. Essa conexão não pode ser considerada uma consequência lógica estrita em ambas as direções. Ou seja, a lógica pura não é suficiente para estabelecer uma relação causal direta entre esses dois elementos no contexto médico. Existem diversos outros fatores e condições que podem estar envolvidos nessa relação complexa.

Essa realidade não é exclusiva do domínio médico, mas se aplica também a outros campos de julgamento, como direito, negócios, design, reparo automotivo, jardinagem, namoro, entre outros. Nessas áreas, as decisões não podem ser baseadas exclusivamente na lógica pura, devido à complexidade dos problemas, à falta de teorias completas e à incerteza prática inerente. É necessário adotar uma abordagem mais abrangente e flexível, que leve em consideração não apenas a lógica, mas também o conhecimento empírico, a intuição e a experiência.

## Utilidade
A teoria da utilidade, em sua essência, estabelece que todo estado, ou sequência de estados, possui um grau de utilidade para um agente específico. Essa utilidade representa o valor subjetivo que o agente atribui a cada estado, refletindo suas preferências individuais. Consequentemente, o agente tenderá a preferir estados com maior utilidade, uma vez que estes são considerados mais desejáveis.

É importante ressaltar que a utilidade de um estado é relativa ao agente em questão. Cada indivíduo tem suas próprias perspectivas, crenças e valores, o que influencia sua percepção da utilidade de um determinado estado. Portanto, a teoria da utilidade reconhece que as preferências e as avaliações de utilidade podem variar entre diferentes agentes, levando em conta a subjetividade inerente às preferências humanas.
## Teroria de Decisão
Baseada no princípio da utilidade máxima esperada (MEU), a teoria de decisão estabelece que um agente é considerado racional quando seleciona a ação que resulta na maior utilidade esperada. Essa ideia fundamental da teoria da decisão está intrinsecamente ligada à busca pela maximização da utilidade em um contexto de incerteza.

O princípio da utilidade máxima esperada se baseia na premissa de que nem sempre é possível prever com certeza os resultados de uma ação. No entanto, é possível estimar a probabilidade de ocorrência de cada resultado e atribuir uma utilidade a cada um deles. Com base nessas estimativas, o agente pode calcular a utilidade esperada, que é a média ponderada das utilidades dos resultados possíveis.

Portanto, um agente racional, de acordo com a teoria de decisão, avalia todas as ações possíveis, considerando suas consequências e as probabilidades associadas a cada resultado. Em seguida, o agente escolhe a ação que maximize a utilidade esperada, ou seja, aquela que, em média, produz o resultado mais desejável.

Esse princípio é especialmente útil em situações onde há incerteza ou risco envolvido. Ao ponderar as probabilidades e as utilidades esperadas, o agente pode tomar decisões informadas, buscando otimizar seus resultados no longo prazo.
## Independência e independência condicional
Ao determinar a independência de variáveis ou proposições, podemos alcançar uma notável redução na quantidade de informação necessária para especificar a distribuição conjunta completa.

Essa capacidade de decompor o conjunto completo de variáveis ​​em subconjuntos independentes é extremamente poderosa. Com essa divisão, a distribuição conjunta completa pode ser fatorada em conjuntos separados, cada um contendo apenas as variáveis ​​relevantes. Essa decomposição simplifica significativamente a representação do domínio e reduz a complexidade do problema de inferência.

Aproveitar proposições independentes é especialmente valioso quando se trata de lidar com problemas complexos de inteligência artificial. Ao identificar quais proposições são independentes entre si, podemos reduzir o tamanho da representação do domínio, o que resulta em uma representação mais eficiente e econômica do conhecimento.

Além disso, a independência de variáveis ​​ou proposições oferece uma série de benefícios práticos. Ela permite uma análise mais focada em partes específicas do problema, simplifica os cálculos envolvidos na inferência e contribui para a capacidade de generalização da IA.

## Regra de Bayes, aplicações e modelo ingênuo
A Regra de Bayes é um dos pilares fundamentais da teoria de probabilidade e desempenha um papel crucial na análise estatística e na tomada de decisões. Ela permite atualizar nossas crenças sobre um evento com base em evidências observadas.

A fórmula que data a regra e Bayes pode ser expressada na forma geral:

P(Y|X) = P(X|Y)P(Y) / P(X)

Porém também possui uma outra expressão, essa quando possui uma evidência "e" a ser considerada:

P(Y|X,e) = P(X|Y, e)P(Y, e) / P(X, e)

Para quantificar a relação causal, utilizamos a probabilidade condicional P(efeito|causa), enquanto a probabilidade condicional P(causa|efeito) descreve a direção diagnóstica. Isso é especialmente útil em tarefas de diagnóstico, em que temos informações sobre as probabilidades condicionais de relações causais.

Por exemplo, consideremos o caso de um médico que deseja diagnosticar uma doença em um paciente com base em seus sintomas. O médico possui informações sobre a probabilidade condicional de um paciente apresentar determinados sintomas dado que ele tem a doença (P(sintomas|doença)), e deseja determinar a probabilidade de o paciente ter a doença dado que ele apresenta esses sintomas (P(doença|sintomas)).

Vamos supor que o médico saiba que a meningite causa torcicolo em 70% dos casos, a probabilidade incondicional de qualquer paciente ter meningite é de 1/50.000 e a probabilidade incondicional de qualquer paciente ter torcicolo é de 1%.

Com base nessas informações, podemos usar a regra de Bayes para calcular a probabilidade de um paciente ter meningite dado que ele apresenta torcicolo.

Aplicando a fórmula da regra de Bayes, encontramos que a probabilidade é de 0,14%, ou seja, há uma expectativa de que 0,14% dos pacientes com torcicolo tenham meningite.

É importante notar que, embora o torcicolo seja um sintoma comum em pacientes com meningite (probabilidade de 0,7), a probabilidade de um paciente com torcicolo ter meningite ainda é baixa. Isso ocorre porque a probabilidade a priori do torcicolo (por qualquer causa) é muito maior do que a probabilidade a priori da meningite.

## Redes Bayesianas
Uma Rede Bayesiana, também conhecida como Rede de Bayes, é um grafo direcionado que combina informações probabilísticas para modelar o relacionamento entre variáveis aleatórias. A estrutura completa de uma Rede Bayesiana é definida da seguinte forma:

- Cada nó no grafo corresponde a uma variável aleatória, podendo ser discreta ou contínua, representando eventos ou estados do sistema em estudo.

- As arestas direcionadas conectam pares de nós, indicando a dependência probabilística entre eles. Se houver uma seta do nó X para o nó Y, diz-se que X é um genitor de Y, o que implica que a variável X influencia a variável Y.

- Elas são estruturadas como grafos acíclicos direcionados, também conhecidos como DAGs (Directed Acyclic Graphs).

- Cada nó Xi na Rede Bayesiana possui uma distribuição de probabilidade condicional associada θ(Xi|genitor(Xi)), que quantifica o efeito dos genitores na variável Xi. 

As Redes Bayesianas têm uma ampla aplicação em diversos campos, incluindo medicina, finanças, inteligência artificial e engenharia. Elas permitem modelar e representar de forma eficiente o conhecimento probabilístico e realizar análises sofisticadas, auxiliando na tomada de decisões em situações de incerteza.
## Inferência

A inferência exata em redes Bayesianas é uma tarefa fundamental em sistemas de inferência probabilística. Essa tarefa consiste em calcular a distribuição de probabilidade a posteriori para um conjunto de variáveis de consulta, com base em eventos observados.

Em outras palavras, quando temos uma rede Bayesiana e desejamos obter informações sobre um conjunto específico de variáveis, dado um conjunto de eventos observados, estamos interessados em calcular a distribuição de probabilidade a posteriori P(X|e).

Vamos considerar um exemplo prático, como o sistema de alarme contra roubo. Suponha que tenhamos uma rede Bayesiana que modela as relações entre as variáveis "Alarme", "Roubo", "John Ligou" e "Mary Ligou". Nesse caso, podemos fazer uma pergunta específica: qual é a probabilidade de um roubo ter ocorrido, dado que John ligou e Mary ligou?

Para responder a essa pergunta, aplicamos a inferência exata na rede Bayesiana. Utilizando os parâmetros de probabilidade condicional e as informações sobre as evidências (John ligou e Mary ligou), realizamos cálculos para obter a distribuição de probabilidade a posteriori desejada.

Essa inferência exata envolve a utilização de técnicas como a propagação da probabilidade e o algoritmo de eliminação de variáveis. Esses métodos permitem que a rede Bayesiana calcule de forma eficiente a distribuição de probabilidade a posteriori, considerando as dependências probabilísticas entre as variáveis e as evidências disponíveis.

## Tempo e Incerteza 
Para o estudo de Tempo e Incerteza, serão considerados dois tipos de problemas: estáticos e dinâmicos.

- Problemas estáticos: o estado das variáveis em análise permanece inalterado ao longo do tempo, independentemente do tempo que levarmos para fazer o diagnóstico ou tomar uma ação. 

- Problemas dinâmicos: o estado das variáveis muda ao longo do tempo, introduzindo incerteza e complexidade. 


## Estados e Observações
No contexto de problemas de tempo discreto, as noções de estados e observações desempenham um papel importante na modelagem probabilística.

Vamos considerar que estamos lidando com amostras temporais enumeradas como 0, 1, 2, ... Nesse caso, o intervalo entre as amostras é considerado constante, como por exemplo, 1/30 segundos. Essa definição do intervalo entre as amostras nos permite estabelecer uma estrutura temporal para o nosso modelo probabilístico.

Cada amostra temporal em um modelo de probabilidade de tempo discreto contém um conjunto de variáveis aleatórias. Essas variáveis podem ser observáveis ou não observáveis. Algumas variáveis são medidas diretamente ou observadas no momento da amostragem, enquanto outras variáveis podem não ser diretamente observáveis e podem requerer inferências ou cálculos para estimar seus valores.

Para simplificar o modelo, supomos que o mesmo subconjunto de variáveis seja observável em cada amostra temporal. Isso significa que as mesmas variáveis estão disponíveis para observação em todas as amostras temporais. Essa suposição facilita a análise e a modelagem probabilística, pois permite que trabalhemos com as mesmas informações em cada momento do tempo.

Ao considerar estados e observações, podemos pensar nas variáveis observáveis como representando o estado atual do sistema na amostra temporal específica. Essas variáveis fornecem informações diretas e concretas sobre o estado do sistema naquele momento.

Por outro lado, as variáveis não observáveis podem representar aspectos ocultos ou latentes do sistema. Essas variáveis podem ser inferidas ou estimadas com base nas variáveis observáveis e nas relações probabilísticas modeladas.
## Modelo de transição e modelos de sensores
Após definirmos o conjunto de variáveis de estado e evidência para um determinado problema, o próximo passo é especificar como o mundo evolui (o modelo de transição) e como as variáveis de evidência recebem seus valores (o modelo de sensor).

- Modelo de Transição: descreve a maneira como as variáveis de estado evoluem ao longo do tempo. Ele especifica a distribuição de probabilidade das variáveis de estado mais recentes, levando em consideração os valores anteriores.

- Modelo de Sensores: descreve como as variáveis de evidência recebem seus valores. Ele especifica a relação probabilística entre as variáveis de estado e as observações realizadas. É fundamental para a fusão das informações das observações com as estimativas do estado atual, permitindo a atualização da distribuição de probabilidade a posteriori.

Os modelos de transição e de sensor são componentes essenciais na modelagem probabilística. O modelo de transição descreve a evolução das variáveis de estado ao longo do tempo, levando em consideração valores anteriores, enquanto o modelo de sensor descreve como as variáveis de evidência recebem seus valores. A suposição de Markov permite simplificar a modelagem, assumindo que o estado atual depende apenas de um número fixo finito de estados anteriores. Esses modelos são fundamentais para realizar a inferência probabilística e atualizar as estimativas do estado atual com base nas observações disponíveis.

## Inferência em modelos temporais:
É possível identificar várias tarefas fundamentais que devem ser resolvidas no contexto de exploração e extração de informações de dados sequenciais utilizando inferência em modelos temporais, dentre as tarefas estão:

- Filtragem:  o objetivo é computar o estado de crença atual, ou seja, a distribuição a posteriori do estado mais recente, levando em consideração todas as evidências observadas até o momento. Essa distribuição, representada por P(Xt|e1:t), fornece uma estimativa atualizada do estado do sistema com base nas informações disponíveis.

- Predição: calcular a distribuição a posteriori de um estado futuro, levando em consideração todas as evidências observadas até o momento atual. Em outras palavras, queremos estimar a distribuição P(Xt+k|e1:t) para um valor k maior que zero, representando um ponto no futuro.

- Suavização: computar a distribuição a posteriori de um estado passado, dadas todas as evidências observadas até o momento atual. Essa distribuição é representada por P(Xk|e1:t), onde k representa um ponto no passado, em que 0 ≤ k < t. A suavização permite obter uma estimativa refinada do estado em momentos anteriores com base nas informações posteriore

- Explicação:  encontrar a sequência de estados que mais provavelmente gerou essas observações. Em outras palavras, desejamos calcular o argmaxx1:t P(x1:t|e1:t), onde x1:t representa a sequência de estados e e1:t é a sequência de observações. 

- Aprendizado: envolve a atualização dos parâmetros e estrutura do modelo com o objetivo de melhor representar os dados e melhorar a capacidade de inferência.


## Modelo Oculto de Markov
O modelo oculto de Markov, conhecido como HMM (hidden Markov model) em inglês, é um modelo probabilístico temporal que descreve o estado de um processo por meio de uma única variável aleatória discreta.

Nesse modelo, os valores possíveis da variável representam os estados possíveis do sistema ou do mundo em análise. Por exemplo, considere o "mundo do guarda-chuva". Nesse caso, o estado do tempo pode ser representado pela variável "chuva". O HMM é adequado para modelar esse tipo de processo, em que há uma única variável de estado que descreve o estado oculto do sistema.

No entanto, mesmo que o modelo possua duas ou mais variáveis de estado, ainda é possível utilizar o HMM combinando essas variáveis em uma única "megavariável". Essa megavariável é construída de forma a conter todas as possíveis combinações de valores das variáveis de estado individuais. Essa abordagem permite representar de maneira eficiente o espaço de estados complexo resultante da combinação de múltiplas variáveis.

Embora os HMMs exijam que o estado seja representado por uma única variável aleatória discreta, não há restrição quanto às variáveis de evidência no modelo.

Diferentemente das variáveis de estado, as variáveis de evidência são sempre observadas e não precisam ser modeladas como variáveis aleatórias. Isso ocorre porque, no HMM, as observações são diretamente observáveis, o que significa que não há necessidade de acompanhar uma distribuição de probabilidade sobre seus valores.

As variáveis de evidência podem ser qualquer tipo de informação observável e relevante para o modelo, como dados sensoriais, sinais acústicos, palavras em um texto, imagens, entre outros. Essas observações são utilizadas para auxiliar na inferência sobre o estado oculto do sistema, permitindo a estimativa dos estados em um determinado momento ou até mesmo a previsão de estados futuros.

Essa flexibilidade em relação às variáveis de evidência torna o HMM uma estrutura bastante versátil, capaz de lidar com diferentes tipos de dados observáveis em diferentes domínios de aplicação. É possível adaptar o modelo para acomodar diferentes tipos de variáveis de evidência, desde que as informações observáveis sejam relevantes para a inferência sobre o estado oculto.
## Filtros de Kalman 
O Filtro de Kalman é um algoritmo de estimação de estados ótimo amplamente utilizado em várias áreas, como sistemas de navegação, piloto automático, visão computacional e processamento de sinais. Esse filtro foi desenvolvido por Rudolf E. Kálmán, um renomado matemático e engenheiro, e seu trabalho foi publicado em 1960.

Vamos entender como o filtro de Kalman funciona através de um exemplo. Suponha que você esteja monitorando a localização do seu carro. Para isso, você utiliza uma combinação de sensores disponíveis no veículo, como IMU (Inertial Measurement Unit), que mede a aceleração e a velocidade angular do carro, hodômetro, que fornece a posição relativa do veículo, e GPS, que oferece a posição absoluta.

O objetivo é obter uma estimativa precisa e confiável da localização atual do carro, levando em consideração as informações coletadas pelos diferentes sensores. É nesse ponto que o filtro de Kalman entra em ação. Ele é capaz de combinar as informações dos sensores, considerando suas incertezas e características, para produzir uma estimativa otimizada do estado atual do sistema, no caso, a localização do carro.

O filtro de Kalman utiliza uma abordagem recursiva, ou seja, a estimativa é atualizada a cada nova medição disponível. Ele estima o estado atual com base no estado anterior e na nova observação. O algoritmo leva em consideração tanto a dinâmica do sistema quanto as incertezas associadas às medições dos sensores.

Uma das aplicações pioneiras do filtro de Kalman foi na missão Apollo 11, que levou o homem à lua. O filtro de Kalman foi utilizado para estimar com precisão as trajetórias do foguete e dos módulos espaciais, considerando as incertezas das medições e do ambiente espacial. Esse exemplo ilustra a capacidade do filtro de Kalman de lidar com sistemas complexos e desempenhar um papel crucial em aplicações críticas.

# Discussões

...

# Projetos e Problemas
...
