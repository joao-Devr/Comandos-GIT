# Biblioteca de Estudo - Comandos Git

Este repositório foi criado como uma **biblioteca de estudo** para mim sobre Git. Aqui você encontrará uma compilação de **comandos básicos** de Git, úteis para iniciantes que estão aprendendo controle de versão.

---

## Todos os comandos do git:

### 1. Para iniciar novo projeto com git

```bash
git init
```

### 2. Adicionar arquivos para commit

```bash
git add
```

Adiciona os arquivos que estão prontos para serem comitados

### 3. Fazer commit

```bash
git commit -m "mensagem"
```

Commita os arquivos no histórico de alteração

### 4. Ver log de alterações

```bash
git log
```

Mostra o log de alterações da branch

### 5. Verificar status

```bash
git status
```

Mostra o estado da ramificação, se tem alterações que não foram adicionadas com o add

### 6. Ver diferenças

```bash
git diff
```

Mostra qual foi a alteração na ramificação e onde foi

### 7. Fazer merge de branches

```bash
git merge "branch alterada" "branch principal"
```

Faz a mescla das ramificações

### 8. Ver branch atual

```bash
git branch
```

Mostra a branch atual

### 9. Criar nova branch

```bash
git branch -b "nome da branch"
```

Cria uma nova branch a partir do histórico da branch

### 10. Mudar de branch

```bash
git checkout "nome da branch"
```

Muda para a branch escolhida

### 11. Adicionar repositório remoto

```bash
git remote add "nome do remote" "url do repositorio"
```

Adiciona um novo repositório remoto

### 12. Enviar alterações para repositório

```bash
git push "nome do remote" "nome da branch"
```

Manda as alterações locais para o repositório

### 13. Atualizar com alterações do repositório

```bash
git pull "nome do remote" "nome da branch"
```

Pega as alterações do repositório e atualiza a máquina

### 14. Atualizar histórico local

```bash
git fetch
```

Atualiza o histórico local de acordo com o histórico do repositório

### 15. Detalhes de um commit ou arquivo

```bash
git show
```

 Mostra detalhes de uma versão específica de um arquivo ou commit

### 16. Comparar Diferenças em Commits

```bash
git diff
```

Compara diferenças entre versões de arquivos ou entre o estado atual e o último commit

### 17. Comparar versão atual de um arquivo com a última versão confirmada

```bash
git diff report.md
```

Compara a versão atual do arquivo report.md com a última versão confirmada (commit)

### 18. Comparar versão na área de preparação com a última versão confirmada

```bash
git diff --staged
```

Compara a versão na área de preparação (staged) com a última versão confirmada

### 19. Exibir histórico de commits

```bash
git log
```

Exibe o histórico de commits, incluindo seus hashes

### 20. Referência ao commit mais recente

```bash
HEAD
```

Refere-se ao commit mais recente (atual HEAD)

### 21. Referência ao commit anterior ao HEAD

```bash
HEAD~1
```

Refere-se ao commit anterior ao HEAD (um antes do mais recente)

### 22. Comparar diferenças entre dois commits específicos

```bash
git diff <hash1> <hash2>
```

Compara as diferenças entre dois commits específicos usando seus hashes

### 23. Reverter um commit

```bash
git revert <commit>
```

Desfaz um commit criando um novo commit com as alterações revertidas(reverte todos os arquivos). Pode usar um hash de commit ou HEAD para especificar qual commit reverter

 Para nao criar um novo commit e apenas reverter as alterações usamos: 

```bash
git revert -n <commit>
```

### 24. Recuperar um arquivo de um commit específico

```bash
git checkout <commit> -- <arquivo>
```

Permite recuperar um arquivo de um commit específico, voltando o arquivo ao estado anterior. Usa o hash do commit ou HEAD, seguido do nome do arquivo

### 25. Remover arquivo da área de preparação

```bash
git restore --staged <arquivo>
```

Remove um arquivo da área de preparação (staging), voltando-o ao diretório de trabalho para edição antes de fazer um novo commit

### 26. Mover arquivos da área de preparação de volta ao repositório

```bash
git restore
```

(sem a opção --staged) Move todos os arquivos da área de preparação de volta para o repositório, desfazendo a preparação de todos os arquivos

### 27. Renomear uma branch

```bash
git branch -m "branch atual" "novo nome da branch"
```

Renomeia uma branch existente para um novo nome

### 28. Excluir uma branch

```bash
git branch -d "nome da branch"
```

Exclui uma branch após o merge (não permite exclusão se houver commits não mesclados)

### 29. Força a exclusão de uma branch

```bash
git branch -D "nome da branch"
```

Força a exclusão de uma branch, mesmo que ainda não tenha sido mesclada

