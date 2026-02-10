Bancos de dados relacionais organizam informações em linhas e colunas. Isso os torna perfeitos para dados estruturados. Mas eles não são ótimos quando temos que lidar com dados não estruturados, como texto, imagens, vídeo e áudio. 

Para converter multimídia em um formato que os computadores podem entender, usamos incorporações vetoriais, que são então armazenadas e organizadas em um banco de dados vetorial. 

Essencialmente, em um banco de dados vetorial, temos arrays de números agrupados com base em sua semelhança. Vamos imaginar a base de dados do YouTube com milhões de vídeos. Esses vídeos podem ser agrupados com base em seu gênero. Podemos ter vlogs, vídeos de jogos, tutoriais, vídeos de como fazer, avaliações tecnológicas, música e outros formatos.

O objetivo é indexar todos os vídeos e organizá-los de uma forma que permita uma recuperação e pesquisa muito rápidas. Para isso, os vetores são organizados no banco de dados. Para que os vídeos com conteúdo semelhante sejam posicionados mais próximos no espaço vetorial. 

Essa organização é baseada em métricas de similaridade que medem quão próximos ou distantes os vetores são uns dos outros, o que pode ser interpretado como qual é a diferença entre vídeos em termos de gênero, conteúdo, comprimento ou outra semelhança estilística.

Em alguns casos, podemos ter milhões e milhões de incorporações vetoriais, o que significa que pesquisar milhões de vetores e procurar semelhanças seria muito lento. Para garantir a recuperação rápida dos dados, as bases de dados vetoriais dependem da indexação e usam técnicas ML que lhes permitem pesquisar de forma eficiente. 

O caso de uso das bases de dados vetoriais que eu descrevi aqui é sobre busca. Podemos utilizar bases de dados vetoriais para busca e busca de similaridade com base no significado e contexto das palavras. 

Além disso, uma das aplicações mais legais de bancos de dados vetoriais é dar aos LLMs como GPT e Gemini memória de longo prazo. Ao armazenar interações passadas ou aprender informações como vetores, um modelo pode referenciar esses dados para entender melhor o contexto.

Por exemplo, se você usar um LLM como assistente de chatbot, ele pode armazenar informações sobre conversas anteriores com você e clientes similares e fornecer respostas mais informadas.

Para seus projetos de IA, considere bases de dados vetoriais populares como Pinecone, Weeveate, Milvus, Chroma e Elasticsearch. Embora altamente popular, Pinecone não é de código aberto, o que pode limitar alguns projetos. Em contraste, Weeveate, Milvus, Chroma e Elasticsearch oferecem alternativas populares de código aberto.