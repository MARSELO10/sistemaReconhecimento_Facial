<img width="753" height="572" alt="sopranosFundo" src="https://github.com/user-attachments/assets/60a089a1-ccf9-4bbc-9dd6-75b4321af8b6" />

---

# ﻿🔍👱🏼‍♀️👦🏻 Sistema de Reconhecimento Facial

![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

---

## 📋 - Descrição 

Um sistema completo de detecção e reconhecimento facial desenvolvido do zero utilizando TensorFlow, OpenCV e machine learning. O sistema é capaz de detectar múltiplas faces simultaneamente e classificá-las com base em um modelo treinado.

---

## 🎯 - Sobre o Projeto de reconhecimento facial

Este projeto implementa um sistema completo de reconhecimento facial que combina técnicas modernas de visão computacional e aprendizado de máquina. O sistema utiliza uma abordagem em duas etapas:

1. **Detecção de Faces**: Utiliza classificadores Haar Cascade do OpenCV para localizar faces em imagens
2. **Reconhecimento de Faces**: Emprega uma rede neural convolucional personalizada para extrair características faciais e um classificador SVM para identificação

O objetivo principal é demonstrar a integração de diferentes tecnologias de IA para criar uma solução prática e funcional de reconhecimento facial.

---

## 🚀 Funcionalidades

* ✅ Detecção múltipla de faces: Localiza e extrai automaticamente todas as faces encontradas em uma imagem, mesmo que sejam várias pessoas ao mesmo tempo.
* ✅ Pré-processamento: Conversão para escala de cinza e redimensionamento para 128×128 pixels.
* ✅ Classificação: Uso do SVM.
* ✅ Extração de características: Rede neural convolucional.
* ✅ Visualização de resultados: Desenho automático de caixas delimitadoras.
* ✅ Treinamento flexível: Permite treinar com datasets reais de rostos ou usar dados sintéticos para demonstração.
* ✅ Métricas de performance: Cálculo automático da acurácia durante o treino do classificador.
* ✅ Persistência do modelo: Salvamento em arquivo.
* ✅ Compatibilidade com Google Colab.

---

## 📁 Instrução de Uso Google Collab

1- Todas as instruções estão documentadas no próprio arquivo do Colab.

2.1 - As dependências necessárias (OpenCV, TensorFlow, scikit-learn, pandas) são instaladas automaticamente.

2.2 - A imagem de entrada deve ser carregada via files.upload(), permitindo escolher diretamente do seu computador.

2.3 - As faces presentes na imagem serão detectadas, recortadas e redimensionadas para 128×128 pixels em escala de cinza.

2.4 - Uma rede neural convolucional gera embeddings de 64 dimensões para cada rosto detectado.

2.6 - As previsões incluem nome da pessoa e nível de confiança, exibidos na imagem com caixas delimitadoras (bounding boxes).

2.7 - O resultado final é salvo em /content/resultado_reconhecimento.jpg e pode ser visualizado no próprio Colab.

<img width="292" height="292" alt="resultado01" src="https://github.com/user-attachments/assets/94aa5991-76e8-473a-b334-19d3f494b9c4" />

Obs: há um problema que o sistema não está treinado para cada rosto, então todos serão nomeados como Adriana.

---

## 🛠️ Tecnologias Utilizadas

* Python
* TensorFlow / Keras - Construção da rede neural convolucional para extração de embeddings faciais
* OpenCV – Detecção de faces, leitura, manipulação e exibição de imagens
* Scikit-learn – Treinamento e avaliação do classificador SVM, além do pré-processamento de rótulos
* NumPy – Operações numéricas e manipulação de matrizes/vetores
* Pandas – Organização e exibição dos resultados em formato de tabela
* Pickle – Salvamento e carregamento do modelo treinado
* oogle Colab

---

## 📁 Estrutura do Projeto

```

projeto
├── FaceRecognitionSystem (class)          # Classe principal para detecção e reconhecimento facial
│   ├── __init__()                         # Inicializa detector HaarCascade, label encoder e rede neural
│   ├── create_face_embedder()             # Cria a rede neural para geração de embeddings (64 dimensões)
│   ├── detect_faces()                     # Detecta múltiplas faces em uma imagem
│   ├── extract_face_embedding()           # Extrai vetor de características (embedding) de uma face
│   ├── train_classifier()                 # Treina classificador SVM com embeddings e labels
│   ├── predict_face()                     # Prediz a identidade de uma face com base no embedding
│   ├── process_image()                    # Processa imagem completa: detecta, extrai e reconhece faces
│   └── draw_results()                     # Desenha caixas delimitadoras e labels sobre a imagem
│
└── main (sequência do script)             # Instancia FaceRecognitionSystem, treina e executa predições


```

---

## 📊 Aplicações em Visão Computacional

* Detecção de múltiplos rostos em imagens
* Extração de embeddings faciais para representar cada rosto em um vetor de 64 dimensões
* Treinamento de classificadores SVM para reconhecimento de identidades
* Reconhecimento de pessoas em imagens reais com previsão de rótulo e score de confiança
* Visualização das predições com caixas delimitadoras e nomes sobre cada face detectada
* Geração de dados sintéticos para simulações quando não há dataset disponível
* Persistência do modelo treinado para reutilização em futuras execuções

---

## 🤝 Patrocinadores ou Afins

- [DIO](https://www.dio.me/): plataforma de cursos e bootcamps online.
- [Baires Dev](https://www.bairesdev.com/): A BairesDev é uma empresa multinacional americana de outsourcing de TI e desenvolvimento de software
- [OpenCV](https://opencv.org/):Biblioteca de visão computacional utilizada para manipulação e exibição de imagens.
- [TensorFlow](https://www.tensorflow.org/?hl=pt-br): Biblioteca para criação e treinamento da rede neural convolucional para embeddings faciais.
- [Scikit-Learn](https://scikit-learn.org/stable/): Biblioteca para treinamento e avaliação do classificador SVM e pré-processamento de labels.
- [Pandas](https://pandas.pydata.org/): Biblioteca para organização e visualização tabular dos resultados.
- - [Python](https://www.python.org/): Linguagem de programação utilizada em todo o projeto.
- [Google Collab](https://colab.google/): O Google Colab (ou Colaboratory) é um ambiente de desenvolvimento integrado (IDE) gratuito e baseado em nuvem que permite escrever e executar código Python diretamente no navegador, sem necessidade de instalação ou configuração.

---

# Contribuição

Contribuições são bem-vindas!\
Se você encontrar algum problema ou tiver sugestões de melhorias, por favor abra uma **issue** ou envie um **pull request** para o repositório.\
Ao contribuir para este projeto, siga as convenções de commits e envie suas alterações em um **branch** ou **file** separado.\
Saiba mais sobre o código de conduta acessando o link: [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)

---

# Licença

Este repositório possui licença [MIT](https://github.com/MARSELO10/sistemaReconhecimento_Facial)



