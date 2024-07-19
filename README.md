# git-tutorial

Primeiros passos usando o Git.

## Versão

~~~powershell
git -v
~~~

## Configuração

~~~powershell
git config --global user.email "you@example.com"
git config --global user.name "your name"
~~~

## Exemplo de jornada com repositório já criado no GitHub

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

## Exemplo de jornada com repositório ainda não criado no GitHub

1. Entrar na pasta local do GitHub 

~~~powershell
cd caminhoGitHub
~~~

2. Criar pasta do repositório

~~~powershell 
mkdir repositorio
~~~

3. Entrar na pasta do repositório

~~~powershell
cd nomeRepositorio
~~~

4. Configurar repositório 

~~~powershell
git init
~~~

5. Verificar status

~~~powershell
git status
~~~

6. Criar README.md via prompt

~~~powershell
echo "# My README" > README.md
~~~

7. Verificar status

~~~powershell
git status
~~~

8. Adicionar o arquivo ao Git

~~~powershell
git add README.md
~~~

9. Verificar status

~~~powershell
git status
~~~

10. Fazer commit

~~~powershell
git commit -m "Create file"
~~~

11. Verificar log

~~~powershell
git log
~~~

12. Verificar status

~~~powershell
git status
~~~

13. Adicionar endereço remoto

~~~powershell
git remote add origin https://github.com/username/repositorio.git
~~~

14. Criar repositório remoto vazio no GitHub 

Use o mesmo nome do repositório criado localmente.

15. Fazer push

~~~
git push -u origin main 
~~~

Esse push mais completo é ideal para quando for feito pela primeira vez, após isso ``git push`` somente. E em caso de Fatal Error no HTTP, resete a url dessa forma:

~~~powershell
git remote set-url origin https://github.com/udanielnogueira/PastaDoProjeto.git
~~~

## Próximos passos

Após a sincronização com a nuvem, basta executar os comandos de adição, commit e push. E caso for criar um pull request, criar uma branch com seu nome antes.

~~~powershell
git add .

git commit -m "Update file"

git push
~~~

## Outros comandos

Criar nova branch

~~~~powershell
git branc novaBranch
~~~~

Mudar para outra branch

~~~~powershell
git checkout outraBranch
~~~~

Apagar mudanças e voltar ao estado anterior

~~~~powershell
git reset --hard
~~~~

Acessar help de um comando

~~~~powershell
git comando --help

# Exemplo
git merge --help
~~~~

Ver mudanças feitas em um commit específico

~~~powershell
git show hashNumber
~~~

Fazer merge de uma novaBranh com a branch main

~~~~powershell
git checkout main
git merge novaBranch
~~~~
