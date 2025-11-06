**1. Clonar o Repositório**

&nbsp;	git clone https://github.com/fernando-s-barreto/hospital-caminho-do-ceu.git



**Em seguida, navegue para o diretório do projeto:**

&nbsp;	cd Hospital-Caminho-do-Ceu



**2. Criar e Ativar o Ambiente Virtual**

&nbsp;	python -m venv venv



**Comando para Ativar**

&nbsp;	Windows (PowerShell)	venv\\Scripts\\activate.bat

&nbsp;	Windows (CMD)	venv\\Scripts\\activate.bat



**3. Instalar as Dependências**

&nbsp;	pip install -r requirements.txt



**4. Configurar e Migrar o Banco de Dados**

&nbsp;	python manage.py migrate



**5. Criar um Superusuário (Opcional, mas Recomendado)**

&nbsp;	python manage.py createsuperuser



**6. Rodar o Servidor**

&nbsp;	python manage.py runserver





**SE DER ERRO NA TORA DE VENV VENV** 

Set-ExecutionPolicy RemoteSigned -Scope CurrentUser


Rodar a Venv
venv\\Scripts\\Activate.ps1

**Se não conseguir pip install -r requirements.txt **

Apague a pasta venv:

Remove-Item -Recurse -Force .\venv


Crie novamente o ambiente virtual:

python -m venv venv


Ative:

.\venv\Scripts\Activate.ps1


Atualize o pip:

python -m pip install --upgrade pip


(Opcional) Reinstale os pacotes necessários:

pip install -r requirements.txt


Agora rode:

pip freeze > requirements.txt

# Não suba a VENV no hub

