- Aluno = Pedro Henrique de Deus Vieira
- Matrícula = 190044055
# Introdução
 Para essa parte serão apresentados tópicos sobre Agente baseado em conhecimento, entendendo sua definição e como ele atua sobre o ambiente utiliando a lógica, na qual também será objeto de estudo. Suas regras e suas partes para a representação do raciocínio serão analisados no conteúdo, além disso será estudao o processo de inferência para um melhor entendimento da atuação de tal agente.
# Apresentação do Conteúdo

## Agente baseado em conhecimento

Um Agente Baseado em Conhecimento  é um tipo de agente que utiliza a lógica como uma classe geral de representações para a construção e aplicação de seu conhecimento. Esse agente é projetado para tomar decisões e executar tarefas de forma autônoma, com base em um conjunto de regras e fatos logicamente estruturados.

Esse agente atua de uma forma diferente sobre os já vistos anteriormente, nos quais possuem conhecimento de forma limitada e inflexível. O agente baseado em conhecimento constrói um modelo lógico do domínio em que opera. Esse modelo inclui uma linguagem de representação, que define o vocabulário utilizado para expressar fatos e regras, bem como as regras de inferência que governam o raciocínio lógico.

## Lógica
A lógica desempenha um papel fundamental na representação e no raciocínio dos agentes baseados em conhecimento. Ela fornece uma estrutura formal para expressar o conhecimento e realizar inferências válidas. A lógica utilizada por esses agentes pode ser dividida em duas partes principais: sintaxe e semântica.

A sintaxe define as regras e a gramática para a construção correta das expressões lógicas. Ela estabelece como os símbolos podem ser combinados para formar fórmulas bem formadas. Os símbolos básicos incluem constantes, variáveis, operadores lógicos e quantificadores.

A semântica está relacionada ao significado atribuído às expressões lógicas. Ela define como as expressões lógicas são interpretadas em termos de verdade e validade. A semântica estabelece um modelo de interpretação para as fórmulas lógicas, que consiste em atribuir valores de verdade aos símbolos e verificar se as fórmulas são verdadeiras ou falsas de acordo com o modelo.

## Processo de inferência

A inferência envolve o uso de regras de raciocínio lógico para derivar novas informações a partir das informações existentes. O agente aplica as regras de inferência de forma sistemática para deduzir conclusões lógicas a partir dos fatos e das regras presentes na sua base de conhecimento.

## Agente baseado em lógica proposicional

Nesse tipo de agente, a base de conhecimento é representada por meio de proposições, que são declarações ou afirmações que podem ser verdadeiras ou falsas. Cada proposição é geralmente representada por um símbolo ou uma variável proposicional.
As proposições podem ser combinadas usando conectivos lógicos, como o AND (E), OR (OU) e NOT (NÃO), para formar expressões lógicas mais complexas. O conectivo AND é utilizado para expressar a conjunção de proposições, o conectivo OR é usado para expressar a disjunção de proposições e o conectivo NOT é usado para negar uma proposição.

# Discussões

Várias aplicações padem ser analisadas dos agentes baseados em conhecimento, dentre eles está sobre diagnóstico médico, no envolve identificar doenças ou condições médicas com base em sintomas apresentados por um paciente. É um problema complexo que requer a análise de várias variáveis, como histórico médico do paciente, sintomas relatados, resultados de exames e conhecimento médico especializado.


# Projetos e Problemas

Segue abaixo um código simples em python representando um agente baseado em conhecimento atuando sobre o Wumpus World  e como ele percebe o ambiente, atualiar sua base de conhecimento e outros.

```python
class WumpusAgent:
    def __init__(self):
        self.knowledge_base = {}  # Base de conhecimento do agente

    def perceive(self, percept):
        # Atualiza a base de conhecimento com as percepções do ambiente
        position = percept['position']
        stench = percept['stench']
        breeze = percept['breeze']
        glitter = percept['glitter']

        self.knowledge_base[position] = {
            'stench': stench,
            'breeze': breeze,
            'glitter': glitter
        }

    def action(self):
        # Retorna a ação a ser tomada com base no conhecimento atual

        # Exemplo: Verifica se há brilho em uma posição e pega o ouro
        for position, knowledge in self.knowledge_base.items():
            if knowledge['glitter']:
                return 'grab'

        # Exemplo: Movimenta-se aleatoriamente caso não haja percepções
        return random.choice(['up', 'down', 'left', 'right'])


# Exemplo de uso do agente no ambiente do Wumpus World
agent = WumpusAgent()

# Loop principal do agente interagindo com o ambiente
while not game_over:
    percept = get_percept()  # Obtém as percepções do ambiente
    agent.perceive(percept)  # Atualiza o conhecimento do agente com as percepções
    action = agent.action()  # Decide a próxima ação a ser tomada
    perform_action(action)  # Executa a ação no ambiente
```



# Conclusão
Foram compreendidos conceitos e tópicos sobre agentes baseados em conhecimentos, nos quais constituem a capacidade de representar informações sobre o mundo, metas e contexto atual através de sentenças lógicas. Essa habilidade permite que esses agentes realizem inferências e tomem decisões de forma autônoma. Essa abordagem apresenta um avanço significativo em termos de autonomia, com ênfase em aprendizado e um maior nível de inteligência baseado não apenas em respostas reflexivas, mas também em raciocínio lógico e conhecimento adquirido.