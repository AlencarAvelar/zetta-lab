# 📊 Análise Socioeconômica da Região Metropolitana de Belo Horizonte
### *Como o nível de educação e renda influencia o desenvolvimento humano*

---

## 🧭 **1. Contextualização**

O Brasil é um país marcado por fortes desigualdades sociais e regionais, onde fatores como **educação, renda e acesso a serviços básicos** impactam diretamente o **desenvolvimento humano**.  

Entender **como esses fatores se relacionam** é essencial para embasar políticas públicas eficazes e direcionadas às necessidades específicas de cada território.  

Neste projeto, focamos na **Região Metropolitana de Belo Horizonte (RMBH)**, utilizando dados do **Atlas do Desenvolvimento Humano no Brasil** para investigar **a influência da educação e da renda sobre o desenvolvimento humano**.

---

## 🎯 **2. Objetivo do Projeto**

Analisar e visualizar como o **nível de escolaridade** e a **renda** afetam o **Índice de Desenvolvimento Humano (IDHM)** nas Unidades de Desenvolvimento Humano (UDHs) da Região Metropolitana de Belo Horizonte (RMBH).

A análise busca responder:
> “Como o nível de educação e renda influencia o desenvolvimento humano nas regiões urbanas da RMBH?”

---

## 🧩 **3. Escopo da Análise**

### Desenvolvimento Humano
- IDHM	Índice de Desenvolvimento Humano Municipal
- IDHM_E	Componente Educação do IDHM
- IDHM_R	Componente Renda do IDHM
- IDHM_L	Componente Longevidade do IDHM
### Educação
- E_ANOSESTUDO	Média de anos de estudo da população
- I_ESCOLARIDADE	Índice de escolaridade
- I_FREQ_PROP	Índice de frequência escolar proporcional
### Renda
- GINI	Índice de Gini (medida de desigualdade de renda)
- RDPC	Renda per capita média 
### 🔹 Identificação Geográfica
- Código da unidade (`Cod_ID`)
- Nome da UDH (`NOME_UDH`)
- Município (`NOME_MUN`)

---

## 🧮 **4. Base de Dados Utilizada**

### 🗂️ Arquivos:
1. **dados-bh.xls**  
   - Contém dados das Unidades de Desenvolvimento Humano (UDHs) da Região Metropolitana de BH.   

2. **A - DICIONÁRIO dos indicadores do Atlas.xlsx**  
   - Dicionário com a descrição de cada variável presente na base principal.  
   - Utilizado para identificação das colunas relevantes à análise.

---

## 📚 **5. Análises Disponíveis**

Este repositório contém os seguintes notebooks de análise:

### `Analisys.ipynb`
Este notebook foca na análise exploratória das relações entre educação, renda e IDHM. As principais análises incluem:
- **Correlação entre Média de Anos de Estudo e IDHM**: Um gráfico de dispersão com linha de regressão mostra a relação entre a média de anos de estudo e o Índice de Desenvolvimento Humano Municipal (IDHM).
- **Correlação entre Renda Per Capita e IDHM**: Similarmente, um gráfico de dispersão com linha de regressão ilustra a relação entre a renda per capita e o IDHM.
- **Heatmap de Correlação**: Um mapa de calor exibe as correlações entre diversas variáveis relacionadas à educação, renda e IDHM, fornecendo uma visão geral das interdependências.
- **Ranking de UDHs por IDHM**: Gráficos de barras apresentam as 10 UDHs com maior e menor IDHM, destacando as áreas de melhor e pior desenvolvimento humano.

### `plot_geopandas.ipynb`
Este notebook utiliza a biblioteca `geopandas` para visualizar dados geográficos e socioeconômicos da RMBH. As análises geográficas incluem:
- **Mapa de IDHM**: Visualização do Índice de Desenvolvimento Humano Municipal (IDHM) distribuído geograficamente pelas UDHs da RMBH, utilizando um esquema de cores para indicar os níveis de desenvolvimento.
- **Mapa de Índice de Escolaridade**: Representação geográfica do Índice de Escolaridade (I_ESCOLARIDADE) nas UDHs.
- **Mapa de Renda Per Capita (RDPC)**: Visualização da Renda Per Capita (RDPC) por UDH.
- **Mapa de Coeficiente de Gini (GINI)**: Distribuição geográfica do Coeficiente de Gini, indicando a desigualdade de renda nas UDHs.

---

---

## 📈 **6. Resultado das Análises**

O presente relatório — **Zetta Lab Relatório de Análise Socioeconômica** — foi elaborado a partir das análises realizadas nos notebooks `Analisys.ipynb` e `plot_geopandas.ipynb`.  

Ele consolida os principais **resultados e visualizações** obtidos durante o estudo, apresentando uma visão integrada sobre como **educação, renda e desigualdade** influenciam o **desenvolvimento humano** na Região Metropolitana de Belo Horizonte (RMBH).

### 📎 **Anexo:** [Zetta_Lab_Relatorio.pdf](./Zetta_Lab_Relatorio.pdf)

Esses resultados reforçam a importância de políticas públicas voltadas à **redução das desigualdades educacionais e econômicas** para promover um desenvolvimento mais equilibrado na RMBH.

---


## 🗂️ **7. Estrutura do Projeto**

```
.
├── data  
│   ├── A - DICIONÁRIO dos indicadores do Atlas.xlsx
│   ├── raw
│   │   ├── dados-bh.xls
│   │   └── shapefiles/  # Contém os arquivos .shp, .dbf, .prj, .shx para geolocalização
│   ├── refined
│   │   └── base_udh_refined.csv
│   └── trusted
│       └── base_udh_trusted.csv
├── notebooks
│   ├── Analisys.ipynb
│   ├── etl_to_refined.ipynb
│   ├── etl_to_trusted.ipynb
│   ├── explore.ipynb
│   ├── plot_geopandas.ipynb
│   └── README.md
├── LICENSE
└── README.md
└── Zetta_Lab_Relatorio.pdf

```

---

## 📚 **8. Créditos e Referências**

- **Dados**: [Atlas do Desenvolvimento Humano no Brasil](https://atlasbrasil.org.br/)
- **Autor do Repositório**: Alencar Avelar

