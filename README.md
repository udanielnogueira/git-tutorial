# git-tutorial

Sincronizando e fazendo push de arquivos locais para a nuvem.

## Configuração

Se for a primeira vez usando o git no terminal:

~~~powershell
git config --global user.email "you@example.com"
git config --global user.name "your name"
~~~

## Repositório já publicado no GitHub (Web ou Desktop)

1. Entrar na pasta local do Github

~~~powershell
cd caminhoGitHub
~~~

2. Clonar repositório

~~~powershell
git clone https://github.com/username/repositorio
~~~

3. Verificar status

~~~powershell
git status
~~~

4. Preparar arquivo

~~~powershell
git add . 
~~~

ou

~~~powershell
git add file.extension
~~~

5. Fazer commit

~~~powershell
commit -m "Update file"
~~~

6. Fazer push

~~~powershell
git push
~~~

## Repositório ainda não criado

1. Entrar na pasta GitHub 

~~~powershell
cd caminhoGitHub
~~~

2. Criar pasta do repositório

~~~powershell 
mkdir repositorio
~~~

3. Acessar pasta do repositório na IDE

4. Configurar repositorio 

~~~powershell
git init
~~~

5. Criar README.md dentro da pasta do repositório

~~~powershell
git add README.md
~~~

6. Verificar status

~~~powershell
git status
~~~

7. Fazer commit

~~~powershell
git commit -m "Create file"
~~~

8. Adicionar endereço remoto

~~~powershell
git remote add origin https://github.com/username/repositorio.git
~~~

9. Criar repositório vazio no GitHub (Web ou Desktop) 

Atenção: use o mesmo nome do repositório criado localmente.

10. Fazer push

~~~
git push -u origin main 
~~~

Quando feito a primeira vez, após isso ``git push`` somente.

**Em caso de Fatal Error no HTTP, resete a url dessa forma:**

~~~powershell
git remote set-url origin https://github.com/udanielnogueira/PastaDoProjeto.git`
~~~

## Próximos passos

Após a sincronização com a nuvem, basta executar os comandos de adição, commit e push.

~~~powershell
git add .

git commit -m "Update file"

git push
~~~

## Extra

Criando branch main e mudando para a main:

~~~powershell
git branch teste
git checkout teste
~~~

Caso for criar um pull request, criar uma branch com seu nome antes.
