# Projeto 1 – Transfer Learning com Deep Learning (DIO)

Este projeto foi desenvolvido como parte de um desafio da plataforma **DIO**, com o objetivo de aplicar o conceito de **Transfer Learning** em uma rede de Deep Learning utilizando **Python** e **TensorFlow**, no ambiente do **Google Colab**.

A proposta é simples: reutilizar um modelo pré-treinado para resolver um novo problema de classificação de imagens, no caso, distinguir **gatos e cachorros**.

---

## 📌 Objetivo do Projeto

- Aplicar Transfer Learning em um cenário prático
- Utilizar um modelo pré-treinado para classificação de imagens
- Trabalhar com datasets reais
- Documentar o processo de forma clara
- Executar todo o fluxo no Google Colab

---

## 🧠 O que é Transfer Learning?

Transfer Learning é uma técnica onde utilizamos um modelo previamente treinado em um grande conjunto de dados (como o ImageNet) e adaptamos esse conhecimento para um novo problema.

Neste projeto:
- O modelo base já sabe extrair características visuais (bordas, formas, texturas)
- Apenas as camadas finais são treinadas para resolver o novo problema
- Isso reduz custo computacional e tempo de treinamento

---

## 📂 Dataset Utilizado

Foi utilizado o dataset **Cats vs Dogs**, carregado diretamente através da biblioteca `tensorflow_datasets`.

Essa abordagem foi escolhida porque:
- Evita versionar dados grandes no GitHub
- Garante reprodutibilidade
- Funciona diretamente no Google Colab

O dataset foi dividido em:
- 80% para treinamento
- 20% para validação

---

## 🏗 Arquitetura do Modelo

- **Modelo base:** MobileNetV2 (pré-treinado no ImageNet)
- **Camadas congeladas:** modelo base
- **Camadas treináveis:** camada de pooling global, camada densa e saída binária

Arquitetura resumida:
- MobileNetV2 (congelada)
- GlobalAveragePooling2D
- Dense (ReLU)
- Dropout
- Dense (Sigmoid)

---

## ⚙️ Tecnologias Utilizadas

- Python
- TensorFlow / Keras
- TensorFlow Datasets
- Google Colab
- GitHub

---

## 🚀 Como Executar o Projeto

Este projeto foi desenvolvido para rodar no **Google Colab**.

Passos:
1. Abra o notebook no Google Colab
2. Execute as células em ordem
3. O dataset será carregado automaticamente
4. Após o treinamento, faça o upload de uma imagem para teste
5. O modelo irá classificar a imagem como **gato** ou **cachorro**

---

## 🔍 Teste com Imagem Externa

Após o treinamento, é possível testar o modelo com imagens externas.

No Colab:
- Faça o upload de uma imagem (`.jpg` ou `.png`)
- O modelo realiza a predição e exibe o resultado no console

---

## 📈 Resultados

Mesmo com poucas épocas de treinamento, o modelo consegue aprender a tarefa proposta, demonstrando a eficiência do uso de Transfer Learning para problemas de classificação de imagens.

---

## ✅ Conclusão

O projeto mostrou, na prática, como o Transfer Learning pode ser utilizado para resolver problemas reais de forma eficiente, reutilizando modelos já treinados e reduzindo a necessidade de grandes volumes de dados e longos tempos de treinamento.

---

## 📎 Observações

- O dataset não está versionado no repositório devido ao seu tamanho
- Todo o fluxo foi pensado para execução no Google Colab
- O texto deste README passou por revisão ortográfica e de clareza com o auxílio
de ferramentas de Inteligência Artificial, mantendo integralmente o conteúdo
técnico e as decisões do autor.
