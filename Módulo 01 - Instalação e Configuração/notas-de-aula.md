## Notas de Aula - Módulo 01

### Curso Git e GitHub do projeto Potência Feminina

#### Instalação
Instale o Git no Windows seguindo estes passos:

1. Baixe o instalador do Git para Windows no site oficial: https://git-scm.com/download/win
2. Execute o arquivo baixado para iniciar o instalador.
3. Siga as instruções do instalador, aceitando as configurações padrão.
4. Durante a instalação, será solicitado que escolha o editor de texto padrão para o Git. Você pode optar por usar o editor padrão sugerido ou escolher outro de sua preferência.
5. Quando a instalação estiver concluída, abra o "Git Bash", um terminal que permite interagir com o Git.

#### Configuração

1. Defina seu nome de usuário e endereço de e-mail no Git com os seguintes comandos:
    ```
    git config --global user.name "[Nome de usuário]"
    git config --global user.email [e-mail]
    ```
2. Para visualizar todas as configurações e assegurar que o Git foi configurado corretamente, utilize o comando:
    ```
    git config --list
    ```
3. Ao executar esse comando, será exibida uma lista de pares chave-valor representando as configurações globais do Git. Observe especialmente os campos ```user.name``` e ```user.email```. Caso não estejam configurados corretamente, repita o passo anterior para corrigir.