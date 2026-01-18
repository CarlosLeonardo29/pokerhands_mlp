<h1 align="center">🃏 Classificação de Mãos de Poker com MLP</h1>

<p align="center">
  Implementação de uma Rede Neural Perceptron Multicamadas para classificação de mãos de poker  
  utilizando diferentes algoritmos de otimização.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python"/>
  <img src="https://img.shields.io/badge/TensorFlow-2.x-orange?style=for-the-badge&logo=tensorflow"/>
  <img src="https://img.shields.io/badge/Scikit--Learn-ML-green?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Dataset-UCI%20Poker%20Hands-red?style=for-the-badge"/>
</p>

---

## 👨‍💻 Autor

### **Eng. Eletricista Carlos Leonardo Lazzari**

<p align="left">
  <a href="https://www.linkedin.com/in/carlos-leonardo29/">
    <img src="https://img.shields.io/badge/LinkedIn-Carlos_Leonardo-blue?logo=linkedin&logoColor=white"/>
  </a>
  <a href="http://lattes.cnpq.br/1607061869218351">
    <img src="https://img.shields.io/badge/Currículo-Lattes-green"/>
  </a>
  <a href="https://linktr.ee/carlosleonardo29">
    <img src="https://img.shields.io/badge/Linktree-Carlos_Leonardo-brightgreen?logo=linktree&logoColor=white"/>
  </a>
</p>

> 📩 Contato: [carlos.leonardo290403@gmail.com](mailto:carlos.leonardo290403@gmail.com)

---

## 🗂️ Conteúdo

- [📌 Visão Geral](#-visão-geral)  
- [📂 Dataset](#-dataset)  

---

## 📌 Visão Geral

Este projeto tem como objetivo aplicar uma **Rede Neural Perceptron Multicamadas (MLP)** para classificar mãos de poker a partir das cartas recebidas.

Cada mão é composta por 5 cartas, e cada carta é descrita por:

- Naipe (1–4)
- Valor (1–13)

Totalizando **10 atributos de entrada** e **10 classes de saída**, correspondentes às combinações oficiais do poker:

| Classe | Descrição |
|------|-------------|
| 0 | Nada |
| 1 | Um Par |
| 2 | Dois Pares |
| 3 | Trinca |
| 4 | Sequência |
| 5 | Flush |
| 6 | Full House |
| 7 | Quadra |
| 8 | Straight Flush |
| 9 | Royal Flush |

---

## 📂 Dataset

- Fonte: **UCI Machine Learning Repository**  
- Instâncias: **1.025.010**  
- Atributos: 10 preditores + 1 classe

Download automático via biblioteca:

```python
from ucimlrepo import fetch_ucirepo
poker_hand = fetch_ucirepo(id=158)
