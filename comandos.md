# Prática de git

## Comandos básicos

### Configuração inicial


```
git config --global user.name "COLOQUE O NOME"
```

```
git config --global user.email "COLOQUE O EMAIL"
```

### Inicializando um repositório

O comando git init serve para inicializar um repositório git em um diretório.

Ele cria um diretório oculto chamado .git, que contém todos os arquivos necessários para o funcionamento do repositório.
```
git init
```

### Verificando o status do repositório

O comando git status serve para verificar o status do repositório.

Ele mostra quais arquivos foram modificados, quais arquivos foram adicionados e quais arquivos foram removidos.

```
git status
```

### Adicionando arquivos para o commit

O comando git add serve para adicionar arquivos para o commit.

Ele adiciona os arquivos para o commit, mas não cria o commit.

Dessa forma adiciona um ou mais arquivos para o commit.

```

git add NOME_DO_ARQUIVO
```

```

git add .
```
Usar um ponto no lugar do nome do arquivo adiciona todos os arquivos modificados para o commit.

```
git add --all
```
Usar --all adiciona todos os arquivos modificados e todos os arquivos criados para o commit.

```
git add . -A
```
Usar -A adiciona todos os arquivos modificados e todos os arquivos criados para o commit.

### Criando um commit

O comando git commit serve para criar um commit.

Ele cria um commit com os arquivos adicionados com o comando git add.

```
git commit -m "MENSAGEM DO COMMIT"
```
Usar -m "MENSAGEM DO COMMIT" adiciona uma mensagem ao commit.

Exemplos:

```
git commit -m "Adicionando o arquivo index.html"

```
Exemplo usando tags para o comit:
```
git commit -m "docs: Adicionando o arquivo index.html"
```

### Visualizando os commits

O comando git log serve para visualizar os commits.

Ele mostra os commits que foram criados no repositório.

```
git log
```

### Visualizando as diferenças

O comando git diff serve para visualizar as diferenças entre os commits.

Ele mostra as diferenças entre os commits.

```
git diff
```

### Branch

O comando git branch serve para criar uma branch.

Ele cria uma branch, que é uma ramificação do repositório.

```
git branch NOME_DA_BRANCH
```

Usando o operador -b 

```
git branch -b NOME_DA_BRANCH
```
O -b serve para criar a branch e já mudar para ela.

### Mudando de branch

O comando git checkout serve para mudar de branch.

Ele muda de branch.

```
git checkout NOME_DA_BRANCH
```

### Merge

O comando git merge serve para juntar duas branchs.

Ele junta duas branchs.

```
git merge NOME_DA_BRANCH
```
Exemplo:

Suponha que tenhamos uma branch chamada de teste e queiramos juntar ela com a branch master

```
git checkout master

git merge teste
```

    
