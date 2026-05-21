# Atividade Overfitting e Underfitting - Deep Learning

Este projeto foi desenvolvido para a atividade prática de Deep Learning do Encontro 12.

O objetivo é demonstrar, usando o dataset Fashion MNIST, os conceitos de:

- Underfitting
- Overfitting
- Regularização com Dropout
- EarlyStopping

## Estrutura do Projeto

encontro12/
├── atividade_overfitting.ipynb
├── requirements.txt
└── README.txt

## Bibliotecas Utilizadas

- TensorFlow: criação e treinamento dos modelos de rede neural
- Keras: construção das camadas dos modelos
- NumPy: operações matemáticas e manipulação dos dados
- Matplotlib: criação dos gráficos de acurácia

## Como Executar o Projeto

1. Criar e ativar o ambiente virtual:

Windows:

python -m venv venv
venv\Scripts\activate

2. Instalar as dependências:

pip install -r requirements.txt

3. Abrir o notebook no VS Code:

atividade_overfitting.ipynb

4. Executar as células em ordem.

## Etapas da Atividade

### 1. Carregamento dos Dados

Foi utilizado o dataset Fashion MNIST, disponível no Keras.

### 2. Normalização dos Dados

Os valores dos pixels foram divididos por 255.0 para ficarem entre 0 e 1.

### 3. Modelo com Underfitting

Foi criado um modelo simples, com poucos neurônios, para demonstrar baixa capacidade de aprendizado.

### 4. Modelo com Overfitting

Foi criado um modelo mais complexo, com várias camadas densas, para demonstrar memorização excessiva dos dados de treino.

### 5. Modelo com Regularização

Foi utilizado Dropout para reduzir o overfitting e EarlyStopping para interromper o treinamento quando a perda de validação parasse de melhorar.

## Conclusão

O modelo simples apresentou underfitting, pois não conseguiu aprender bem os padrões dos dados.

O modelo mais complexo apresentou overfitting, pois teve desempenho melhor no treino do que na validação.

O modelo com regularização apresentou melhor generalização, pois usou Dropout e EarlyStopping para reduzir a memorização excessiva e melhorar o desempenho em dados novos.