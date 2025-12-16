# Transfer Learning com Deep Learning usando Python

## 📌 Descrição do Projeto
Este projeto aplica o método de Transfer Learning em uma rede de Deep Learning
utilizando Python e TensorFlow no ambiente Google Colab.  
Foi utilizado um modelo pré-treinado (MobileNetV2) para classificar imagens de
gatos e cachorros.

## 🧠 Conceito de Transfer Learning
Transfer Learning consiste em reutilizar o conhecimento adquirido por um modelo
treinado em um grande conjunto de dados para resolver um novo problema,
reduzindo o tempo de treinamento e a necessidade de grandes volumes de dados.

## 🗂 Dataset Utilizado
- Dataset: Cats vs Dogs
- Classes: Gatos e Cachorros
- Estrutura de pastas organizada em treino e validação

## 🏗 Arquitetura do Modelo
- Modelo base: MobileNetV2 (pré-treinado no ImageNet)
- Camadas congeladas
- Camadas finais personalizadas para classificação binária

## ⚙️ Tecnologias Utilizadas
- Python
- TensorFlow / Keras
- Google Colab
- GitHub

## 📊 Resultados
O modelo alcançou uma boa acurácia na base de validação, demonstrando a eficiência
do uso de Transfer Learning para classificação de imagens.

## 🚀 Como Executar
1. Abra o notebook no Google Colab
2. Faça o upload do dataset
3. Execute as células em ordem

## 📌 Conclusão
O uso de Transfer Learning mostrou-se uma abordagem eficaz para problemas de
classificação com conjuntos de dados relativamente pequenos.
