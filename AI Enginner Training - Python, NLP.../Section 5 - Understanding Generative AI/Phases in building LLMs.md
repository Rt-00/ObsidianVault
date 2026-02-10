Fases ao criar LLMs:

- Model Design 
- Dataset Engineering
- Pre-training
- Preliminary Evaluation
- Post-training
- Fine-tuning
- Final testing & Evaluation

No mundo real, esses estágios não são sempre sequenciais.

---

Model Design

Fase inicial que discutimos sobre o projeto do modelo, envolve estrategistas e desenvolvedores de IA que selecionam a arquitetura da rede neural a sem empregada. Por exemplo, eles podem escolher Transformers, CNNs, RNNs etc. Além disso, eles devem decidir sobre a profundidade do modelo, o número de camadas na rede neural e o total de parâmetros que ela conterá. As escolhas de arquitetura nesse estágio determinarão o escopo do trabalho e o que o modelo pode ou não fazer.

---

Dataset Engineering

Há um ditado popular entre os profissionais de dados que diz que um modelo é tão bom quanto os dados usados para construí-lo. A fase de engenharia do conjunto de dados é crucial, envolvendo a coleta, a limpeza e a estruturação dos dados de treinamento para o modelo. Há duas maneiras de obter dados para construir um modelo de IA:

- Extraia dados disponíveis publicamente da internet;
- Use dados proprietários.

 Mas poucas empresas possuem dados suficientes para criar um LLM com dados proprietários. Somente muitos estrategistas de IA, como Bernard Ma, concordam que as empresas que possuem mais dados proprietários provavelmente terão uma vantagem competitiva ao criar sistemas de IA.

É essencial que os desenvolvedores de IA envolvidos na engenharia de conjuntos de dados considerem as principais questões éticas, incluindo:

- Diversidade dos Dados (Data diversity) e a criacão de conjuntos de dados que abordem vários vieses;
- Ética dos dados (Data ethics)

---

Pre-training

Envolve o treinamento do modelo em um grande corpus de dados brutos da fase de Dataset Engineer. Durante o pré-treinamento, obtemos uma versão bruta do modelo.

Dependendo dos dados pré-treinamento, o modelo poderia fornecer saídas indesejáveis. Por exemplo, se a treinássemos com dados do fórum da internet, o modelo poderia fornecer respostas de saída contendo linguagem ofensiva, e diferentes vieses.

Além disso, podemos estar construindo um modelo que será usado para um domínio específico. E quando um modelo treinado em dados gerais precisa ser usado em uma indústria específica, precisamos adaptar suas saídas para atender às exigências especializadas do campo. 

Suponha que você está trabalhando em um chatbot de suporte ao cliente. Nesse caso, você quer treinar o chatbot para responder de uma forma amigável ao cliente que corresponda às expectativas dos clientes e ao serviço que eles usam ao falar com o pessoal de suporte ao cliente humano. 

Assim, os desenvolvedores de IA avaliam o desempenho preliminar do modelo e ganham uma ideia de suas capacidades. Assim que entenderem o que precisa ser melhorado, abordarão essas questões na fase pós-treinamento.

---

Post-training

O pós-treinamento consiste em duas etapas. Primeiro, desenvolvedores de IA usam ajuste fino supervisionado com dados de alta qualidade para melhorar o modelo pré-treinado.

No segundo passo, eles vão refinar o modelo incorporando feedback humano, como anotações.

---

Fine-tuning

Atualiza os pesos do modelo para melhorar sua qualidade e velocidade. Por exemplo, mudando pesos, podemos fazer um modelo menor e mais rápido, mais adequado para uma tarefa específica e menos capaz em geral de desempenho.

---

Final testing & Evaluation

Por fim, na fase final, novamente testamos e avaliamos o modelo. Desta vez, somos muito mais rigorosos e queremos colocar-nos no lugar do utilizador final. Pretendemos avaliar a qualidade da resposta do modelo, precisão, velocidade e crucialmente seu comportamento ético.