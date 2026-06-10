# ⚡ Níveis de Risco para Queda de Raios na Região de São José dos Campos – SP

## 📖 Sobre o Projeto

Este repositório reúne os códigos desenvolvidos para o Trabalho de Conclusão de Curso (TCC) do MBA em Data Science e Analytics da USP/ESALQ.

O estudo investiga o comportamento do campo elétrico atmosférico durante tempestades e propõe uma metodologia para identificação de níveis de risco de queda de raios utilizando técnicas de análise estatística e aprendizado de máquina não supervisionado.

A pesquisa foi desenvolvida com dados provenientes da campanha CHUVA – Vale do Paraíba e tem como foco a região de São José dos Campos (SP), uma área monitorada por sensores de campo elétrico atmosférico (Electric Field Mill – EFM).

---

## 🎓 Informações Acadêmicas

**Título:** Níveis de risco para queda de raios na região de São José dos Campos – SP

**Autora:** Franciane Rodrigues

**Orientador:** William Barbosa

**Curso:** MBA em Data Science e Analytics

**Instituição:** USP/ESALQ

**Ano:** 2022

---

## 🎯 Objetivo

Avaliar o comportamento do campo elétrico atmosférico durante tempestades e identificar possíveis níveis de risco para ocorrência de descargas atmosféricas.

A pesquisa foi motivada pela seguinte questão:

> É possível identificar níveis de risco para queda de raios a partir do padrão de comportamento do campo elétrico atmosférico?

---

## 🌩️ Contexto

O Brasil é o país com maior incidência de raios do mundo, registrando aproximadamente 77,8 milhões de descargas atmosféricas por ano. Além dos riscos à vida humana, os raios geram impactos econômicos significativos em setores como energia, telecomunicações, construção civil, aviação e agronegócio.

Nesse contexto, sistemas de alerta baseados em sensores de campo elétrico atmosférico surgem como uma alternativa promissora para monitoramento e prevenção de eventos severos.

---

## 📡 Base de Dados

Os dados utilizados são provenientes da campanha:

**CHUVA – Vale do Paraíba (FAPESP 2009/15235-8)**

Período de coleta:

* Novembro de 2011 a Março de 2012

Foram utilizados dados de sete sensores de campo elétrico atmosférico distribuídos entre São José dos Campos, Vale do Paraíba e Região Metropolitana de São Paulo.

Os sensores registram continuamente a intensidade do campo elétrico atmosférico em unidades de Volt por metro (V/m).

---

## 🗺️ Localização dos Sensores

O projeto inclui a construção de mapas interativos utilizando Python e Folium para visualização espacial da rede de sensores.

Sensores utilizados na campanha:

* MET
* BIN
* AER
* PEQ
* IEAV
* IAG
* NOVADUTRA

A maior concentração dos instrumentos encontra-se no município de São José dos Campos (SP).

---

## 🔬 Metodologia

O estudo foi dividido em duas abordagens complementares.

### 1. Análise Exploratória de Dados

Foi realizada uma caracterização estatística dos valores absolutos de campo elétrico utilizando:

* Estatística descritiva;
* Tabelas de frequência;
* Quartis;
* Boxplots;
* Identificação de limiares de risco.

O objetivo foi compreender como o campo elétrico se comporta antes e durante eventos de tempestade.

---

### 2. Machine Learning Não Supervisionado

Foi aplicado o algoritmo:

**K-Means Clustering**

A técnica foi utilizada para identificar agrupamentos naturais nos dados de campo elétrico registrados durante uma tempestade ocorrida em 28 de novembro de 2011.

Foram avaliadas diferentes configurações:

* Dados brutos;
* Dados absolutos;
* Dados padronizados;
* Dados absolutos padronizados.

A determinação do número de grupos foi realizada utilizando o Método do Cotovelo (Elbow Method).

---

## 🤖 Tecnologias Utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-Learn
* Folium
* K-Means Clustering
* StandardScaler

---

## 📊 Principais Resultados

### Análise Estatística

A análise exploratória permitiu propor cinco níveis de classificação para o campo elétrico atmosférico:

| Nível            | Faixa de Campo Elétrico |
| ---------------- | ----------------------- |
| Ruído Eletrônico | Até 51 V/m              |
| Sem Risco        | Até 127 V/m             |
| Atenção          | 127 a 312 V/m           |
| Risco Alto       | 312 a 510 V/m           |
| Risco Extremo    | Acima de 510 V/m        |

Esses intervalos foram obtidos a partir da distribuição estatística dos dados observados durante tempestades.

---

### Agrupamento por K-Means

A aplicação do algoritmo K-Means também resultou na identificação de cinco grupos associados a diferentes níveis de risco.

Os agrupamentos foram interpretados como:

* Ruído eletrônico;
* Sem risco;
* Atenção;
* Risco alto;
* Risco extremo.

A utilização de valores absolutos apresentou melhor interpretação física dos resultados quando comparada aos dados brutos.

---

## 💡 Contribuições

Este trabalho demonstra o potencial da Ciência de Dados aplicada à Meteorologia e à Eletricidade Atmosférica.

Os resultados podem contribuir para:

* Sistemas de alerta de raios;
* Monitoramento de tempestades severas;
* Apoio à tomada de decisão em operações sensíveis ao clima;
* Desenvolvimento futuro de modelos preditivos para ocorrência de descargas atmosféricas.

---

## 🔭 Trabalhos Futuros

Como continuidade da pesquisa, são sugeridos:

* Testes com outros algoritmos de agrupamento;
* Inclusão de variáveis meteorológicas;
* Integração com sistemas de localização de raios;
* Desenvolvimento de modelos preditivos utilizando Machine Learning supervisionado;
* Avaliação de técnicas de Deep Learning para previsão de atividade elétrica atmosférica.

---

## 👩‍💻 Autora

Franciane Rodrigues

Física | Mestre em Meteorologia | Cientista de Dados

MBA em Data Science e Analytics – USP/ESALQ

GitHub: https://github.com/francianerod

