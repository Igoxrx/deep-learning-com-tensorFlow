# Deep Learning com TensorFlow

## Resumo

Este repositório contém um Jupyter Notebook dedicado à resolução de exercícios práticos que envolvem a construção, o treinamento e a avaliação de Redes Neurais Artificiais (ANN). O projeto utiliza a biblioteca TensorFlow para a modelagem profunda de dados, focando na extração de métricas de desempenho para problemas complexos de classificação ou regressão. A abordagem inclui desde o design da arquitetura das camadas até a análise de convergência do modelo.

## Dependências e Requisitos

* **Linguagem:** Python 3.x
* **Bibliotecas:** * `tensorflow`: Para criação e treinamento das redes neurais.
    * `scikit-learn`: Para pré-processamento de dados e divisão de conjuntos.
    * `pandas` e `numpy`: Para manipulação e tratamento de estruturas de dados.
    * `matplotlib`: Para visualização de curvas de aprendizado (loss e acurácia).
* **Ferramentas:** Jupyter Notebook, JupyterLab ou Google Colab.

## Instruções de Instalação e Execução

Para reproduzir os experimentos contidos neste projeto, siga as etapas abaixo:

1.  **Arquivos Necessários:**
    Realize o download do arquivo `aprendizado de máquina com tensorflow.ipynb` para o seu diretório de trabalho.

2.  **Instalação de Dependências:**
    Instale as bibliotecas necessárias através do terminal utilizando o comando:
    ```bash
    pip install tensorflow scikit-learn pandas numpy matplotlib jupyter
    ```

3.  **Inicialização:**
    Inicie o ambiente do Jupyter em sua máquina:
    ```bash
    jupyter notebook
    ```

4.  **Execução:**
    Abra o notebook pelo navegador. Certifique-se de que os datasets referenciados na atividade estejam localizados no mesmo diretório do arquivo `.ipynb` antes de executar as células de forma sequencial.

## Exemplo de Uso

O notebook demonstra o fluxo de trabalho essencial para Deep Learning, integrando o TensorFlow com ferramentas de engenharia de recursos do Scikit-Learn:

```python
import tensorflow as tf
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler

# Fluxo de preparação contido no notebook:
# Divisão dos dados em treino e teste
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)

# Normalização de recursos para facilitar a convergência da rede
scaler = StandardScaler()
X_train_scaled = scaler.fit_transform(X_train)
X_test_scaled = scaler.transform(X_test)
```

---

## Licença

Este material possui finalidade acadêmica, servindo como registro de estudos.
