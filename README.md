# Meu-ambiente-Python
Área de desenvolvimento python.

### Python e UV.
[UV](https://docs.astral.sh/uv/getting-started/installation/)

- Resumo:
### Cria o projeto completo
```sh uv init nome-do-projeto ```

### Ou inicializa dentro de um projeto existente:
```sh uv init ```

### Instala Python, cria venv e instala dependências em 1 comando
```sh uv sync ```

### Instala pacotes
```sh uv add requests ruff pyright ```

### Remove pacotes
```sh uv remove requests ```

### Requerimentos via requirements.txt
```sh uv add -r requirements.txt ```

### Executa scripts Python sem ativar venv
```sh uv run src/main.py ```

### Instala ferramentas como ruff ou pyright globalmente
```sh uv tool install ruff ```
```sh uvx ruff ```
```sh uv tool uninstall ruff ```

### Outros comandos
```sh uv python list ```

```sh uv python list ```

```sh uv python install 3.12.10 ```

```sh uv python pin 3.12.10 ```
