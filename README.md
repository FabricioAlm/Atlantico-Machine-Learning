# 🤖 Atlântico - Aprendizado de Máquina

Bem-vindo ao repositório do curso **Machine Learning e Dados**!  
Aqui você encontrará atividades teóricas, exercícios práticos em Python, notebooks interativos e datasets para análise e modelagem.

---

## 📂 Estrutura do Repositório
- 📘 **Atividade1** → Questões conceituais sobre Machine Learning  
- 💻 **Atividade2** → Exercícios práticos de programação em Python e análise de dados  
- 📓 **Atlântico_Atividade2.ipynb** → Notebook com código da atividade 2 (executável no Colab)  
- 📊 **trem.csv** → Dataset para uso nos exercícios de classificação  

---

## 📝 Atividade 1 (ATIV-01)
Questões conceituais sobre Machine Learning:

1. **O que é Machine Learning?**  
   Subcampo da IA que cria modelos a partir de dados para tomada de decisão ou previsões, aprendendo conforme o processamento é realizado.

2. **Conjuntos de treinamento, validação e teste**  
   - Treinamento: ajuste de parâmetros para criar o modelo.  
   - Validação: ajuste de hiperparâmetros.  
   - Teste: avaliar desempenho em dados novos.

3. **Dados ausentes**  
   Devem ser tratados, por exemplo, removendo linhas incompletas para não comprometer o modelo.

4. **Matriz de confusão**  
   Permite avaliar acertos e erros (VP, VN, FP, FN) e calcular métricas como acurácia, precisão, recall e F1-score.

5. **Áreas de aplicação**  
   Saúde (previsão de patologias), indústria (previsão de vendas), meio ambiente (detecção de poluição), inspeções visuais etc.

---

## 📝 Atividade 2 (ATIV-02)
Exercícios práticos de programação em Python e análise de dados:

### 🔹 Parte 1 – Python
1. Função que retorna números ímpares de uma lista.  
2. Função que retorna números primos de uma lista.  
3. Função que retorna elementos exclusivos entre duas listas.  
4. Função que encontra o segundo maior valor em uma lista.  
5. Função que ordena lista de tuplas (nome, idade) por nome.

### 🔹 Parte 2 – Análise de Dados com Pandas
6. Identificação e tratamento de outliers (desvio padrão ou quartis).  
7. Concatenar vários DataFrames com `pd.concat()`.  
8. Ler arquivo CSV em DataFrame e exibir primeiras linhas.  
9. Selecionar coluna e filtrar linhas com condição.  
10. Tratar valores ausentes (NaN) em DataFrame.

---

## 📊 Dataset
O arquivo **trem.csv** contém a lista de imagens e suas respectivas categorias, utilizado para os exercícios de classificação.  
Ele já está disponível neste repositório e pode ser lido diretamente no Google Colab com o seguinte código:

```python
import pandas as pd

url = "https://raw.githubusercontent.com/FabricioAlm/Atlantico-Aprendizado-de-Maquina/principal/trem.csv"
df = pd.read_csv(url, sep=";")  # separador ; conforme estrutura do arquivo
df.head()

