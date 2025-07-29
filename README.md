# 🔋 Energy Consumption Analysis with Clustering

Este projeto utiliza técnicas de **análise exploratória**, **redução de dimensionalidade (PCA)** e **agrupamento (KMeans)** para identificar padrões no consumo de energia elétrica a partir de um dataset com medições reais.

---

## 📊 Objetivo

O objetivo principal deste notebook é aplicar **PCA** para redução de dimensionalidade e **KMeans** para agrupar padrões de consumo de energia com base em diversas variáveis, como:

- Potência ativa e reativa
- Tensão
- Corrente
- Submedições de energia

---

## 🧪 Técnicas utilizadas

- **Normalização** dos dados com `MinMaxScaler`
- **Redução de dimensionalidade** com `PCA` (Principal Component Analysis)
- **Clustering** com `KMeans` e análise do número ideal de clusters
- **Métricas de avaliação**, como:
  - **Soma das distâncias intra e inter-clusters**
  - **Silhouette Score**
- **Visualização dos clusters** com `matplotlib`

---

## 📁 Estrutura dos dados

As colunas utilizadas na análise incluem:

- `Global_active_power`
- `Global_reactive_power`
- `Voltage`
- `Global_intensity`
- `Sub_metering_1`
- `Sub_metering_2`
- `Sub_metering_3`

Essas variáveis representam diferentes formas de medição do consumo de energia em uma residência.

---

## 🧠 Principais etapas do notebook

1. **Carregamento e normalização dos dados**
2. **Divisão em amostras para treino e avaliação**
3. **Aplicação do PCA**
4. **Determinação do número ideal de clusters**
5. **Treinamento do modelo KMeans**
6. **Visualização dos clusters**
7. **Análise com Silhouette Score**
8. **Criação de um mapa de clusters com os dados originais**

---

## 📈 Visualizações

- Gráficos dos clusters reduzidos para 2 dimensões com PCA
- Centróides destacados em preto
- Avaliação visual do agrupamento com diferentes valores de *k*

---

## 🛠️ Requisitos

Você pode instalar os pacotes necessários com:

```bash
pip install numpy pandas matplotlib scikit-learn scipy
