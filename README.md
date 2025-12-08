# 🍷 Análise da Qualidade de Vinhos (Wine Quality Analysis)

## 📋 Descrição do Projeto

Este projeto consiste na aplicação de técnicas de **Modelagem Estatística** e **Machine Learning** no conjunto de dados de Vinhos Tintos, com o objetivo de analisar as relações entre as variáveis físico-químicas e a qualidade final percebida.

O trabalho cumpre os requisitos de análise exploratória de dados (**EDA**), implementação de algoritmos de **Regressão** (Linear, Múltipla, Polinomial) e **Classificação** (Regressão Logística, Naive Bayes), e **otimização sistemática** dos modelos via Validação Cruzada (CV) e Grid Search.

### Hipótese de Negócio Central

A hipótese principal testada é que a **qualidade percebida de um vinho** é significativamente descrita e previsível por variáveis como a **acidez volátil** e o **teor alcoólico**, sendo estes os descritores mais influentes na sua classificação final.

### Variáveis Alvo Analisadas

1.  **Regressão:** `quality` (Score contínuo de 3 a 8).
2.  **Classificação:** `vinho_bom` (Binária: 1 para qualidade $\geq 7$, 0 para as demais).

---

## 🛠️ Instalação e Execução (Reprodutibilidade)

Para garantir a **reprodutibilidade total** e evitar conflitos de dependência (como os que envolvem o `pycaret`), o projeto utiliza o **Conda** para gerenciamento de ambiente, conforme o arquivo `environment.yml`.

### 📦 Pré-requisitos

Certifique-se de ter o **Miniconda** ou **Anaconda** instalados em seu sistema.

### 🚀 Instalação do Ambiente

1.  **Crie e Ative o Ambiente:** Utilize o arquivo `environment.yml` para replicar o ambiente.
    ```bash
    # 1. Crie o ambiente 
    conda env create -f environment.yml 
    
    # 2. Ative o ambiente
    conda activate 'pycaret_env' 
    ```

### ➡️ Execução do Projeto

Todo o relatório, código-fonte, resultados, gráficos de diagnóstico e análises estão contidos no arquivo Jupyter Notebook.

1.  **Inicie o Jupyter Notebook:** Certifique-se de que o ambiente Conda está ativado e execute o comando:
    ```bash
    jupyter notebook
    ```
2.  **Abra o Notebook:** Navegue e abra o arquivo `main.ipynb`.
3.  **Execute as Células:** Execute todas as células sequencialmente para replicar a EDA, o treinamento dos modelos e a otimização.

---

## 📂 Organização do Repositório

| Arquivo/Pasta | Descrição |
| :--- | :--- | :--- |
| `main.ipynb` | O **Relatório Final**. Contém o código completo, EDA, modelos, otimização e a narrativa de resultados. |
| `winequality-red.csv` | O conjunto de dados original do vinho tinto. |
| `environment.yml` | Arquivo para recriar o ambiente Conda, garantindo a **reprodutibilidade total** das dependências. |
| `LICENSE` | Documento que especifica a licença de uso do código-fonte (MIT). |
| `.gitignore` | Configuração para ignorar arquivos de log (`logs.log`) e pastas de ambiente virtual (venv). |

---

## 🔗 Fonte de Dados e Licença

**Conjunto de Dados:** O trabalho utilizou o conjunto de dados **Red Wine Quality** de Cortez et al. (2009).

**Fonte Original (Kaggle/UCI):**
[UCI Wine Quality Dataset](https://www.kaggle.com/datasets/uciml/red-wine-quality-cortez-et-al-2009)

**Licença do Código:** Este código-fonte está sob a licença **MIT**.
