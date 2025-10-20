# Análise Epidemiológica da Síndrome Congênita do Zika (SCZ) em Pernambuco

## 📊 Análise Temporal, Espacial e Estatística (2015-2024)

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.0+-green.svg)](https://pandas.pydata.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Completo-success.svg)]()

---

## 👩‍🔬 Autora

**Giovanna Clócate Cavalcante de Almeida**

📧 Contato: [giovanna.clocate2004@exemplo.com]  
🔗 LinkedIn: [https://www.linkedin.com/in/giovanna-cl%C3%B3cate-34aa84289/]  

---

## Sobre o Projeto

Este repositório contém uma análise epidemiológica completa dos casos de Síndrome Congênita do Zika (SCZ) notificados no estado de Pernambuco entre as Semanas Epidemiológicas 30/2015 e 52/2024.

O estudo aborda três dimensões principais:

1. **📈 Análise Temporal**: Evolução dos casos ao longo de 9 anos
2. **🗺️ Análise Espacial**: Distribuição geográfica por Regiões de Saúde
3. **🔬 Análise Estatística**: Testes de hipóteses e identificação de fatores associados

### 🎯 Objetivos

- Descrever temporalmente os casos de SCZ (2015–2024)
- Mapear a distribuição espacial dos casos por Região de Saúde
- Determinar fatores associados à classificação final dos casos
- Aplicar testes estatísticos para validar achados
- Produzir relatório técnico com mapas, tabelas e interpretações

---

## 🗂️ Estrutura do Repositório

```
📁 scz-pernambuco-analise/
│
├── 📓 notebook/
│   └── analise_scz_pernambuco.ipynb          # Notebook Jupyter completo
│
├── 📊 data/
│   ├── scz_pernambuco_tabela1.csv            # Dados por Região de Saúde
│   ├── scz_pernambuco_tabela2.csv            # Dados temporais (2015-2024)
│   ├── scz_pernambuco_tabela3.csv            # Características dos casos
│   └── municipios_pe.shp                     # Shapefile IBGE (opcional)
│
│
├── 📄 relatório/
│   ├── relatorio_zika.pdf             # Relatório em PDF
│
│
│
├── 📖 README.md                               # Este arquivo

```

---

## 🔧 Requisitos e Instalação

### Pré-requisitos

- Python 3.8 ou superior
- Jupyter Notebook ou JupyterLab
- Git (para clonar o repositório)

### Instalação

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/scz-pernambuco-analise.git
cd scz-pernambuco-analise

# Crie um ambiente virtual (recomendado)
python -m venv venv
source venv/bin/activate  # Linux/Mac
# ou
venv\Scripts\activate  # Windows


### 📦 Dependências Principais

```python
pandas>=2.0.0
numpy>=1.24.0
matplotlib>=3.7.0
seaborn>=0.12.0
scipy>=1.10.0
geopandas>=0.13.0  
jupyterlab>=4.0.0
```

---

## 🚀 Como Usar

### Opção 1: Notebook Jupyter 

```bash
# Inicie o Jupyter
jupyter notebook

# Abra o arquivo:
# notebooks/analise_scz_pernambuco.ipynb
```

### Opção 2: Script Python

```bash
# Execute o script standalone
python scripts/analise_scz.py
```
---

## 📊 Dados Utilizados

### Fonte de Dados

**Boletins Epidemiológicos Trimestrais da Síndrome Congênita do Zika**  
Secretaria Estadual de Saúde de Pernambuco (SES-PE)  
Período: SE 30/2015 a SE 52/2024

### Tabelas Incluídas

| Tabela | Descrição | Variáveis |
|--------|-----------|-----------|
| **Tabela 1** | Distribuição por Região de Saúde | Região, Confirmado, Descartado, Inconclusivo, Em Investigação |
| **Tabela 2** | Distribuição temporal anual | Ano, Classificação Final (2015-2024) |
| **Tabela 3** | Características dos casos | Sexo, Tipo de Notificação, Presença de Microcefalia |

### 🗺️ Dados Geoespaciais (Opcional)

- **Malha Municipal Digital**: IBGE (2020)
- **Formato**: Shapefile (.shp)
- **Sistema de Coordenadas**: SIRGAS 2000 (EPSG:4674)

---

## 📈 Principais Resultados

### 🔍 Achados Gerais

- **Total de Casos Notificados**: 3.135
- **Casos Confirmados**: 471 (15,0%)
- **Período de Pico**: 2015-2016 (71,3% das notificações)
- **Declínio**: 96,2% entre 2015 e 2024

### 🗺️ Distribuição Espacial

- **Região Mais Afetada**: Região I - Recife e RMR (52,0% dos confirmados)
- **Segunda Região**: Região IV - Caruaru (15,9% dos confirmados)
- **Concentração**: RS I e IV concentram 67,9% dos casos

### 📊 Características dos Casos

- **Predomínio Feminino**: 60,7% (p < 0,001)
- **Microcefalia Confirmada**: 51,3% dos casos
- **Notificação Neonatal**: 89,8% ≤28 dias de vida

### 📉 Análise Estatística

| Teste | Estatística | p-valor | Interpretação |
|-------|-------------|---------|---------------|
| **Qui-quadrado Temporal** | χ² = 4.127,6 | < 0,001 | Distribuição não uniforme |
| **Spearman (Tendência)** | ρ = -0,976 | < 0,001 | Forte declínio temporal |
| **Qui-quadrado Espacial** | χ² = 897,3 | < 0,001 | Concentração espacial |
| **Teste Binomial (Sexo)** | Z = 12,7 | < 0,001 | Predominância feminina |

---

## 📝 Metodologia

### Desenho do Estudo

**Tipo**: Estudo descritivo de série temporal com análise de distribuição espacial

**Abordagem**: Análise de dados secundários

### Análises Realizadas

#### 1️⃣ **Análise Descritiva**
- Frequências absolutas e relativas
- Medidas de tendência central e dispersão
- Taxas de confirmação por ano e região

#### 2️⃣ **Análise Temporal**
- Série temporal (2015-2024)
- Teste de Qui-quadrado para uniformidade
- Correlação de Spearman para tendência

#### 3️⃣ **Análise Espacial**
- Distribuição por Região de Saúde
- Identificação de clusters de alta incidência
- Mapas temáticos (coropléticos)

#### 4️⃣ **Testes Estatísticos**
- Qui-quadrado (χ²)
- Correlação de Spearman (ρ)
- Teste Binomial
- Nível de significância: α = 0,05

---

## 📚 Documentação Adicional

### 📖 Relatório Técnico Completo

Acesse o [relatório técnico completo](relatorios/relatorio_tecnico_scz.md) com:

- Introdução e contextualização
- Metodologia detalhada
- Resultados com interpretação epidemiológica
- Discussão aprofundada
- Conclusões e recomendações
- Referências bibliográficas


## 📜 Licença

Este projeto está licenciado sob a **Licença MIT** - veja o arquivo [LICENSE](LICENSE) para detalhes.

### ⚠️ Disclaimer

Os dados utilizados são de domínio público, provenientes de boletins epidemiológicos oficiais. A análise foi realizada para fins acadêmicos e de vigilância em saúde pública. As interpretações e conclusões são de responsabilidade da autora.

---

## 🔗 Links Úteis

- 🏥 [Secretaria de Saúde de Pernambuco](http://portal.saude.pe.gov.br/)
- 📊 [Boletins Epidemiológicos SCZ](http://portal.saude.pe.gov.br/boletins)
- 🗺️ [IBGE - Malhas Territoriais](https://www.ibge.gov.br/geociencias/downloads-geociencias.html)
- 🦟 [Ministério da Saúde - Zika](https://www.gov.br/saude/pt-br/assuntos/saude-de-a-a-z/z/zika-virus)
- 📚 [PAHO - Zika Virus](https://www.paho.org/en/topics/zika)

---

## 📞 Contato

**Giovanna Clócate Cavalcante de Almeida**

- 📧 Email: [giovanna.clocate2004@gmail.com]
- 💼 LinkedIn: [linkedin.com/in/seu-perfil](https://www.linkedin.com/in/giovanna-clócate-34aa84289/)
- 🐙 GitHub: [@seu-usuario](https://github.com/giclocate)
- 🎓 Lattes: [lattes.cnpq.br/seu-id](http://lattes.cnpq.br/0116133424195806)

