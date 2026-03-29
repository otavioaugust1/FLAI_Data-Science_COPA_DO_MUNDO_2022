# ⚽🌍 FLAI_Data-Science_COPA_DO_MUNDO_2022 🌍⚽

<div align="center">

[![Licença: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Python](https://img.shields.io/badge/python-v3.9+-blue.svg)
[![Status](https://img.shields.io/badge/status-active-brightgreen.svg)](https://github.com/otavioaugust1/FLAI_Data-Science_COPA_DO_MUNDO_2022)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)

</div>

---

## 📖 Sobre o Projeto

Este projeto utiliza técnicas de **Data Science** e **Inteligência Artificial** para prever resultados de partidas da Copa do Mundo de 2022. A modelagem é baseada na distribuição de Poisson, que ajuda a quantificar a probabilidade de gols em partidas de futebol.

> "Modelar não é representar a realidade, mas transmitir uma equação útil."

### 🔗 Referências
- [Notícia: Plataforma interativa prevê resultados de jogos](https://g1.globo.com/sp/sao-carlos-regiao/noticia/2022/11/23/copa-do-mundo-plataforma-interativa-feita-por-estatisticos-preve-resultados-de-jogos-veja.ghtml?utm_source=whatsapp&utm_medium=share-bar-mo)
- [FLAI - Inteligência Artificial e Data Science](https://www.flai.com.br/)

---

## 🧠 Questões Abordadas

### 1️⃣ Como modelar a distribuição de gols das equipes em um jogo?

A **Distribuição de Poisson** é utilizada para calcular a probabilidade de gols em uma partida. A fórmula é:

$$
P(k; \lambda) = \frac{e^{-\lambda} \lambda^k}{k!}
$$

Onde:
- \(k\): número de gols
- \(\lambda\): média de gols esperados
- \(e\): número de Euler

### 2️⃣ Como calcular o número médio de gols por equipe por jogo?

A média histórica de gols esperados em uma Copa do Mundo é de **2,75 gols por jogo**. Para calcular a média de gols de cada equipe:

\[
m_1 = m \cdot \frac{f_1}{f_1 + f_2}
\]

\[
m_2 = m - m_1
\]

Onde:
- \(f_1\): força da equipe 1
- \(f_2\): força da equipe 2

A força de cada equipe é baseada no ranking da FIFA, ajustado para um intervalo entre 0 e 1.

---

## 🏗️ Estrutura do Projeto

```
FLAI_Data-Science_COPA_DO_MUNDO_2022/
├── dados/                # Dados utilizados no projeto
├── image/                # Imagens e gráficos
├── partida.py            # Código principal para modelagem
├── Data_Science_na_Copa_do_Mundo_Qatar_2022.ipynb  # Notebook com análises
├── LICENSE               # Licença do projeto
├── README.md             # Documentação
└── requirements.txt      # Dependências do projeto
```

---

## 🚀 Como Começar

1. Clone o repositório:
   ```bash
   git clone https://github.com/otavioaugust1/FLAI_Data-Science_COPA_DO_MUNDO_2022.git
   ```
2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
3. Explore o notebook:
   ```bash
   jupyter notebook Data_Science_na_Copa_do_Mundo_Qatar_2022.ipynb
   ```

---

## 🎥 Aulas Disponíveis

- [AULA 1 - YouTube](https://www.youtube.com/watch?v=5Q2_2GYiBwM)
- [AULA 2 - YouTube](https://www.youtube.com/watch?v=7eCjyJ-8Se4&t=7s)

---

## 👨‍💻 Contribuidor

- **Nome:** Otavio Augusto
- **Email:** otavioaugust@gmail.com
- **GitHub:** [@otavioaugust1](https://github.com/otavioaugust1)
- **Versão:** 0.2.1

---

## 📜 Licença

Este projeto está licenciado sob a licença [MIT](LICENSE). Sinta-se à vontade para usar, modificar e compartilhar este projeto, desde que mantenha os créditos ao autor original.






