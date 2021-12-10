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

- Declarações de Variáveis (const, let, var)
  - Tipos
    - String
      - Conjunto de caracteres que sempre estarão entre aspas
  ```javascript
  const frase = "Brasília, capital do Brasil"
  ```
    - Number 
      - Qualquer valor numérico 
  ```
  123,456
  ``` 
    - Boolean
      - É um tipo de dado que só pode ser dois valores 1 ou 0, verdadeiro ou falso.
  ```
  1>0 true
  1<0 false
  ``` 
    - Null
      - Nulo é um valor vazio, ou seja, é uma variável que existe com o valor vazio.
  ```javascript
  let exempleNull = [ahsudhasd]
  exempleNull = null
  ```  
    - Undefined
      - É uma variável que o código não reconhece, ou seja, não foi declarada no código 
  ```javascript
  
  ``` 
    - Object
      - É uma entidade independente, com propriedades e tipos. Compare-o com uma xícara, por exemplo. Uma xícara é um objeto, com propriedades. Uma xícara tem uma cor, uma forma, peso, um material de composição, etc. Da mesma forma, objetos em JavaScript podem ter propriedades, que definem suas características. 
      - Usa-se chave
      - DECLARAÇÃO
       ```javascript
       const caneco = {name: "canecacio", size: "500"}
       ```
      - CHAMADA DA PROPRIEDADE
      ```javascript
      console.log(caneco.size)
      console.log(caneco.name)
      // estou dando um log só na propriedade size ou name, dentro de caneco
      ``` 
    - Array
      - É usado para armazenar um conjunto de elementos de qualquer tipo em uma variável
      - Usa-se colchete
  ```javascript
  const arrayexample = ["texto", caneco.size ]
  const arrayexample = [elemento1, 25, false]
  ``` 