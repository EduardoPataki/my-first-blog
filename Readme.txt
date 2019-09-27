>>>>>>>>>> Inicie o seu ambiente virtual executando:<<<<<<<<<<<<<

command-line

$ source myvenv/bin/activate

$ deactivate

>>>>>>>>>>>>>>>>> Criando o projeto Django <<<<<<<<<<<<<<<<

$ django-admin startproject mysite .

>>>>>>>>>>>> Criando tabelas para nossos modelos no banco de dados <<<<<<<<<<<

O último passo é adicionar nosso novo modelo ao banco de dados. Primeiramente,
precisamos fazer com que o Django entenda que fizemos algumas alterações nos
nossos modelos. (Acabamos de criar um modelo de Post!) Vá para o console e
digite python manage.py makemigrations blog. Deve ficar assim:

command-line

(myvenv) ~/djangoblog $ python manage.py makemigrations blog

Observação: Lembre-se de salvar os arquivos que você editar. Caso contrário,
o computador executará uma versão antiga que pode gerar mensagens de erro
inesperadas.

O Django preparou um arquivo de migração que precisamos aplicar ao nosso
banco de dados. Digite python manage.py migrate blog e a saída deve ser:

command-line

(myvenv) ~/djangoblog $ python manage.py migrate blog

>>>>> Executar <<<<<<<<<

$ python manage.py runserver

no console para iniciar o servidor web. Vá para o seu navegador e digite
o endereço http://127.0.0.1:8000/admin/.
Você verá uma página de login

