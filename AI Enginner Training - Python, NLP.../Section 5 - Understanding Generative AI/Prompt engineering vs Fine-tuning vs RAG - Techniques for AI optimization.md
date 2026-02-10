Quero resumir três conceitos cruciais de IA Gen nesta lição.

- Prompt Engineering
- RAG
- Fine-tuning

Todas as três técnicas melhoram a precisão e eficácia de resposta de uma LLM em cenários específicos, visando diferentes aspectos da funcionalidade de IA.

---

Prompt Engineering

O Prompt Engineering é quando explicamos ao modelo como se comportar, ou que contexto considerar. Nós não mudamos nenhum de seus pesos ou adicionamos novos dados. 

Usamos instruções e fornecemos exemplos verbais, explicando a saída desejada que queremos obter. 

Isso é bastante fácil de fazer, e a melhor parte é que podemos refinar consistentemente nossos prompts através de múltiplas iterações para alcançar saídas de IA satisfatórias. É importante notar que o modelo não muda. Apenas se adapta às nossas instruções verbais.

---

 Retrieval-Augmented Generation ou Geração Aumentada por Recuperação (RAG) é outra técnica que não altera os pesos do modelo. 
 
 Com R-A-G, anexamos um banco de dados ao modelo, que pode ser usado como biblioteca para contexto expandido. 
 
 Este método fornece significativamente mais exemplos de como o modelo pode ser usado para aprender a executar otimamente.

---

Fine-tuning

Tornar um LLM mais inteligente ou rápido é improvável sem modificar seu peso. Essa tarefa complexa requer treinamento adicional para um modelo já treinado. Este processo é conhecido como Fine-tuning. 

Às vezes, são necessários dados extras para conduzir o Fine-tuning. Além disso, Fine-tuning pode ser computacionalmente caro, e não podemos usar um processo iterativo como Prompt Engineer ou RAG. 

Um exemplo que irá esclarecer ainda mais as coisas: Desde a introdução do GPT, nossa equipe está ansiosa para explorar produtos utilizando um LLM. Eventualmente desenvolvemos um simulador de entrevista baseado no GPT. 

Se nós retreinássemos o modelo GPT e atribuíssemos novos pesos para torná-lo mais leve e rápido, para dar respostas aos usuários mais rápido, isso teria sido Fine-tuning. 

Nós não podíamos fazer isso porque o ajuste fino do OpenAI era um programa experimental inacessível a todos os desenvolvedores durante a construção de ferramentas. 
Mas mesmo que estivesse disponível, não se encaixa no nosso caso de uso, porque queremos criar um bot de entrevista que possa generalizar bem e adaptar-se às circunstâncias em mudança durante uma entrevista. 

O objetivo foi potencializar o modelo, integrando um banco de dados de perguntas de entrevistas amostrais, proporcionando contexto para consultas personalizadas com base no tipo de entrevista selecionado pelos usuários. Isso levou à incorporação do RAG, com múltiplos ajustes feitos ao banco de dados durante o desenvolvimento do aplicativo com base no desempenho do modelo.

A fase de Prompt Engineer foi a mais demorada. Tivemos que instruir o modelo sobre a exibição de questões de código, os tipos de consultas para várias etapas da entrevista, avaliar os alunos posteriormente, o tom de comunicação, acompanhar as respostas e outros aspectos.