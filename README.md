# IA Censo Escolar

Projeto de análise de dados do Censo Escolar brasileiro utilizando Python.

## Pré-requisitos

- Python 3.12 ou superior
- pip (geralmente instalado com o Python)

## Instalação

### Linux/Mac

1. Clone o repositório:
```bash
git clone <url-do-repositorio>
cd ia_censo_escolar
```

2. Crie o ambiente virtual:
```bash
python3 -m venv .venv
```

3. Ative o ambiente virtual:
```bash
source .venv/bin/activate
```

4. Instale as dependências:
```bash
pip install -r notebooks/requirements.txt
```

### Windows

1. Clone o repositório:
```cmd
git clone <url-do-repositorio>
cd ia_censo_escolar
```

2. Crie o ambiente virtual:
```cmd
python -m venv .venv
```

3. Ative o ambiente virtual:
```cmd
.venv\Scripts\activate
```

4. Instale as dependências:
```cmd
pip install -r notebooks\requirements.txt
```

## Executando os Notebooks

### Linux/Mac

1. Ative o ambiente virtual (se ainda não estiver ativo):
```bash
source .venv/bin/activate
```

2. Inicie o Jupyter Notebook:
```bash
jupyter notebook notebooks/
```

Ou, se preferir usar JupyterLab:
```bash
jupyter lab notebooks/
```

### Windows

1. Ative o ambiente virtual (se ainda não estiver ativo):
```cmd
.venv\Scripts\activate
```

2. Inicie o Jupyter Notebook:
```cmd
jupyter notebook notebooks/
```

Ou, se preferir usar JupyterLab:
```cmd
jupyter lab notebooks/
```

## Notebooks Disponíveis

- `01_visualizacao_inicial.ipynb` - Visualização inicial dos dados
- `02_visualizacao_2022.ipynb` - Análise do Censo 2022
- `03_visualizacao_2023.ipynb` - Análise do Censo 2023
- `04_visualizacao_2024.ipynb` - Análise do Censo 2024
- `05_visualizacao_totais.ipynb` - Merge de dados de 2022 a 2025

## Estrutura do Projeto

```
ia_censo_escolar/
├── data/                           # Diretório de dados
│   ├── microdados_censo_escolar_2022/
│   ├── microdados_censo_escolar_2023/
│   ├── microdados_censo_escolar_2024/
│   └── microdados_censo_escolar_2025_/
├── notebooks/                       # Notebooks de análise
│   ├── 01_visualizacao_inicial.ipynb
│   ├── 02_visualizacao_2022.ipynb
│   ├── 03_visualizacao_2023.ipynb
│   ├── 04_visualizacao_2024.ipynb
│   ├── 05_visualizacao_totais.ipynb
│   └── requirements.txt
├── .venv/                          # Ambiente virtual (criado após instalação)
└── README.md                       # Este arquivo
```

## Dependências

- pandas - Manipulação de dados
- matplotlib - Visualização de dados
- polars - Manipulação de dados de alta performance

## Desativar o Ambiente Virtual

### Linux/Mac
```bash
deactivate
```

### Windows
```cmd
deactivate
```

## Troubleshooting

### Erro "No module named 'polars'"
Certifique-se de que o ambiente virtual está ativado antes de executar os notebooks.

### Erro de permissão no Linux/Mac
Se tiver problemas de permissão ao criar o ambiente virtual, tente:
```bash
python3 -m venv --system-site-packages .venv
```

### Jupyter não reconhece o kernel
Se o Jupyter não reconhecer o kernel do ambiente virtual, instale o ipykernel:
```bash
pip install ipykernel
python -m ipykernel install --user --name=venv
```

## Licença

[Adicionar informações de licença se aplicável]
