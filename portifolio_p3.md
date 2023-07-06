- Aluno: Pedro Henrique de Deus Vieira
- Matricula: 190044055

# Introdução

Nessa terceira parte do portifólio, serão apresentados e discutidos tópicos principalmente sobre Satisfação de Condições, abordando temas sobre definição e estruturação de problemas, tipos de condições e outros. Além disso será apresentado também algoritmos para soluções de problemas definidos.

# Apresentação do Conteúdo

## Representação Atômica vs. Fatorada
Para entender sobre essas representações, é importante antes compreender o que seria um CSP . A sigla se remete a um tipo de problema chamado Constraint Satisfaction Problem (ou em português: Problemas de Satisfação de Condições (PSC)), no qual é possível descrever como um problema onde se está presente uma série de variáveis para serem analisadas, e cada uma dessas variáveis possuem um valor para satisfazer as condições das mesmas.

Serão analisadas duas representações para esses tipos de problemas, a Representação Atômica e a Fatorada, tais explicações de cada uma estão descritas abaixo:

- Representação Atômica

    A representação atômica é uma abordagem em que os problemas de satisfação de condições são representados em termos de variáveis e cláusulas. Nesse tipo de representação, cada variável representa uma propriedade ou condição específica, e as cláusulas são usadas para expressar as restrições entre as variáveis. Essas restrições são normalmente definidas por meio de conectivos lógicos, como "e" (AND) e "ou" (OR).
- Representação Fatorada

    Já representação fatorada possui uma abordagem que desmembra o problema em fatores independentes. Cada fator representa uma restrição específica do problema. Esses fatores podem ser combinados para formar uma representação conjunta do problema, que é então resolvida para encontrar uma solução válida.


## Definindo Problemas de Satisfação de Condições
Após uma breve passada sobre o que seriam os problemas de satisfação de condições, agora será explicado como funciona a definição de tais problemas.
Para início, é importante saber que um PSC envolve a atribuição de valores às variáveis de um conjunto X, representado por {X1, X2, ..., Xn}. Essas atribuições são do tipo Xi = Vi, Xj = Vj, onde cada variável Xi recebe um valor Vi de seu respectivo domínio.

Uma atribuição é considerada consistente ou legal quando não viola nenhuma das condições especificadas no conjunto C. Ou seja, todas as restrições impostas pelas condições são atendidas pela atribuição realizada. Por exemplo, se houver uma condição que restrinja que duas tarefas não possam ser realizadas simultaneamente, uma atribuição será consistente se atribuir valores às variáveis de forma que essa restrição seja respeitada.

Já uma atribuição completa é aquela em que todas as variáveis recebem um valor, ou seja, todas as variáveis do conjunto X possuem uma atribuição correspondente em uma solução em potencial. Uma solução para um PSC é considerada uma atribuição completa e consistente quando todas as variáveis possuem valores atribuídos que satisfazem todas as condições impostas.

Por outro lado, uma atribuição parcial ocorre quando algumas variáveis permanecem sem atribuições, ou seja, ainda não receberam um valor específico. Uma solução parcial, por sua vez, é uma atribuição parcial que é consistente, ou seja, respeita todas as condições especificadas até o momento.

Vale ressaltar que os problemas de satisfação de condições são, em geral, classificados como problemas NP-completos. Isso significa que encontrar uma solução ótima para um PSC pode ser extremamente desafiador, envolvendo um esforço computacional considerável, especialmente em problemas de grande escala.

Em resumo, um PSC lida com a atribuição de valores às variáveis de um conjunto X, garantindo que as atribuições sejam consistentes com as condições especificadas no conjunto C. Uma solução para um PSC é uma atribuição completa e consistente, enquanto uma atribuição parcial ou solução parcial envolve a falta de atribuição para algumas variáveis. Devido à sua complexidade computacional, os PSCs são considerados problemas NP-completos.

## Tipos de condições

Existem vários tipos de condições que podem estar envolvidos na definição de um PSC, dentre eles estão:

- Unárias: São condições que se aplicam a uma única variável. Elas definem as restrições internas de uma variável, como limites de domínio ou restrições específicas sobre os valores que uma variável pode assumir. 

- Binárias: São condições que envolvem duas variáveis. Elas estabelecem restrições entre pares de variáveis, especificando relações ou restrições mútuas entre elas.

- Ternárias: São condições que envolvem três variáveis.

- Globais: São condições que envolvem mais de duas variáveis. Elas especificam relações complexas entre várias variáveis do PSC.

Essas e outras podem ser encontras nos problemas, como exemplo as lógicas, condições de preferência e etc.

## Consistência

Consistência é um conceito bastante importante quando se trata em problemas de satisfação de condições. Refere-se à propriedade de uma atribuição de valores às variáveis de um PSC que respeita todas as condições impostas. Uma atribuição consistente é aquela em que nenhum dos valores atribuídos viola as restrições definidas pelas condições.

Algumas dessas consistências podem ser observadas abaixo:

- Consistência de Arco: 

É aplicada a pares de variáveis em um PSC.
Verificação: Envolve a verificação de todas as combinações possíveis de valores atribuídos a um par de variáveis para garantir que sejam consistentes com as restrições binárias entre elas.
Descarte de atribuições inconsistentes: Se uma atribuição violar alguma restrição binária, ela é considerada inconsistente e deve ser descartada.
Benefícios: Reduz o espaço de busca, eliminando atribuições inconsistentes desde o início do processo de resolução.
- Consistência de Trajeto: 

