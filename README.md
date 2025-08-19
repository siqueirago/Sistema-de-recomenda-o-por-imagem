# 🔎 Sistema de Recomendação por Imagens Digitais

Este projeto implementa um sistema de recomendação baseado em imagens digitais utilizando Python, TensorFlow/Keras e Google Colab.
O objetivo é encontrar imagens similares dentro de um conjunto, aplicando redes neurais convolucionais pré-treinadas (CNN - Transfer Learning) para extrair características visuais e calcular a similaridade entre elas.

## 🚀 Tecnologias Utilizadas

* Python 3

* Google Colab (ambiente de execução)

* TensorFlow / Keras (modelos pré-treinados como VGG16, ResNet50 ou MobileNet)

* NumPy & Pandas (manipulação de dados)

* Matplotlib (visualização)

* scikit-learn (cálculo de distâncias e métricas)

## 📂 Estrutura do Projeto
````
├── imagens/                # Pasta com as imagens de exemplo
├── notebook.ipynb          # Código principal no Google Colab
├── exemplo.png             # Imagem de teste enviada
├── README.md               # Documentação do projeto
````
## ⚙️ Como Funciona

1. Extração de Características:
Utilizamos uma CNN pré-treinada (ex: ResNet50) sem a última camada para gerar vetores de características de cada imagem.

2. Indexação:
Todos os vetores das imagens são armazenados em memória para busca eficiente.

3. Busca de Similaridade:
Quando o usuário insere uma nova imagem, extraímos suas características e calculamos a distância (ex: cosseno ou euclidiana) em relação às demais.

4. Recomendação:
Retornamos as imagens mais semelhantes à imagem de entrada.

## ▶️ Como Executar no Google Colab

1. Abra o Google Colab

2. Faça upload do arquivo notebook.ipynb.

3. Faça upload de uma pasta de imagens para teste.

4. Execute todas as células.

5. Carregue uma imagem de consulta e veja as imagens recomendadas.


## 📌 Próximos Passos

1. Implementar busca aproximada (ANN) para acelerar recomendações em grandes bases.

2. Criar uma interface web simples com Streamlit.

2. Avaliar o sistema com métricas de recomendação (ex: Precision@K).

## 👨‍💻 Autor

Projeto desenvolvido por Julio Siqueira no Google Colab.
