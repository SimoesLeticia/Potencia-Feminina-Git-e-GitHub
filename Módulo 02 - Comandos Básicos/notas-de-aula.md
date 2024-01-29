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
<table border=\"1\">
<tr><td>Cria um repositório Git vazio ou reinicializa um já existente.

**`git init [diretório]`**</td></tr>

<tr><td>Clona um repositório em um novo diretório.
	
**`git clone [url]`**</td></tr>
</table>

### Faça uma mudança
<table border=\"1\">
<tr><td>Adiciona o arquivo ao staging area para ser incluído no próximo commit.

**`git add [nome do arquivo]`**</td></tr>

<tr><td>Adiciona todas as mudanças no diretório de trabalho ao staging area para serem incluídas no próximo commit.

**`git add .`**</td></tr>

<tr><td>Realiza um commit, adicionando as mudanças previamente preparadas no staging area.

**`git commit -m "[texto do commit]"`**</td></tr>

<tr><td>Adiciona automaticamente todas as mudanças no diretório de trabalho ao staging area e realiza um commit.

**`git commit -am "[texto do commit]"`**</td></tr>
</table>

### Confira seu repositório
<table border=\"1\">
<tr><td>Exibe o estado atual do repositório, mostrando arquivos modificados, adicionados ou removidos.

**`git status`**</td></tr>

<tr><td>Mostra as diferenças entre as mudanças no diretório de trabalho e o último commit.

**`git diff`**</td></tr>

<tr><td>Apresenta o histórico de commits do repositório, incluindo detalhes como autor, data e mensagem de commit.

**`git log`**</td></tr>

<tr><td>Fornece um histórico de commits simplificado, exibindo cada commit em uma única linha com a mensagem resumida.

**`git log --oneline`**</td></tr>

<tr><td>Exibe informações detalhadas sobre o último commit.

**`git show`**</td></tr>

<tr><td>Exibe informações detalhadas sobre o commit especificado.

**`git show [commit]`**</td></tr>
</table>

### Branches e Merging
<table border=\"1\">
<tr><td>Lista as branches existentes no repositório, indicando a atual com um asterisco.

**`git branch`**</td></tr>

<tr><td>Cria uma nova branch

**`git branch [nome da branch que será criada]`**</td></tr>

<tr><td>Muda para a branch especificada.

**`git checkout [nome da branch]`**</td></tr>

<tr><td>Cria e muda para uma nova branch especificada.

**`git checkout -b [nome da branch que será criada]`**</td></tr>

<tr><td>Deleta a branch especificada.

**`git branch -d [nome da branch]`**</td></tr>

<tr><td>Combina as alterações da branch especificada à branch atual.

**`git merge [nome da branch]`**</td></tr>

<tr><td>Reescreve o histórico de commits movendo a branch atual para o topo da branch especificada.

**`git rebase [nome da branch]`**</td></tr>
</table>

### Sincronize
<table border=\"1\">
<tr><td>Adiciona um novo repositório remoto com a URL fornecida.

**`git remote add [url]`**</td></tr>

<tr><td>Busca as alterações do repositório remoto, atualizando as referências locais sem mesclar automaticamente.

**`git fetch`**</td></tr>

<tr><td>Obtém as mudanças do repositório remoto e mescla automaticamente com a branch local atual.

**`git pull`**</td></tr>

<tr><td>Envia as alterações locais para o repositório remoto associado, atualizando-o com os commits locais.

**`git push`**</td></tr>
</table>

### Desfaça mudanças
<table border=\"1\">
<tr><td>Desfaz as alterações no arquivo especificado, mantendo as mudanças no stage.

**`git reset [nome do arquivo]`**</td></tr>

<tr><td>Desfaz todas as alterações no working directory e no stage, retornando ao estado do commit especificado.

**`git reset --hard`**</td></tr> 

<tr><td>Cria um novo commit que desfaz as mudanças introduzidas pelo commit especificado.

**`git revert [commit]`**</td></tr>
</table>

### E por último!
<table border=\"1\">
<tr><td>Em caso de dúvida, use o git help, ele mostra informações de ajuda para o comando git especificado.

**`git [comando] --help`**</td></tr>
</table>