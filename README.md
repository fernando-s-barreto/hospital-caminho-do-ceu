HospitalTech – Guia de Instalação
1. Clonar o Repositório
git clone https://github.com/fernando-s-barreto/hospital-caminho-do-ceu.git


Acesse a pasta do projeto:

cd HospitalTech

2. Criar e Ativar o Ambiente Virtual

Criar ambiente virtual:

python -m venv venv


Ativar no PowerShell:

venv\Scripts\Activate.ps1


Ativar no CMD:

venv\Scripts\activate.bat


Se ocorrer erro de permissão no PowerShell:

Set-ExecutionPolicy RemoteSigned -Scope CurrentUser

3. Instalar Dependências
pip install -r requirements.txt

4. Migrar o Banco de Dados
python manage.py migrate

5. Carregar Usuário Padrão
python manage.py loaddata admin_default.json


Login padrão:

Login: admin

Senha: admin123

6. Iniciar o Servidor
python manage.py runserver


Acesse no navegador:

http://127.0.0.1:8000/

Observações Importantes

Não envie a pasta venv para o GitHub.

Caso o pip install -r requirements.txt apresente erro:

Apague a pasta venv

Crie novamente:

python -m venv venv


Ative e rode:

pip install --upgrade pip
pip install -r requirements.txt
