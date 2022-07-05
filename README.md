# django-project-docs

<h1 align="center">
Criação de  projeto django
</h1>

# 👾 Introdução

O primeiro passo é criar a pasta do projeto:

- No terminal utilize o comando `` mkdir <NomeDaPasta> `` para criar a pasta e o comando ``cd <NomeDaPasta>`` para entrar dentro dela.

O segundo passo é criar um ambiente virtual python:

- No terminal utilize o comando ``python3 -m venv <NomeDoAmbienteVirtual>`` para criar um ambiente virtual.
- Para ativar o ambiente virtual utilize o comando ``source <NomeDoAmbienteVirtual>/bin/activate``  no Linux e macOS | no Windows utilize o comando source ``<NomeDoAmbienteVirtual>/Scripts/activate``

Depois de criar o ambiente virtual é necessário baixar o Django e o DjangoRestFramework:

- Para isso digite em seu terminal ``pip install django djangorestframework``

----

## 👾 Criando o primeiro app

O primeiro passo é escrever no terminal o seguinte comando: 
- ``python3 manage.py startapp <nomeDoApp>``

É bom já criarmos também a estrutura inicial do banco de dados:
- ``python3 manage.py migrate``

Para saber se deu certo, é necessário apenas rodar o servidor:
- ``python3 manage.py runserver`` e acessar http://localhost:8000 no seu browser.
- Se tudo der certo uma tela escrito "The install worked successfully! Congratulations" aparecerá ao entrar na página.

Agora precisamos criar um super usuário com o seguinte comando:
- ``python3 manage.py createsuperuser``

Depois é preciso adicionar tudo ao ``settings.py``
- Primeiro, abra o arquivo ``settings.py`` que fica na raiz do projeto.
- Depois em ``INSTALLED_APPS`` adicione o app criado e ``rest_framework`` dentro do array.

Essa é a estrutura inicial do projeto.

----

# 👾 Modelagem
