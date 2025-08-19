🔎 Sistema de Recomendação por Imagens Digitais

Este projeto implementa um sistema de recomendação baseado em imagens digitais utilizando Python, TensorFlow/Keras e Google Colab.
O objetivo é encontrar imagens similares dentro de um conjunto, aplicando redes neurais convolucionais pré-treinadas (CNN - Transfer Learning) para extrair características visuais e calcular a similaridade entre elas.

🚀 Tecnologias Utilizadas

Python 3

Google Colab (ambiente de execução)

TensorFlow / Keras (modelos pré-treinados como VGG16, ResNet50 ou MobileNet)

NumPy & Pandas (manipulação de dados)

Matplotlib (visualização)

scikit-learn (cálculo de distâncias e métricas)

📂 Estrutura do Projeto
├── imagens/                # Pasta com as imagens de exemplo
├── notebook.ipynb          # Código principal no Google Colab
├── exemplo.png             # Imagem de teste enviada
├── README.md               # Documentação do projeto

⚙️ Como Funciona

Extração de Características:
Utilizamos uma CNN pré-treinada (ex: ResNet50) sem a última camada para gerar vetores de características de cada imagem.

Indexação:
Todos os vetores das imagens são armazenados em memória para busca eficiente.

Busca de Similaridade:
Quando o usuário insere uma nova imagem, extraímos suas características e calculamos a distância (ex: cosseno ou euclidiana) em relação às demais.

Recomendação:
Retornamos as imagens mais semelhantes à imagem de entrada.

▶️ Como Executar no Google Colab

Abra o Google Colab
.

Faça upload do arquivo notebook.ipynb.

Faça upload de uma pasta de imagens para teste.

Execute todas as células.

Carregue uma imagem de consulta e veja as imagens recomendadas.

📸 Exemplo de Uso

Imagem de consulta:

Resultado da recomendação:

Imagem 1 (mais similar)

Imagem 2

Imagem 3

📌 Próximos Passos

Implementar busca aproximada (ANN) para acelerar recomendações em grandes bases.

Criar uma interface web simples com Streamlit.

Avaliar o sistema com métricas de recomendação (ex: Precision@K).

👨‍💻 Autor

Projeto desenvolvido por Julio Siqueira no Google Colab.
