## Notas de Aula - Módulo 02

### Curso Git e GitHub do projeto Potência Feminina

---
### Conceitos Básicos

- **main/master:** Representa a linha principal de desenvolvimento em um repositório Git. É a ramificação padrão para o código estável e pronto para produção.
- **origin:** Refere-se ao repositório remoto de onde o clone foi criado. É o ponto de referência padrão para interações com o repositório remoto.
- **head:** Aponta para o commit atual em que você está trabalhando. Pode referenciar uma branch específica, indicando onde novos commits serão adicionados.
- **branch:** É uma linha de desenvolvimento independente que permite trabalhar em funcionalidades ou correções sem interferir diretamente na linha principal. Facilita a colaboração e o gerenciamento de alterações.
- **commit:** Um commit adiciona as alterações mais recentes do código-fonte para o repositório, tornando essas alterações parte da revisão principal do repositório.
- **merge:** É o processo de combinar as alterações de uma branch com outra, resultando em um novo commit que integra as modificações das duas linhas de desenvolvimento.
- **rebase:** É a ação de pegar uma sequência de commits, "pegá-los" e aplicá-los como se tivessem sido feitos em outro ponto. Ajuda a manter um histórico de commit mais linear e limpo, mas deve ser usado com cuidado para evitar problemas de colaboração.

---
### Inicie um projeto
Cria um repositório Git vazio ou reinicializa um já existente.

```git init [diretório]```

Clona um repositório em um novo diretório.

```git clone [url]```

---
### Faça uma mudança
Adiciona o arquivo ao staging area para ser incluído no próximo commit.

```git add [nome do arquivo]```

Adiciona todas as mudanças no diretório de trabalho ao staging area para serem incluídas no próximo commit.

```git add .```

Realiza um commit, adicionando as mudanças previamente preparadas no staging area.

```git commit -m "[texto do commit]"```

Adiciona automaticamente todas as mudanças no diretório de trabalho ao staging area e realiza um commit.

```git commit -am "[texto do commit]"```

---
### Confira seu repositório
Exibe o estado atual do repositório, mostrando arquivos modificados, adicionados ou removidos.

```git status```


Mostra as diferenças entre as mudanças no diretório de trabalho e o último commit.

```git diff```


Apresenta o histórico de commits do repositório, incluindo detalhes como autor, data e mensagem de commit.

```git log```


Fornece um histórico de commits simplificado, exibindo cada commit em uma única linha com a mensagem resumida.

```git log --oneline```

Exibe informações detalhadas sobre o último commit.

```git show```

Exibe informações detalhadas sobre o commit especificado.

```git show [commit]``` 

---
#### Branches e Merging

Lista as branches existentes no repositório, indicando a atual com um asterisco.

```git branch```

Cria uma nova branch

```git branch [nome da branch que será criada]```

Muda para a branch especificada.

```git checkout [nome da branch]```

Cria e muda para uma nova branch especificada.

```git checkout -b [nome da branch que será criada]```

Deleta a branch especificada.

```git branch -d [nome da branch]```

Combina as alterações da branch especificada à branch atual.

```git merge [nome da branch]```

Reescreve o histórico de commits movendo a branch atual para o topo da branch especificada.

```git rebase [nome da branch]```

---
### Sincronize

Adiciona um novo repositório remoto com a URL fornecida.

```git remote add [url]```

Busca as alterações do repositório remoto, atualizando as referências locais sem mesclar automaticamente.

```git fetch``` 

Obtém as mudanças do repositório remoto e mescla automaticamente com a branch local atual.

```git pull``` 

Envia as alterações locais para o repositório remoto associado, atualizando-o com os commits locais.

```git push```

---
### Desfaça mudanças

Desfaz as alterações no arquivo especificado, mantendo as mudanças no stage.

```git reset [nome do arquivo]``` 

Desfaz todas as alterações no working directory e no stage, retornando ao estado do commit especificado.

```git reset --hard``` 

Cria um novo commit que desfaz as mudanças introduzidas pelo commit especificado.

```git revert [commit]``` 

---
#### E por último!

Em caso de dúvida, use o git help, ele mostra informações de ajuda para o comando git especificado.

```git [comando] --help```