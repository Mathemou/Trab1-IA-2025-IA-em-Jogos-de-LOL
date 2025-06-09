# 📊 Trabalho 1 - Inteligência Artificial e Sistemas Inteligentes (2025)

Este repositório contém a implementação do **Trabalho 1** da disciplina de Inteligência Artificial e Sistemas Inteligentes, ministrada pelo Prof. Flávio Miguel Varejão em 2025.

O objetivo do trabalho é realizar uma **comparação experimental** entre diferentes algoritmos de classificação, utilizando **validação cruzada aninhada**, com análise estatística dos resultados obtidos.

---

## 🧠 Técnicas de Classificação Avaliadas

- Decision Tree (DT)
- K-Nearest Neighbors (KNN)
- Multi-layer Perceptron (MLP)
- Random Forest (RF)
- Heterogeneous Boosting (HB) — implementação própria

---

## 🗂 Estrutura do Projeto

```
.
├── data/
│   └── jogosLol2021.csv     # Base de dados usada nos experimentos
├── requirements.txt         # Dependências do projeto
├── Trab1_Nome_Sobrenome.ipynb   # Código-fonte em Jupyter Notebook
└── README.md                # Este arquivo
```

---

## 📁 Dados

A base de dados `jogosLol2021.csv` contém registros de partidas do jogo *League of Legends* durante a temporada de 2021. Cada instância representa uma partida, com várias características numéricas e uma variável alvo binária indicando a equipe vencedora.

Você deve **descartar o identificador da partida** e realizar **pré-processamento**, incluindo:
- Codificação de variáveis categóricas
- Codificação da variável alvo
- Padronização das características numéricas

A tarefa específica (ex.: usar dados de pré-jogo, 10 minutos, etc.) depende do **último dígito da matrícula**.

---

## ⚙️ Execução

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/trab1-ia-2025.git
   cd trab1-ia-2025
   ```

2. Crie um ambiente virtual (opcional, mas recomendado):
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/macOS
   venv\Scripts\activate     # Windows
   ```

3. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

4. Execute o notebook:
   ```bash
   jupyter notebook Trab1_Nome_Sobrenome.ipynb
   ```

---

## 📈 Resultados Esperados

- Tabela com:
  - Média de acurácia por classificador
  - Desvio padrão
  - Intervalo de confiança a 95%

- Boxplots comparativos entre os classificadores

- Tabela de testes estatísticos pareados:
  - Teste **t** pareado (triângulo superior)
  - Teste de **Wilcoxon** (triângulo inferior)
  - Resultados significativos em **negrito**

---

## 📝 Observações

- Usar `random_state=36854321` para o `RepeatedStratifiedKFold`.
- Usar `random_state=13` nos classificadores para reprodutibilidade.
- O classificador HB combina: DT, NB, KNN e MLP.
- O critério de votação do HB é **votação majoritária**.

---

## 📄 Artigo

Além do notebook, um artigo em LaTeX (máximo 5 páginas) deve ser entregue via Overleaf, contendo:
1. Introdução
2. Base de Dados
3. Método Heterogeneous Boosting
4. Experimentos e Resultados
5. Conclusão
6. Referências

---

## 📅 Prazo de Entrega

📌 **Data limite: 09/07/2025**

O trabalho deve ser enviado como dois arquivos com o mesmo nome:
- `Trab1_Nome_Sobrenome.ipynb`
- `Trab1_Nome_Sobrenome.pdf`

---

## 🚫 Penalidades

- Entregas atrasadas não serão avaliadas.
- Trabalhos copiados (plágio) receberão nota **zero**.

---

**Disciplina:** Inteligência Artificial e Sistemas Inteligentes  
**Professor:** Flávio Miguel Varejão  
**Ano:** 2025
