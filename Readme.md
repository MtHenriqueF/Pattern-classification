## Estudo de Classificação Bayesiana e Redução de Dimensionalidade
Este notebook é um estudo prático e visual dos fundamentos da teoria de decisão Bayesiana e uma análise comparativa entre duas técnicas populares de redução de dimensionalidade: PCA (Análise de Componentes Principais) e LDA (Análise Discriminante Linear).

Através de uma série de questões, o código gera dados sintéticos de duas classes, treina classificadores, estima parâmetros e visualiza fronteiras de decisão e projeções de dados para solidificar a compreensão teórica.

## Conceitos abordados

- **Teoria de decisão Bayesiana**:O princípio de minimizar o erro de classificação ao escolher a classe com a maior probabilidade a posteriori.

- **Verossimilhança (Likelihood)**: Como modelar a probabilidade dos dados pertencerem a uma classe, utilizando a distribuição Gaussiana Multivariada como nosso modelo de verossimilhança.

-**Análise de Componentes Principais (PCA)**: Uma técnica não supervisionada que encontra as direções de maior variância nos dados para reduzir a dimensionalidade.

- **Análise Discriminante Linear (LDA)**: Uma técnica supervisionada que encontra a direção que melhor separa as classes para reduzir a dimensionalidade com foco em classificação.

## Principais resultados:

- Fronteira Estimada vs. Verdadeira: A fronteira de decisão calculada a partir dos dados amostrais se aproxima muito bem da fronteira ideal (calculada com os parâmetros reais), validando o processo de estimação.

- Deslocamento da Fronteira com Priors: Fica claro que aumentar a probabilidade a priori de uma classe expande sua região de decisão, movendo a fronteira para longe de seu centro.

- PCA vs. LDA: A análise comparativa demonstra visual e quantitativamente que a LDA é superior à PCA para tarefas de classificação. A projeção LDA resulta em uma separação muito maior entre as classes no espaço de dimensionalidade reduzida, pois seu objetivo é maximizar a discriminação, ao contrário da PCA, que apenas maximiza a variância.