Também conhecida como consistência global, é uma forma mais abrangente de consistência em PSCs.
Verificação: Envolve a verificação de todas as combinações possíveis de valores atribuídos a um conjunto de variáveis, levando em consideração as restrições binárias e globais.
Garantia de respeito às restrições: Verifica se as atribuições respeitam todas as restrições impostas pelo conjunto completo de condições do PSC.
Desafios computacionais: A consistência de trajeto pode ser mais exigente computacionalmente, especialmente em problemas com grandes espaços de busca.

- Consistência K:

É uma forma mais restritiva de consistência que busca garantir a consistência de arco entre todos os pares de variáveis dentro de uma "vizinhança" de tamanho K.
Vizinhança: Uma vizinhança é definida como um subconjunto de variáveis que são relacionadas ou têm interações diretas.
Redução do espaço de busca: A consistência K permite eliminar atribuições inconsistentes em uma vizinhança específica, reduzindo ainda mais o espaço de busca.
Equilíbrio entre eficiência e abrangência: A escolha do valor K é um compromisso entre a abrangência da consistência e a eficiência computacional, pois um valor maior de K pode tornar a verificação mais demorada.

## Algoritmos
Um algoritmo bastante utilizado nos PSC's é o algoritmo AC-3.O objetivo principal dele é tornar as variáveis de um PSC consistentes com as restrições binárias impostas entre elas, simplificando os problemas de satisfação de condições. Ele faz isso, iterativamente, examinando pares de variáveis e removendo valores inconsistentes de seus domínios. O algoritmo percorre todos os arcos do PSC, onde cada arco representa uma restrição binária entre duas variáveis.

Ao aplicar o algoritmo AC-3, o espaço de busca é reduzido significativamente, pois os valores inconsistentes são eliminados dos domínios das variáveis. Isso evita a necessidade de considerar atribuições que seriam inconsistentes desde o início. Além disso, a consistência é propagada através dos arcos, permitindo eliminar valores inconsistentes em cascata.

## Estrutura de problemas

Problemas de satisfação de condições são frequentemente representados através de estruturas de problemas, que capturam as relações e restrições entre as variáveis e suas possíveis combinações de valores. Uma estrutura comum para representar um PSC é o uso de grafos em árvore.

Um grafo em árvore é uma estrutura de dados composta por nós (ou vértices) conectados por arestas (ou arcos). Essa estrutura é bem adequada para representar PSCs devido à sua natureza hierárquica, que reflete as relações entre as variáveis e suas dependências.

Na representação de um PSC por meio de um grafo em árvore, cada variável é representada por um nó do grafo. As arestas do grafo representam as relações entre as variáveis, geralmente refletindo as restrições binárias entre elas. Por exemplo, se existir uma restrição entre as variáveis X e Y, uma aresta será criada entre os nós correspondentes a X e Y no grafo em árvore. Essa representação em forma de grafo em árvore permite visualizar e compreender facilmente as dependências entre as variáveis. 

# Discussões

Após análises sobre problemas de satisfação de condições e seus respectivos princípios, é possível observar aplicações de PSC em várias áreas, dentre elas está a bioinformática.

Eles têm sido amplamente aplicados nessa área para resolver uma variedade de desafios relacionados ao processamento e análise de dados biológicos. Sua aplicação vêm permitindo modelar e resolver problemas complexos envolvendo sequências de DNA, estruturas de proteínas, interações genéticas e outros aspectos da biologia.

Um exemplo é a montagem de genomas, onde sua montagem envolve o processo de reconstruir a sequência completa de DNA de um organismo a partir de pequenos fragmentos de sequências conhecidas. Esse problema pode ser formulado como um PSC, onde as variáveis correspondem às posições dos fragmentos e as restrições especificam como esses fragmentos se sobrepõem e se combinam corretamente para formar o genoma completo.

# Projetos e Problemas
Vamos considerar um exemplo simples de um problema de satisfação de condições em que temos três variáveis: X1, X2 e X3, com os seguintes domínios: D1 = {1, 2, 3}, D2 = {4, 5}, D3 = {6, 7}. As condições que especificam as combinações permitidas de valores são as seguintes: X1 < X2 e X3 > X2.

Segue código python abaixo utilizando a abordagem de busca exaustiva:

```python

from itertools import product

# Definir os domínios
D1 = [1, 2, 3]
D2 = [4, 5]
D3 = [6, 7]

# Verificar todas as combinações possíveis
solutions = []
for x1, x2, x3 in product(D1, D2, D3):
    # Verificar as condições
    if x1 < x2 and x3 > x2:
        solutions.append((x1, x2, x3))

# Imprimir as soluções encontradas
for solution in solutions:
    print(solution)

```

E sua saída será

```python

(1, 4, 6)
(1, 4, 7)
(1, 5, 6)
(1, 5, 7)
(2, 4, 6)
(2, 4, 7)
(2, 5, 6)
(2, 5, 7)
(3, 4, 6)
(3, 4, 7)
(3, 5, 6)
(3, 5, 7)
```

Essas são todas as combinações de valores que satisfazem as condições especificadas. Cada linha representa uma solução válida para o PSC, onde o valor de X1 é menor que o valor de X2 e o valor de X3 é maior que o valor de X2.
# Conclusão

A matriz do tema aprensentado no documento foi sobre Problemas de Satisfação de Condições, passando pelos seus conceitos iniciais, entendo suas representações, seus tipos e as devidas definições para determinados tipos de cenários, foi possível perceber que é um importante processo para a contrução de inteligências artificiais e projetos de algoritmos como exemplo. 