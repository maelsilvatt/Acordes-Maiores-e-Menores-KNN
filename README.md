# Classificação de Acordes Musicais com KNN

Este projeto tem como objetivo classificar acordes musicais em maiores ou menores utilizando técnicas de processamento de áudio e aprendizado de máquina. Foram utilizados 100 arquivos de áudio no formato WAV (50 acordes maiores e 50 menores).

## 📌 Visão Geral

O projeto consiste nas seguintes etapas principais:

1. **Extração de Features**: Utilização da biblioteca Librosa para extrair características relevantes dos áudios.
2. **Análise Exploratória**: Visualização das features e suas correlações.
3. **Pré-processamento**: Normalização dos dados.
4. **Seleção de Features**: Identificação das características mais importantes usando Random Forest.
5. **Classificação**: Implementação de um classificador KNN manual e comparação com a versão do Scikit-Learn.

## 📂 Estrutura do Projeto

```
/projeto-classificacao-acordes
│
├── /data
│   └── Acordes.zip       # Arquivo contendo os samples de áudio
│
├── classificacao_acordes.ipynb  # Notebook principal com todo o código
│
└── README.md             # Este arquivo
```

## 🛠️ Tecnologias Utilizadas

- Python 3
- Bibliotecas:
  - Librosa (processamento de áudio)
  - NumPy, Pandas (manipulação de dados)
  - Matplotlib, Seaborn (visualização)
  - Scikit-Learn (machine learning)

## 🔍 Principais Features Extraídas

- **Chroma Features**: Representação cromática do espectro (importante para reconhecimento de acordes)
- **MFCCs**: Coeficientes cepstrais em frequência mel (características timbrais)
- **Tonnetz**: Representação tonal espaço-temporal
- **RMS**: Energia do sinal
- **Razão Harmônica/Percussiva**

## 📊 Resultados

O modelo KNN alcançou uma acurácia média de ~90% na classificação de acordes maiores e menores, utilizando as melhores features identificadas pelo Random Forest.

| Método         | Acurácia Média |
|----------------|----------------|
| KNN Manual     | ~90%           |
| KNN (Sklearn)  | ~90%           |

## 🚀 Como Executar

1. Extraia o arquivo `Acordes.zip` na pasta `/data`
2. Execute o notebook Jupyter `classificacao_acordes.ipynb` (todas as dependências estão listadas no notebook)

## 📚 Referências

- Documentação Librosa: https://librosa.org/doc/latest/index.html
- Scikit-Learn KNN: https://scikit-learn.org/stable/modules/neighbors.html

## ✉️ Contato

Para dúvidas ou sugestões, entre em contato com o autor do projeto.
