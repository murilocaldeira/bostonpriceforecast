Este é um Data App utilizado para exibir a solução de Machine Learning para o problema de predição de valores de imóveis de Boston.

Com base no seguinte dataset, que mostra o valor de imóveis da cidade de boston: 

from sklearn.datasets import load_boston

boston = load_boston()


Foi analisado o dataset e excluidas as colunas com alta correlação entre si e sem relação com a variável alvo, as colunas com alta ocorrencia de valores faltantes assim como os 16 maiores valores de imóveis (outliers)

Após isso, para predição foi criado um base line com base no número de quartos (RM) devido a alta correlação com a variavel alvo e testados mais 3 métodos de machine learning, comparando o coeficiente de Pearson com os valores reais da base. 

Algoritimos testados:
Regressão Linear
Arvore de decisão
Random Forest

Utilizado então o Random Forest para realizar a predição, pois foi o algorítimo mais preciso.

Nesta solução está o DATASET dentro da pasta model. 

Para executar, após clonar os arquivos: 

1 - Instalar Python 3.8 e o pip
2 - pip install -r requirements.txt
3 - streamlit run app.py






