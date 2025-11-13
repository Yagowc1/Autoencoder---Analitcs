# Redução de Dimensionalidade
# Introdução
O texto a seguir tem como objetivo fornecer uma breve introdução a um grupo de métodos de redução de dimensionalidade. Nele será apresentada uma pequena descrição de cada um dos métodos, assim como uma demonstração de seu funcionamento na prática, por meio da linguagem de programação python. Ao fim de tudo, será feita uma análise comparativa dos diferentes métodos de redução para que se possam ser tiradas as conclusões finais. 
## PCA
A Principal Component Analysis (PCA), ou Análise de Componentes Principais, se trata de uma técnica que busca analisar uma base de dados na tentativa de encontrar as direções de maior variância entre eles. A partir daí, ele formula um grupo menor de novas variáveis que melhor represente os padrões importantes dos dados. Essas variáveis são os chamados "componentes principais", que dão nome ao método.

Para determinar esses componentes principais, a PCA centraliza os dados ao redor de sua média e calcula os autovetores e autovalores da matriz de covariância. Os autovetores são então utilizados para explicar as direções de maior variância dos dados, semelhante a uma linha desenhada em um gráfico. Já os autovalores explicam quanto que esses dados variam nessa dada direção, ou seja, como que esses dados estão distribuídos dentro dessa linha.

## LDA
Já a Linear Discriminant Analysis (LDA), ou Análise Discriminatória Linear, se refere a uma outra técnica de redução de dimensionalidade, mas essa se baseando em combinar 2 ou mais características em uma só (chamada classe), efetivamente reduzindo o número de variáveis a serem analisadas sem perder dados relevantes.

Para tal, a LDA inicia seu procedimento calculando a média e matriz de covariância para cada uma das classes identificadas. Após isso, ela calcula a matriz de dispersão entre as classes e entre os elementos de cada classe. A ideia aqui é reduzir ao máximo a variância entre os elementos da mesma classe, enquanto aumenta a variância entre classes diferentes. No contexto de um gráfico, a LDA une os pontos que estão próximos em grupos, deixando os grupos distantes uns dos outros.