# AULACIA PROGRAMAÇÃO
## AULA 07/10/21 - Conceitos iniciais Git
- COMANDOS GIT:
  - add
    - Adiciona um arquivo
    ``` 
    git add exemplo/arquivo.js
    ```
    - Adiciona todos os arquivos da pasta
    ```
    git add .
    ```
    Após adicionar os arquivos criados, faz o "git commit" para lançar os arquivos para o repositório local.

  
  - commit (Salva na arvore local)
    
    - Adiciona as modificações para a arvore local
    ```
    git commit -m "descrição do que foi feito"
    ```

  - push
    
    - Manda as alterações da arvore local para a arvore remota (servidor), vem após o commit
    ```
    git push
    git push <origin> <master> (empurra as alterações do local para uma brench específica)
    ```
    
  
  - fetch 
    - Não muda nada, apenas atualiza as informações do repositório local local com o remoto (é o fofoqueiro)
    ```
    git fetch
    ```
  
  - checkout
    - Troca de brench ( a ramificação) 
  ```
  git checkout <nome_da_branch>
  git checkout [nome_da_branch]
  git checkout -b <novo_nome_da_brench> (cria a branch caso ela nao exista)
  ```

  - branch
    
    - mostra o nome das branchs (ramificações)
  ```
  git branch (mostra as branchs locais)
  git branch -a (mostra todas as branchs)
  ```


## AULA 2 - BASICO DO VSCODE

- 