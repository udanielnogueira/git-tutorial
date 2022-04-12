# GitTutorial

Ao instalar o Git, escolher as opções main.

## Repositório e arquivo do zero

1. Entrar em Desktop: 

`cd desktop`

2. Criar uma pasta que será o repositório: 

`mkdir projeto`

3. Entrar nessa pasta repositório e instalar o git: 

`git init`

4. Confira o arquivo .git na pasta: 

`ls -h`

5. Usar uma IDE e criar um código na pasta

6. Verificar o status atual: 

`git status`

(Ele vai dizer que você está no branch Master, que precisa rastrear o arquivo e que não há um commit.)

7. Rastrear o arquivo:

`git add .\example.py`

8. Depois disso, posso fazer o commit: 

`git commit -m "Create file"`

("Create file" ou outra mensagem pra dizer o que você estava fazendo no momento do commit.)

9. Se for a primeira vez no commit:

```
git config --global user.email "you@example.com"
git config --global user.name "your name"
```

10. Eviar o commit ao repositório remoto:

`git remote add origin https://github.com/udanielnogueira/Python101.git`

11. Dar o push:

`git push -u origin master`

(Origin é o local para onde eu estou mandando.)

12. Criando branch main e mudando para a main:

```
git branch main
git checkout main
```

(Caso for criar um pull request, criar uma branch com seu nome antes.)

## Repositório já criado no GitHub Desktop

1. Entre na pasta (do repositório)

2. `git pull`

3. `git status`

4. `git add . OU git add file.py`

5. `git commit -m "Update file"`

6. `git push`

## Linha de criação alternativa

1. Entrar na pasta GitHub com cd

2. `mkdir PastaDoProjeto`

3. Abrir a pasta no VS Code

4. Criar um README.md no VS Code

5. `git add README.md`

6. `git commit -m "Create files"`

7. `git remote add origin http://github.com/udanielnogueira/PastaDoProjeto.git`

8. Criar esse repositório vazio no GitHub (Web ou Desktop) 

9. `git push -u origin main` (Quando feito uma vez, `git push` somente)

Em caso de Fatal Error no HTTP, resete a url dessa forma:

`git remote set-url origin https://github.com/udanielnogueira/PastaDoProjeto.git`
