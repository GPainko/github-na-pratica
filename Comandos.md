# Comandos do Terminal

Comandos mostrados durante o curso **GitHub na prática**.

## Clonar repositório
Clona um repositório existente na máquina local.
```bash
git clone <url-do-repositorio>
```

## Criar nova branch e ir para ela
Cria uma nova branch e muda para ela automaticamente.
```bash
git checkout -b <nome-nova-branch>
```

## Verificar branches existentes
Lista as branches locais do repositório.
```bash
git branch
```

## Analisar o status do repositório/branch
Mostra o status dos arquivos modificados, criados ou em staging.
```bash
git status
```

## Preparar arquivos para o commit
### Enviar todos os arquivos modificados e criados:
```bash
git add .
```

### Enviar somente um arquivo específico:
```bash
git add <nome-do-arquivo>
```

Exemplo para o `.gitignore`:
```bash
git add .gitignore
```

## Configurar identidade do Git
Define o nome e o e-mail do usuário globalmente.
```bash
git config --global user.name "nome-do-usuario"
git config --global user.email "email-do-usuario"
```

## Desfazer um `git add`
Remove arquivos da área de staging sem perder as modificações.
```bash
git reset <caminho-do-arquivo>
```

Para desfazer **todos** os arquivos adicionados:
```bash
git reset
```

## Commitar alterações
Grava as alterações no histórico local do repositório.
```bash
git commit -m "Mensagem descritiva do commit"
```

## Subir branch e commits para o repositório remoto
Sobe a nova branch e os commits associados.
```bash
git push -u origin <nome-da-branch>
```

### Atualizar commits em uma branch já existente:
```bash
git push
```

## Voltar para a branch `main`
Muda para a branch principal (main ou master).
```bash
git checkout main
```

## Deletar branch
### Deletar uma branch local:
```bash
git branch -d <nome-da-branch>
```

### Deletar uma branch no repositório remoto:
```bash
git push origin --delete <nome-da-branch>
```

## Puxar alterações do repositório remoto
Atualiza o repositório local com as alterações do repositório remoto.
```bash
git pull
```

## Ver histórico de commits
Exibe o histórico de commits com detalhes.
```bash
git log
```

## Desfazer commits
### Voltar ao último commit, mantendo alterações locais:
```bash
git reset --soft HEAD~1
```

### Descartar completamente o último commit:
```bash
git reset --hard HEAD~1
```

## Exibir diferenças entre arquivos
### Mostrar diferenças entre arquivos no diretório:
```bash
git diff
```

### Comparar com um commit específico:
```bash
git diff <commit-hash>
```
