Vamos começar como um jogo de associação de palavras para introduzir alguns conceitos.

Quatro jogadores divididos em duas equipes. Um jogador sussurra uma palavra secreta para um oponente, que então deveria dizer uma palavra relacionada em voz alta para ajudar seu  colega de equipe a adivinhar a palavra original sussurrada. O colega então tenta um palpite, se estiver incorreto, a próxima equipe pode tentar descrever a palavra secreta, o primeiro a adivinhar a palavra correta ganha.

Por exemplo, se eu ouvir a palavra banana, posso dizer amarelo para o meu colega de equipe, mas amarelo pode ser associado a muitas outras coisas, incluindo taxis, girassóis, limões, ouro... Portanto, embora exista a possibilidade de meu colega adivinhar banana a partir de amarelo, não é o resultado mais provável. O uso da palavra casca poderia melhorar a precisão. De qualquer forma, para ir bem nesse jogo devemos pensar na palavra que maximiza a probabilidade do seu colega de equipe acertar. Algumas palavras podem ser muito complexas, então precisaremos de algumas tentativas para entendê-las, fornecendo mais contexto.

Isso é uma boa analogia de como os LM funcionam.  Um LM prevê principalmente a palavra ideal para preencher um espaço em branco. Por exemplo, se um usuário digitar "ser ou não ser, essa é a xxxxxxx". O modelo vai responder: "questão", assim como no jogo de associação de palavras, preenchendo com a palavra mais provável. Portanto, os LLMs são probabilísticos, capazes de prever a palavra ausente em uma frase com base em no contexto fornecido pelas palavras anteriores.

Em geral, temos dois tipos de modelos de linguagem: mascarados e autorregressivos.

Os modelos de linguagem mascarados podem adivinhar a palavra ausente independentemente de sua posição em uma frase. Por exemplo, considerando a frase:
"Água xxxxx em 0 graus célsius", O modelo poderia usar as informações de antes e depois do espaço em brando para preencher com "congela".

Os modelos autorregressivos preveem a próxima palavra usando o contexto das palavras anteriores. Nesse caso a sentença seria: "Aguá congela em 0 graus xxxxx" e, analisando o contexto das palavras anteriores, preencheria com célsius.

Os modelos GPT da OpenAI são autorregressivos, que funcionam condicionando cada previsão a todas as palavras geradas.

Mas como os LMs podem prever a próxima palavra em uma sequência? Isso se baseia no aprendizado estatístico de grandes quantidades de dados. Um modelo de linguagem ganha a capacidade de trabalhar com a linguagem analisando e aprendendo com os padrões e estruturas encontrados no texto de entrada que ele processa. Isso envolve a digestão de grandes conjuntos de dados contento diversos estilos e usos linguísticos que permitem que o modelo reconheça e preveja sequências de palavras possíveis em diferentes contextos.

Com o tempo, o modelo constrói um mapa probabilístico de associações e dependências de palavras, aumentando sua capacidade de gerar respostas coerentes e contextualmente apropriadas a solicitações mais complicadas.

Os resultados dos modelos de linguagem são abertos, o que significa que eles podem usar o vocabulário criado pelo aprendizado com dados de treinamento para gerar um número infinito de resultados possíveis.

A palavra gerar é fundamental, daí o nome IA generativa. Inicialmente, os desenvolvedores de IA se concentraram na criação de modelos adaptados a um único idioma, mas os modelos modernos são capazes de processar e compreender vários idiomas.

Em geral discutimos o comportamento de LMs, mas qual a diferença com os LLM? e o qual tamanho qualifica um LM como LLM?

O termo LLM não tem uma definição formal e significa mais que ele foi treinado com grande volume de dados e esse volume de dados continua se expandindo com o tempo. Portanto, o que é grande hoje, não será tão grande em alguns anos.