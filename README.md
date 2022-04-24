# sistema-django-intermediario
- Sistema simples Web com Django, utilizando banco de dados Postgres. 

- Criado com base em conhecimentos adquiridos no curso Programação Web com Python e Django Framework: Essencial, na plataforma Udemy:

https://www.udemy.com/course/programacao-web-com-django-framework-do-basico-ao-avancado/

## Deploy

O sistema atualmente está disponível no heroku:

https://sistema-produtos-intermediario.herokuapp.com/


## Dependências

- django = 4.0.4
- gunicorn = 20.1.0
- whitenoise = 6.0.0
- django-bootstrap4 = 22.0
- django-stdimage = 5.3.0
- psycopg2-binary = 2.9.3


## Instalação

1. clonar o repositório em algum diretório escolhido:
```bash
git clone https://github.com/maldonadopereira/sistema-django-intermediario.git
```

2. Criar uma venv, no exemplo a seguir será utilizado o pipenv:
```bash
pipenv shell
```

3. Instalar as dependências:
```bash 
pipenv sync 
```

4. Sincronize a base de dados:

```bash
python manage.py migrate
```

5. Crie um usuário (Administrador do sistema):

```bash
python manage.py createsuperuser
```

6. Teste a instalação carregando o servidor de desenvolvimento (http://localhost:8000 no navegador):

```bash
python manage.py runserver
```

## Implementações

- Cadastro de produtos;
- Configuração completa para envio de E-mail pelo sistema.