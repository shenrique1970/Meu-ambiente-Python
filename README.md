# 🐍 Ambiente Python3 com mise no Zorin OS

## 1. Instalar Python via mise
```bash
mise install python@3.12

mise use -g python@3.12

mise local python@3.12
```
obs: Isso cria um arquivo .mise.toml na pasta do projeto.

## 2. Criar ambiente virtual
```
python -m venv .venv
source .venv/bin/activate
```

## 3. Atualizar pip e instalar pacotes essenciais
```
pip install --upgrade pip
pip install jupyterlab black flake8 isort poetry

```
## 4. Configuração do projeto com mise
Crie um arquivo .mise.toml na raiz do projeto:

```
[tools]
python = "3.12"
```
obs: Assim, sempre que entrar na pasta, o mise ativa automaticamente o Python 3.12.



