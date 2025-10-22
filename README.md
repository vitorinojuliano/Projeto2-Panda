# Projeto2-Panda
  Classificação de Imagens com CNN Shallow e CNN Deep — Fashion-MNIST

# Descrição do Projeto

  Este projeto faz parte das Semanas 10 e 11 do projeto de extensão de Data Science, com o objetivo de comparar duas arquiteturas de redes neurais convolucionais (CNN) — uma shallow (rasa) e uma deep (profunda) — aplicadas à classificação de imagens do dataset Fashion-MNIST.

  O dataset contém 70.000 imagens em tons de cinza (28x28 pixels) de roupas e acessórios divididos em 10 classes, como camisetas, calças, bolsas e botas.

# Objetivo

  Avaliar como a profundidade da rede (quantidade de camadas convolucionais e neurônios) influencia na capacidade de generalização e precisão do modelo.

# Dataset — Fashion-MNIST
  Tipo de dado	Quantidade	Dimensão	Observações
  Treino	60.000	28x28	Dividido em 48.000 treino + 12.000 validação
  Teste	10.000	28x28	Utilizado apenas para avaliação final

Classes:
  
  0: Camiseta/Top
  1: Calça
  2: Pullover
  3: Vestido
  4: Casaco
  5: Sandália
  6: Camisa
  7: Tênis
  8: Bolsa
  9: Bota

# Etapas do Projeto

* 1-Importação das bibliotecas (TensorFlow, Keras, NumPy, Matplotlib, Seaborn, scikit-learn)
* 2-Carregamento e inspeção do dataset
* 3-Análise exploratória — distribuição de classes e visualização de amostras
* 4-Pré-processamento
* 5-Normalização dos pixels (0–255 → 0–1)
* 6-Reformatação para formato compatível com CNN ((28, 28, 1))
* 7-Conversão dos rótulos para One-Hot Encoding
* 8-Divisão treino/validação/teste
* 9-Arquitetura: CNN (Convolutional Neural Network)
    ** CNN Shallow - Uma camada convolucional, porém mais larga.
    ** Aprende: Padrões simples e locais (bordas, linhas, cores)
    ** CNN Deep - Quatro camadas convolucional, mais especializada.
    ** Aprende: Padrões hierárquicos e complexos (texturas -> partes -> objetos inteiros)
* 10-Comparação de desempenho e análise dos resultados
