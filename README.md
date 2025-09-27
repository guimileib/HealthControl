# 🏃‍♂️ Health Control - Análise de Padrões Sono vs Atividade Física

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-green.svg)](https://scikit-learn.org/)
[![License](https://img.shields.io/badge/License-MIT-red.svg)](LICENSE)

## 📋 Sobre o Projeto

Este projeto aplica a metodologia **Knowledge Discovery in Databases (KDD)** para analisar padrões entre qualidade do sono e atividade física, utilizando técnicas de **Machine Learning** para descobrir insights e desenvolver modelos preditivos.

### 🎯 Objetivos
- **Clusterização**: Identificar grupos ocultos de padrões sono-atividade
- **Classificação**: Prever performance diária baseada em dados de sono
- **Insights**: Descobrir correlações práticas para otimização de rotinas de saúde

## 🔬 Metodologia KDD

O projeto segue rigorosamente as 5 fases da metodologia KDD:

| Fase | Descrição | Implementação |
|------|-----------|---------------|
| **1. Seleção** | Identificação do problema e dados relevantes | Filtro temporal, exploração inicial |
| **2. Pré-processamento** | Limpeza e preparação dos dados | Remoção de outliers, tratamento de missing |
| **3. Transformação** | Engenharia de features | Criação de 8 features derivadas |
| **4. Mineração** | Aplicação de algoritmos ML | K-means + Random Forest |
| **5. Interpretação** | Avaliação e validação | Métricas, visualizações, insights |

## 📊 Resultados Principais

### 🎯 Clusterização (K-means)
- **7 clusters** identificados com diferentes padrões sono-atividade
- **Silhouette Score**: 0.269
- **Melhor padrão**: Performance de 100% em cluster específico

### 🌲 Classificação (Random Forest)
- **Acurácia**: 60.6% na predição de performance diária
- **Feature mais importante**: Horário de dormir (0.386)
- **Insight**: Regularidade > Duração total do sono

## 🗂️ Estrutura do Projeto

```
health_control/
├── 📁 data/                          # Dados sintéticos
│   ├── synthetic_health_export.xml   # Dados em formato Apple Health
│   └── synthetic_health_summary.csv  # Resumo em CSV
├── 📓 health_control_github.ipynb    # Notebook principal (versão GitHub)
├── 🐍 generate_synthetic_data.py     # Script gerador de dados sintéticos
├── 📄 health_control_ieee_paper.tex  # Relatório IEEE em LaTeX
├── 📋 requirements.txt               # Dependências do projeto
├── 🎯 .gitignore                     # Arquivos ignorados pelo Git
└── 📖 README.md                      # Este arquivo
```

## 🚀 Como Usar

### 1. Clone o Repositório
```bash
git clone https://github.com/guimileib/HealthControl.git
cd HealthControl
```

### 2. Instale as Dependências
```bash
pip install -r requirements.txt
```
### 3. Importe seus dados do app Saúde 
```bash
exportar.xml
```

## 📦 Dependências

- **pandas** >= 1.3.0 - Manipulação de dados
- **numpy** >= 1.21.0 - Computação numérica
- **scikit-learn** >= 1.0.0 - Machine Learning
- **matplotlib** >= 3.4.0 - Visualizações
- **seaborn** >= 0.11.0 - Visualizações estatísticas
- **jupyter** >= 1.0.0 - Ambiente de notebooks

Instale todas as dependências com:
```bash
pip install -r requirements.txt
```

## 📈 Visualizações

O projeto gera 4 visualizações principais:

1. **Distribuição dos Clusters** - Tamanho de cada grupo identificado
2. **Sono vs Energia por Cluster** - Scatter plot colorido por cluster
3. **Importância das Features** - Ranking das variáveis mais preditivas
4. **Performance por Cluster** - Taxa de sucesso por padrão identificado

## 📊 Exemplo de Uso

```python
# Carregar dados originais do seu apple watch
import pandas as pd
dados_originais = pd.read_xml("exportar.xml")

```

## 📚 Referências Científicas

- Fayyad, U., Piatetsky-Shapiro, G., & Smyth, P. (1996). *From data mining to knowledge discovery in databases*
- Han, J., Pei, J., & Kamber, M. (2011). *Data mining: concepts and techniques*
- Walker, M. (2017). *Why We Sleep: Unlocking the Power of Sleep and Dreams*

## 🤝 Contribuições

Contribuições são bem-vindas! Por favor, siga estas diretrizes:

1. **Fork** o projeto
2. **Crie** uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. **Commit** suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. **Push** para a branch (`git push origin feature/AmazingFeature`)
5. **Abra** um Pull Request

## 📝 TODO List

- [ ] Implementar algoritmos de Deep Learning
- [ ] Criar dashboard web interativo
- [ ] Adicionar mais métricas de validação
- [ ] Expandir para dados de múltiplos usuários
- [ ] Incluir análise de séries temporais

## 📄 Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.

## 👨‍💻 Autor

**Guilherme Lima**
- GitHub: [@guimileib](https://github.com/guimileib)
- LinkedIn: [Guilherme Lima](https://www.linkedin.com/in/guimileib/)
- Email: guilhermemileib@gmail.com

## 🙏 Agradecimentos

- Apple Inc. pela inspiração na estrutura de dados do Apple Health
- Comunidade Python pela excelente documentação
- Contribuidores do scikit-learn pelas ferramentas de ML
- Professor Leandro Nogueira

---

⭐ **Se este projeto foi útil para você, considere dar uma estrela!** ⭐

## 📞 Suporte

Se você encontrar algum problema ou tiver dúvidas:

1. Verifique a seção [Issues](https://github.com/guimileib/HealthControl/issues)
2. Crie uma nova issue com detalhes do problema
3. Entre em contato através do email: guilhermemileib@gmail.com

---

**🔬 Ciência de Dados + 🏃‍♂️ Saúde = 📊 Insights Poderosos**
