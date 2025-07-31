# Meu-ambiente-Python
Área de desenvolvimento python.

## Gerenciando tudo com o uv

[uv](https://docs.astral.sh/uv/getting-started/) é uma ferramenta que promete bastante. Sua intenção é substituir praticamente todas as outras ferramentas: pip, pip-tools, pipx, poetry, pyenv, twine, virtualenv, e outras... Até agora tem cumprido tudo com perfeição. Além disso, é uma ferramenta extremamente rápida, escrita em Rust.

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

