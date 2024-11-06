# Comandos terminal

Comandos mostrados durante o curso github na pratica

## clonar repositorio
    git clone url repositorio

## criar nova branch e ir para ela
    git checkout -b nome-nova-branch

## verificar branch existentes
    git branch

## analisar o status do repositorio/branch
    git status

## Preparar para o commit
    // enviar todos os arquivos criados. 
    git add .

    // enviar somente o arquivo .gitignore
    git add .gitignore

## Configurar identidade
    git config --global user.name "nome do usuario"
    git config --global user.email "email do usuario"

## Desfazer git add
    git resert caminho-do-arquivo

## Subir branch nova e arquivo
    git push -u origin nova-branch

## Voltar para branch main
    git checkout main

## deletar branch
    git branch -d nome-da-branch

## Puxar alterações do git
    git pull