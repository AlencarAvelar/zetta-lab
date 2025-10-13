# 📊 Análise Socioeconômica da Região Metropolitana de Belo Horizonte  
### *Como o nível de educação e renda influencia o desenvolvimento humano*

---

## 🧭 **1. Contextualização**

O Brasil é um país marcado por fortes desigualdades sociais e regionais, onde fatores como **educação, renda e acesso a serviços básicos** impactam diretamente o **desenvolvimento humano**.  

Entender **como esses fatores se relacionam** é essencial para embasar políticas públicas eficazes e direcionadas às necessidades específicas de cada território.  

Neste projeto, focamos na **Região Metropolitana de Belo Horizonte (RMBH)**, utilizando dados do **Atlas do Desenvolvimento Humano no Brasil (PNUD, IPEA e FJP)** para investigar **a influência da educação e da renda sobre o desenvolvimento humano**.

---

## 🎯 **2. Objetivo do Projeto**

Analisar e visualizar como o **nível de escolaridade** e a **renda** afetam o **Índice de Desenvolvimento Humano (IDH)** na Região Metropolitana de Belo Horizonte.

A análise busca responder:
> “Como o nível de educação e renda influencia o desenvolvimento humano nas regiões urbanas da RMBH?”

---

## 🧩 **3. Escopo da Análise**

### 🔹 Variável Dependente
- **IDHM (Índice de Desenvolvimento Humano Municipal)** — indicador composto que mede desenvolvimento humano em:
  - **Educação (IDHM_E)**
  - **Renda (IDHM_R)**
  - **Longevidade (IDHM_L)**

### 🔹 Variáveis Explicativas
- **Educação:**
  - Média de anos de estudo (`MEDIA_ANOS_ESTUDO`)
  - Taxa de analfabetismo (`T_ANALF15M`)
  - Frequência escolar (`I_FREQ_PROP`, `T_FREQ5A14`, `T_FREQ15A17`)
- **Renda:**
  - Renda per capita (`RENDAPC`)
  - Renda média (`RENDAMED`)
  - Índice de Gini (`GINI`)
  - Proporção de pobreza e extrema pobreza (`POBREZA`, `EXTREMA_POBREZA`)

### 🔹 Identificação Geográfica
- Código da unidade (`Cod_ID`)
- Nome da UDH (`NOME_UDH`)
- Município (`NOME_MUN`)

---

## 🧮 **4. Base de Dados Utilizada**

### 🗂️ Arquivos:
1. **RM 63100 Belo Horizonte - Base UDH 2000_2010.xlsx**  
   - Contém dados das Unidades de Desenvolvimento Humano (UDHs) da Região Metropolitana de BH.  
   - 1.246 linhas e 237 colunas (dados detalhados sobre demografia, educação, renda e IDH).  
   - Fonte: [Atlas do Desenvolvimento Humano no Brasil](https://atlasbrasil.org.br/)

2. **A - DICIONÁRIO dos indicadores do Atlas.xlsx**  
   - Dicionário com a descrição de cada variável presente na base principal.  
   - Utilizado para identificação das colunas relevantes à análise.

---

## ⚙️ **5. Etapas Realizadas**

### 🧠 1️⃣ Definição do tema e escopo
- Tema original: *impactos socioeconômicos no Brasil*  
- Recorte definido: *análise do desenvolvimento humano, educação e renda na Região Metropolitana de BH.*

### 📊 2️⃣ Obtenção e compreensão dos dados
- Identificação de fontes oficiais (Atlas Brasil - PNUD/IPEA/FJP).  
- Leitura dos arquivos `.xlsx` e reconhecimento da estrutura da base (`Sheet1` com dados principais).  

### 🧾 3️⃣ Identificação das variáveis relevantes
- Seleção das colunas necessárias para análise (IDHM, Educação e Renda).  
- Exclusão planejada das demais variáveis (saúde, saneamento, demografia etc.).  

### 🧹 4️⃣ Planejamento do pré-processamento
- Seleção de colunas de interesse.  
- Padronização de tipos e tratamento de valores ausentes.  
- Salvamento de uma versão limpa em CSV para análises estatísticas e visuais.

---

## 📈 **6. Próximos Passos**

1. **Pré-processamento**
   - Dropar colunas irrelevantes  
   - Tratar valores nulos e padronizar nomes  
   - Normalizar e converter variáveis numéricas  

2. **Análise exploratória**
   - Estatísticas descritivas (média, desvio, distribuição)  
   - Correlações entre escolaridade, renda e IDHM  
   - Identificação de outliers e padrões regionais  

3. **Visualização de dados (Dashboard)**
   - Gráficos de correlação  
   - Mapas de calor e gráficos comparativos por município  
   - Dashboard interativo com análise da desigualdade intraurbana  

4. **Interpretação e Conclusões**
   - Avaliar o impacto da escolaridade e renda sobre o desenvolvimento humano  
   - Identificar regiões com maior vulnerabilidade e desigualdade  

---


## 📚 **8. Referências**

- [Atlas do Desenvolvimento Humano no Brasil (PNUD/Ipea/FJP)](https://atlasbrasil.org.br/)  