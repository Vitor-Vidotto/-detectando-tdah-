# 🧠 Detectando TDAH com Tweets usando Machine Learning

Este projeto utiliza Machine Learning para identificar possíveis indícios de **TDAH (Transtorno de Déficit de Atenção com Hiperatividade)** com base em **tweets públicos de usuários**, utilizando dados extraídos do repositório [IEEE DataPort](https://ieee-dataport.org/documents/twitter-dataset-mental-disorders-detection).

> ⚠️ **Este projeto tem finalidade educacional e de pesquisa. Não substitui diagnóstico clínico.**

---

## 📂 Dataset

Fonte: [Twitter Dataset for Mental Disorders Detection](https://ieee-dataport.org/documents/twitter-dataset-mental-disorders-detection)

O dataset contém tweets categorizados em:
- `Adhd`
- `Depression`
- `PTSD`
- `Control`
  
Neste projeto, focamos na distinção entre `Adhd` e `Control`.

---

## 📦 Instalação

1. **Clone o repositório:**
```bash
git clone https://github.com/seu-usuario/detectando-tdah.git
cd detectando-tdah
```
2.**Crie e ative um ambiente virtual (opcional mas recomendado):**
```
python -m venv .venv
source .venv/bin/activate  # Linux/macOS
.venv\Scripts\activate     # Windows
```
3. **Instale as dependências:**
```
pip install -r requirements.txt
```
## Executando o Notebook
1. **Abra o Jupyter Notebook:**

```
jupyter notebook
```
2. **Abra o arquivo Detectando_TDAH.ipynb.**

3. **Execute as células em ordem. Elas incluem:**

Importação de bibliotecas

Leitura dos dados

Pré-processamento

Treinamento de modelos

Avaliação de desempenho

🗃️ **Estrutura do Projeto**

📁 detectando-tdah/
├── Detectando_TDAH.ipynb        # Notebook principal
├── requirements.txt             # Dependências Python
└── README.md      

📈 **Técnicas Utilizadas**
* Vetorização: TF-IDF

* Balanceamento: Reamostragem com resample

* Modelos de Classificação:

* Naive Bayes

* Regressão Logística

* SVM (LinearSVC)

* Árvore de Decisão

* Random Forest

* Gradient Boosting

**Avaliação:**

* Accuracy

* F1-score

* Matriz de Confusão

📊**Exemplo de Resultados**
* Precisão média entre os modelos: ~65% (dependendo da divisão e do balanceamento)

* F1-score: particularmente útil para lidar com desbalanceamento entre Adhd e Control

🧼 **Pré-processamento**
* Remoção de emojis e URLs

* Normalização de texto

* Foco apenas em tweets com rótulo Adhd ou Control

* Armazenamento em CSV intermediário

💡 **Melhorias Futuras**
* Adicionar validação cruzada (cross-validation)

* Explorar embeddings mais robustos (Word2Vec, BERT)

* Construir uma API REST ou dashboard interativo

* Avaliar modelos Deep Learning com LSTM ou Transformers

👨‍⚕️ **Aviso Legal**
Este projeto tem caráter acadêmico e experimental. Não se destina a diagnósticos médicos. O uso indevido ou interpretação incorreta pode trazer riscos. Sempre consulte um profissional de saúde.

