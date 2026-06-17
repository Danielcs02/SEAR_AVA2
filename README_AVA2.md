# Análise Facial com DeepFace — Reconhecimento de Expressões

Trabalho da disciplina **Sistemas Evolutivos e Aplicados à Robótica** — Universidade Veiga de Almeida (UVA).

## Sobre

Análise facial automatizada utilizando a biblioteca **DeepFace**, aplicada a cinco fotografias com diferentes expressões faciais (brava, triste, surpresa, neutra e feliz). O estudo avalia a capacidade do modelo em identificar atributos como idade, gênero, emoção e etnia.

## Resultados

| Expressão | Idade | Gênero | Emoção Detectada | Confiança | Etnia |
|-----------|-------|--------|------------------|-----------|-------|
| Brava | 23 | Man (100%) | angry | 64,40% | latino hispanic |
| Triste | 24 | Man (100%) | neutral | 66,60% | latino hispanic |
| Surpresa | 24 | Man (98,7%) | neutral | 92,33% | asian |
| Neutra | 23 | Man (100%) | neutral | 82,54% | latino hispanic |
| Feliz | 27 | Man (99,8%) | happy | 90,49% | latino hispanic |

**Observações:**
- O modelo classificou corretamente 3 das 5 expressões (brava, neutra e feliz)
- Expressões mais sutis (triste e surpresa) foram identificadas como neutras
- A estimativa de idade variou entre 23 e 27 anos
- O gênero foi corretamente identificado em todas as imagens

## Como executar

### Pré-requisitos

- Conta no [Google Colab](https://colab.research.google.com/)
- 5 fotografias com expressões faciais distintas para upload

### Passos

1. Abra o arquivo `notebook.ipynb` no Google Colab
2. Execute a primeira célula para instalar a biblioteca DeepFace
3. Execute as células seguintes — quando o upload for solicitado, selecione suas fotografias
4. Os resultados serão exibidos no console após a análise de cada imagem

### Bibliotecas utilizadas

- [DeepFace](https://github.com/serengil/deepface) — biblioteca de reconhecimento e análise facial
- [OpenCV](https://opencv.org/) — manipulação e visualização de imagens
- [NumPy](https://numpy.org/) — operações com arrays
- [Requests](https://requests.readthedocs.io/) — download de imagens via URL

## Estrutura do projeto

```
├── notebook.ipynb    # Notebook principal com a análise facial
├── README.md         # Este arquivo
```

## Referências

- [DeepFace — Documentação Oficial](https://github.com/serengil/deepface)
- [DataCamp — A Beginner's Guide to Facial Recognition with DeepFace](https://www.datacamp.com/tutorial/face-recognition-python-deepface)
- [OpenCV Documentation](https://docs.opencv.org/)
