

🚀 Ambiente PowerShell + Python

1. Instalação do Python
`powershell
winget install Python.Python.3.12
python --version
pip --version
`

---

2. Gerenciamento de Pacotes
`powershell
python -m pip install --upgrade pip
pip install virtualenv
`

Criar e ativar ambiente virtual:
`powershell
python -m venv .venv
.\.venv\Scripts\activate
`

---

3. Ferramentas Essenciais
`powershell
pip install jupyterlab black flake8 isort
pip install poetry
`

---

4. Configuração do PowerShell ($PROFILE)
Abra com:
`powershell
notepad $PROFILE
`

Cole:
`powershell

==============================

Configuração PowerShell para Python

==============================

Oh My Posh
oh-my-posh init pwsh --config "$env:POSHTHEMESPATH\paradox.omp.json" | Invoke-Expression

Autocomplete inteligente
Import-Module PSReadLine
Set-PSReadLineOption -PredictionSource History
Set-PSReadLineOption -PredictionViewStyle ListView

Ícones no terminal
Import-Module Terminal-Icons

==============================

Aliases úteis

==============================
Set-Alias py python
Set-Alias pipup "python -m pip install --upgrade pip"
Set-Alias venv "python -m venv .venv"

==============================

Funções personalizadas

==============================
function act { .\.venv\Scripts\activate }
function jlab { jupyter lab }
function runpy { param($file) python $file }
`

---

5. Integração com Windows Terminal
- Configure perfis separados:
  - PowerShell (Python)
  - WSL2 (Ubuntu/Fedora) para rodar Python em Linux
- Use Nerd Fonts para ícones bonitos.
- Ative GPU Text Rendering e transparência.

---

🎨 Resultado
- Prompt estilizado com Oh My Posh  
- Autocomplete inteligente  
- Aliases rápidos para Python (py, venv, act, jlab)  
- Ambientes isolados com venv ou poetry  
- Perfis no Windows Terminal para alternar entre PowerShell e WSL2  
`

---

👉 Esse arquivo .me (ou .md) pode ser usado como guia de setup no seu repositório ou documentação pessoal.  

Quer que eu prepare também um exemplo de settings.json do Windows Terminal já com perfil Python configurado?