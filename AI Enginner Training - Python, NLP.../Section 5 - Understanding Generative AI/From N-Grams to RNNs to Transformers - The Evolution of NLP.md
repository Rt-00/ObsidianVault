
A primeira técnica: N-Grams. É um elemento fundamental para a modelação da linguagem. A ideia é simples, podemos estimar a probabilidade de uma palavra com base nas n palavras anteriores menos uma. Assim num n-gram com n igual a 1, chamado unigrama, um menos um seria zero. Representação?

```
n = 1('unigram') -> 1 - 1 = 0
```

Isso significa que a previsão não se baseia em nenhum contexto.

Vejamos como isso funciona. Temos a seguinte frase e o objetivo é prever a palavra final:

**My favorite sport is basketball**

O modelo n-gram funciona por não utilizar nenhuma palavra da frase em questão e ainda assim conseguir prever a palavra "basquetebol". Ao invés disso, analisa todo o texto e procura a palavra que aparece mais vezes. Assumindo que a palavra com a maior frequência é a melhor aposta para preencher o espaço em branco na frase. Assim, o modelo unigrama pode prever palavras comuns como "o" ou, "e", independentemente do seu ajuste efetivo com as palavras anteriores na frase. Mas se `n=2`, chamado bigrama, a previsão do basquete depende apenas da palavra anterior:

```
n = 2('bigrama') -> 2 - 1 = 1

Na frase em questão irá analisar: "is"
```

O mesmo se aplica a um trigrama:

```
n = 3('trigrama') -> 3 - 1 = 2

Na frase em questão irá analisar: "sport is"
```

O seu objetivo é simplesmente otimizar as previsões com base nas frequências de aparecimento nos dados de treino.

---

Redes Neurais

As redes neurais são, sem dúvida, um grande passo em frente. As redes neurais recorrentes, ou RNNs, são redes neurais que funcionam melhor com texto. Um dos principais pontos fortes das RNNs é a sua capacidade de reter informações de etapas anteriores da rede neural. A análise das palavras anteriores numa frase ajuda a rede RNN a decidir qual a palavra seguinte. Trata-se de um avanço considerável em comparação com os modelos de N-gramas, porque a ordem e o contexto dos pontos de dados são cruciais quando se lida com a linguagem. O principal desafio das RNN é sua dificuldade em lidar com textos grandes, uma vez que tendem a perder informação anterior com segmentos de textos progressivos. Este problema é designado por problema do gradiente de fuga. Para resolver este problema, os cientistas de IA desenvolveram redes de memória de curto prazo ou LSTM. Os LSTM melhoram os modelos de RNN tradicionais, introduzindo uma arquitetura de porta (Gate architecture) para escolher a informação a reter e a descartar. Isso permite que a rede mantenha informações importantes a longo prazo e esqueça os dados irrelevantes, o que torna os LSTMs significativamente melhores em tarefas que envolvem dados de texto complexos. A principal desvantagem dos LSTM é o seu elevado custo computacional e a lenta velocidade de treino em grandes conjuntos de dados, o que os torna não escaláveis.

---

Transformers

Em 2017, o artigo "Attention is all you need" introduziu o conceito de transformers e o mecanismo de atenção (attention mechanism). O mecanismo de atenção permite que um modelo avalie o significado de várias palavras  ou partes de palavras ou tokens numa sequência de entrada para gerar uma saída. Por conseguinte, o modelo identifica palavras chave e concentra-se mais  intensamente, reduzindo os custos computacionais e melhorando a escalabilidade. Os transformadores processam o texto concentrando-se seletivamente em partes relevantes da sequência. Isto é conseguido atribuindo uma pontuação de atenção a cada palavra na sequência de entrada:

![[Pasted image 20260209190757.png]]

As palavras com pontuações maiores são consideradas mais significativas, permitindo que os transformadores lidem com dependências de longo alcance.