# Comandos GIT / GITHUB

## cria uma chave nova para git

- ssh-keygen -t ed25519 -C email

entrar na pasta que foi criado a chave e mostra a chave
- cat id_ed25519.pub

copia a chave para o github
inicia um projeto github
- eval $(ssh-agent -s)

adiciona a chave 
- ssh-add id_ed25519


## **git hub**


Clona um repositório
- git clone [chave ssh do repositório]

Cria um repositório na pasta que está aberto
- git init

Setar configurações do git
- git config --global user.[campo] "[email]" 

Excluir propriedade
- git config --global --unset user.[campo]

Vincula nosso repositório git com git hub
- git remote add [nome: origin] [link do repositório]

Lista repositorios do git
- git remote -v

Empurra repositório para github
- git push [nome repositorio: orirgin] master

Puchar repositório online para o local
- git pull [nome repositprio: origin] master


Adicionar todos arquivos da pasta a lista
- git add *

comitar (salvar no git)
- git commit -m "mensagem qualquer"

verificar status
- git status


## Extras

Gera o sha1 de um arquivo
- openssl sha1 texto.txt