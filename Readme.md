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


## AULA 2 - BASICO DO JavaScript

- Declarações de Variáveis (const, let, var)
  - Const
    - Não pode ser mudada e nem declarada sem valor
  ```javascript
  const name = ["Mateus"]
  const size = ["gigas"]
  ```
  - Let
    - Pode ser mudada e declarada sem valor
  ```javascript
  let name = ["Mateus"]
  let size = ["monstrao"]
  ```
  - Var
    - Possui caracteristicas da const e let, mas esta caindo em desuso.   
  
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

- OPERAÇÕES ARITMÉTICAS
  - \+  (soma)
  - \-  (subtração)
  - \*  (multiplicação)
  - /   (divisão)
  - %   (é a sobra da divisão)
  - \** (Elevado)
  - \** (1/2) (raiz quadrada do numero)


- OPERAÇÕES COMPARADORAS
  - = (atribui um valor a uma variável)
  - == (compara se o valor é igual ao outro)
  - === (compara o valor e o tipo da variável)
  ```javascript
    9 ** (1 / 2)  // 3 ( Raiz quadrada de 9)
    9 ** 1 / 2  // 4.5 ( 9 elevado a 1, divido por 2)
    9 % 3  // 0 (9 dividido por 3, sobra 0)
    10 % 3  // 1 ( 10 divido por 3, sobra 1)
    
    2 == 2  // true ( compara 2 por 2)
    2 == 3  // false (compara 2 por 3)
    2 === 2  // true ( compara tanto o valor quanto o tipo)
    2 === 3  // false ( compara tanto o valor quanto o tipo)
    2 == "2"  // true (compara 2 com o valor 2, mas são tipos diferentes)
    2 == "3"  // false (compara 2 com o valor 3, mas são tipos diferentes)
    2 === "2"  // false 

    true === "true"  // false
    true == "true"  // false
    false == "false"  // false
    false === "false"  // false

    "hakjsda"  // hakjsda
    !!0  // false
    
  ```
  - !== (diferente)
  ```javascript
    2 != "2" // false 
    2 != "3" // true 
  ```
  - !=== ()
  ```javascript
    2 !=== "2" // true ( compara tanto o numero quanto o tipo) 
  ``` 
  - < (menor)
  - \> (maior)
  - <= (menor ou igual)
  - \>= (maior ou igual)

- OPERAÇÕES LOGICAS
  - && e
  ```javascript
  0 * 0 -> 0
  0 * 1 -> 0
  1 * 0 -> 0
  1 * 1 -> 1
  ```
  - || ou
  ```javascript
  0 + 0 -> 0
  0 + 1 -> 1
  1 + 0 -> 1
  1 + 1 -> 1
  ```
  - ! not (inverte o valor do elemento)
  ```javascript
  !0 -> 1
  !1 -> 0
  ```

- BLOCOS

- FUNÇÕES
  - Declaração 1
  ```javascript
    function exemplo(atributo) {
      // o que a função vai fazer
    }
    // atributo é o valor que recebo quando chamo a função (não necessariamente precisa ter)
  ```
  - Declaração 2
  ```javascript
    const exemplo = (atributo) => {
      // o que a função vai fazer
    }
    
  ```
  - Chamada
  ```javascript
  console.log(exemplo)// somente pego o valor que ta guardado dentro dela//
  console.log(exemplo()) // a função sendo executada
  ```
  - Retorno
  ```javascript
  //PRIMEIRA FORMA
  function exemplo () {
    return "deucerto"
  }

  console.log(exemplo()) // deucerto

  // SEGUNDA FORMA
  const exemplo = () => {
  return "deucerto";
  };

  console.log(exemplo()); // deucerto
  ```
