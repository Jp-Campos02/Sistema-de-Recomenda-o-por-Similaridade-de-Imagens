# Sistema de Recomendação por-Similaridade de Imagens


Este projeto é um sistema de recomendação baseado em similaridade de imagens utilizando Deep Learning. O objetivo é recomendar produtos com aparência física semelhante a partir de uma imagem de consulta, como camisetas, calças, tênis e bolsas. Este sistema pode ser aplicado em e-commerces, ajudando os usuários a encontrar produtos visualmente relacionados.

Tecnologias Utilizadas
Python
TensorFlow/Keras
ResNet50 (pré-treinada no ImageNet)
Matplotlib
Sklearn
ImageDataGenerator
Descrição
O sistema utiliza um modelo de Deep Learning (ResNet50) para extrair embeddings das imagens. Após a extração, a similaridade entre as imagens é calculada utilizando a similaridade do cosseno.

A partir de uma imagem de consulta, o sistema retorna as imagens mais similares dentro de um conjunto previamente definido de classes (como camisetas, calças, tênis, bolsas).

Fluxo do Projeto
Pré-processamento:
As imagens são carregadas e pré-processadas utilizando a função preprocess_input do modelo ResNet50.

Extração de Embeddings:
Utiliza-se o modelo ResNet50 (sem a camada superior) para obter as características representativas de cada imagem.

Cálculo de Similaridade:
A similaridade entre os embeddings das imagens é calculada usando similaridade do cosseno.

Recomendações:
Para uma imagem de consulta, as imagens mais similares são apresentadas em ordem decrescente de similaridade.

Requisitos
Para executar o projeto, você precisa das seguintes bibliotecas instaladas:

tensorflow
numpy
matplotlib
scikit-learn
