É um subconjunto da aprendizagem automática inspirado no funcionamento do cérebro humano.

![[Pasted image 20260202215556.png]]
A primeira camada é como nossa informação de entrada, semelhante à nossa observação de um dia ensolarado e cheio de gente na praia

A segunda camada é começa a reconhecer recursos mais complexos, como formas ou objetos específicos. Cada camada intermediária da rede neural desenvolve uma compreensão mais detalhada dos recursos básicos identificados pelas cadas anteriores, portando há um aumento incremental no nível de detalhes adquiridos. As camadas mais profundas (finais), sintetizam recursos de nível inferior em recursos de alto nível, representando os aspectos mais complexos. É assim que podemos identificar o rosto estranho gerado por IA.

É um processo complexo que permite que as máquinas aprendam processando as informações de entrada em etapas.

Chamamos isso de ANN (Artificial Neural Network):
![[Pasted image 20260202220236.png]]
Como os nosso sentidos a primeira camada envia dados brutos para o cérebro, em seguida, as camadas intermediárias ou ocultas processam as informações de entrada, as redes neurais podem ter uma ou muitas camadas ocultas/intermediárias. Adicionar novas camadas aumenta a sua capacidade de aprendizado, mas a desvantagem é que ela precisa ser cuidadosamente gerenciada para garantir um aprendizado eficaz. Também temos uma camada de saída que gera o resultado final. 

Cada camada da rede neural artificial é composta por neurônios, ou nós, responsáveis por processar e transformar as informações recebidas.

Voltando ao exemplo do MNIST (é um famoso banco de dados de dígitos manuscritos (0-9) usado como "Hello World" para Machine Learning). O processo começa com a camada de entrada da ANN recebendo uma imagem de um dígito escrito à mão. Cada pixel dessa imagem serve como um nó de entrada. No caso do MNIST têm 28 por 28 pixels, portanto, a camada de entrada normalmente tem 784 nós de entrada:

![[Pasted image 20260202220900.png]]

Imagine que os 784 nós de entrada sejam armazenados como um vetor dentro da rede neural para formar a camada de entrada. Cada um desses 784 nós de entrada contém um número baseado em quão claro ou escuro ele é. Aqui, zero representa branco enquanto qualquer calor maior que zero indica uma cor diferente de branco. Quanto maior o número, mais escuro será o conteúdo em um determinado nó.

Descrevemos os 784 nós de entrada da camada de entrada como a largura das redes neurais e seu número de camadas como sua profundidade. Aqui a rede compreende três camadas ocultas, juntamente com as camadas de entrada e saída, totalizando uma profundidade de 5. Temos várias conexões entre os nós, por que os nós de cada camada estão vinculados a todos os nós da camada subsequente. Essa extensa rede é essencial para aprender com os dados de entrada, servidor como transformações matemáticas. Essas transformações ocorrem por meio de uma combinação de pesos e operações não lineares com combinações de pesos ideais em todos os nós, possibilitando o aprendizado. Esse método traduz a entrada por meio de várias camadas, refinando as informações antes de gerar um resultado.

Porque precisamos de tantas camadas? Que tipo de transformações podemos esperar em cada camada para obter um sistema capaz de reconhecer os dígitos de uma foto?

Quando vemos uma imagem, em segundo plano, nosso cérebro conecta vários componentes do que ela é feita. Por exemplo, o número três é composto por dois elementos: uma parte superior arrendondada e uma parte inferior curva.

A primeira camada oculta em nossa rede neural pode aprender a reconhecer esses recursos a partir dos dados de entrada. Em seguida, na segunda camada oculta, continuamos a nos basear nas informações processadas pela camada anterior. Identificamos bordas e curvas e agora podemos usá-las para discernir formas mais complexas, como loops e interseções. Quando chega na terceira camada, já aprendemos a reconhecer o número 3, por fim, a camada de saída pega os dados processados da última camada oculta e determina se o dígito é um 3.