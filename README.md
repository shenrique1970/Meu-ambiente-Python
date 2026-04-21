📌 1. Instalar o Python com mise
No terminal:

bash
mise install python@3.12
Isso baixa e instala o Python 3.12 dentro do ambiente controlado pelo mise.

Se quiser usar essa versão globalmente:

bash
mise use -g python@3.12
Ou apenas dentro de um projeto:

bash
mise local python@3.12
Isso cria um arquivo .mise.toml na pasta do projeto, fixando a versão.

📌 2. Criar ambiente virtual
Com o Python instalado via mise, você pode criar um ambiente virtual:

bash
python -m venv .venv
source .venv/bin/activate
No Zorin OS (que usa bash/zsh por padrão), o comando source ativa o ambiente.

📌 3. Instalar pacotes essenciais
Dentro do ambiente virtual:

bash
pip install --upgrade pip
pip install jupyterlab black flake8 isort poetry
📌 4. Configurar mise para sempre usar Python
Se quiser que o mise sempre carregue o Python certo, edite o arquivo .mise.toml do projeto:

toml
[tools]
python = "3.12"
