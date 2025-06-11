# Meu-ambiente-Python
Área de desenvolvimento python.

### Python e UV - Um pacote Python extremamente rápido e gerenciador de projetos, escrito em Rust...
[UV](https://docs.astral.sh/uv/getting-started/installation/)

- Resumo:
### Cria o projeto completo
```uv init nome-do-projeto ```

### Ou inicializa dentro de um projeto existente:
```uv init ```

### Instala Python, cria venv e instala dependências em 1 comando
```uv sync ```

### Instala pacotes
```uv add requests ruff pyright ```

### Remove pacotes
```uv remove requests ```

### Requerimentos via requirements.txt
```uv add -r requirements.txt ```

### Executa scripts Python sem ativar venv
```uv run src/main.py ```

### Instala ferramentas como ruff ou pyright globalmente
```uv tool install ruff ```

```uvx ruff ```

```uv tool uninstall ruff ```

### Outros comandos
```uv python list ```

```uv python list ```

```uv python install 3.12.10 ```

```uv python pin 3.12.10 ```
