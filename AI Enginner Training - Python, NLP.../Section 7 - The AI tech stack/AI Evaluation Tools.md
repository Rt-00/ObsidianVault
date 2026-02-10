Já mencionei que nossa equipe construiu um aplicativo simulador de entrevista alimentado pela GPT. 

A fase mais desafiadora do processo de desenvolvimento não foi preparar o banco de dados com perguntas de entrevista para serem alimentadas à IA ou ao trabalho do desenvolvedor. Em vez disso, descobrimos que gastamos mais tempo em Prompt Engineer da IA e QAing suas respostas. 

Isso destacou uma questão vital que todos constroem produtos de IA, avaliação de modelo. 

Depois de construir um produto alimentado por IA, você precisa de uma maneira confiável para testar sua saída. Se você pular a fase de avaliação, você corre o risco de ir ao vivo com um produto de IA que alucina, fornece respostas inconsistentes, como questões éticas, que hoje em dia é provavelmente o maior disjuntor de negócios, e em geral libera um produto que não está à altura dos padrões exigidos e não funciona como esperado. 

Então decidimos usar a IA popular como uma abordagem de juiz, o que significa essencialmente pedir uma IA para avaliar a saída de outra IA. O juiz de IA selecionará e avaliará uma amostra de perguntas e respostas do simulador de entrevista de IA. Nosso aplicativo é construído de uma forma que permite aos alunos serem feitos dois tipos principais de perguntas, questões abertas e codificação. Os dois são muito diferentes de uma perspectiva de IA. 

As perguntas de código são tarefas fechadas, e muito mais fáceis de avaliar do que as abertas. Com questões de codificação, o IA sabe que tipo de saída deve esperar da tarefa, mas pode, portanto, facilmente avaliar se a ferramenta calculada corretamente ou se seu código produziu uma determinada saída.

Questões abertas são muito mais subjetivas e difíceis de avaliar, mas modelos fortes estão melhorando nessa atividade. Segundo o relatório do Estado de IA de Langchains, 58% dos projetos construídos em sua plataforma utilizaram a IA como juiz, o que mostra a importância crescente dessa parte do Devcycle de IA. 

Os benefícios substanciais da avaliação da IA pela IA incluem a eficiência de custo, escalabilidade, velocidade e a capacidade de rever um volume maior de interações com os clientes. Isso é especialmente importante se você tiver milhares ou dezenas de milhares de usuários e quiser implantar um aplicativo com IA. Por outro lado, os modelos de IA carecem de intuição humana e ética, o que pode levar a desafios em contextos em que a compreensão e os julgamentos morais são cruciais. Portanto, também é imperativo envolver juízes humanos no processo de avaliação.