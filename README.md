# Bem Vindo ao Meu Grimório!!!
Aqui eu compartilho todo o conhecimento que eu já adiquiri sobre JavaScript.   
A maioria das coisas que eu ja aprendi foi pelo curso da [Origamid](https://www.origamid.com/).

## DOM
### O Que É?
O DOM É uma interface que representa documentos HTML através de objetos. Com ela é possivel manipular a estrutura, estilo e conteúdo desses documentos.
#### Exemplo:   
Um exemplo de DOM é a parte de elements do menu inspecionar.
![image](https://github.com/user-attachments/assets/5c4b5d9e-7bf0-4013-ae37-7235e90868ad)

## Elementos Primitívos
### O Que É?
Os elementos primitívos são os elementos "principais" do JavaScript.
### Quais São?
**String**: Representa um texto.
```js
  var mensagem = "Olá!"
  console.log(mensagem) // Olá!
```
**Boolean**: Representa uma entidade lógica e pode ter 2 valores (true e false).
```js
  var conta = 1 + 1 == 3
  console.log(conta) // false
```
**Null**: Representa algo vazio. Geralmente usado para indentificar se algo está sem dados.
```js
  var lista
  console.log(lista == null) // true
```
**Undefined**: Apresenta uma variável sem dados.
```js
  var minhaVariavel
  console.log(minhaVariavel) // undefined
```

## Variáveis
### O Que É?
As variaveis são uma maneira de "armazenar" as coisas e usá-las de uma forma mais prática.
### Tipos
**Var**: Variável que pode ser modificada de qualquer nivel de escopo.
```js
  var conta = 1 + 1
```
**Let**: Variável que pode ser modificada apenas pelo seu escopo ou superior.
```js
  let conta = 1 + 1
```
**Const**: Variável que não pode ser modificada de forma alguma.
```js
  const conta = 1 + 1
```

## Seleção de Elementos
### O Que É?
No JavaScript a seleção de elementos é muito importante, pois é assim que podemos adicionar, remover e modificar elementos do HTML.
### Como selecionar
Existem várias maneiras de selecionar elementos no JavaScript. Essas são:  
<br>**querySelector**: Seleciona o primeiro elemento que combinar com um seletor CSS específico.
```js
  const paragrafo = document.querySelector("p")
  cnosole.log(paragrafo) // <p>Esse é o prmeiro parágrafo do site.</p>
```
**querySelectorAll**: Seleciona todos elementos que combinarem com um seletor CSS específico.  (_Essa função retorna uma Array_)
```js
  const paragrafos = document.querySelectorAll("p")
  cnosole.log(paragrafo) // [p.p1, p.p1]
```
**getElementById**: Seleciona um elemento HTML por um id específico.
```js
  const titulo = document.getElementById("titulo1")
  cnosole.log(titulo) // <h1 id="titulo">Titulo do Site</h1>
```
**getElementsByClassName**: Seleciona todos elementos HTML de uma classe específica.  (_Essa função retorna uma Array_)
```js
  const links = document.getElementsByClassName("link")
  cnosole.log(links) // [a.link, a.link, a.link, a.link]
```
**getElementsByTagName**: Seleciona todos elementos por uma tag HTML específica.  (_Essa função retorna uma Array_)
```js
  const paragrafos = document.getElementsByTagName("img")
  cnosole.log(paragrafo) // [img.logoSite, img.background]
```
**getElementsByName**: Seleciona todos elementos por um atributo name HTML específico.  (_Essa função retorna uma Array_)
```js
  const feedbacks = document.getElementsByName("textarea")
  cnosole.log(paragrafo) // [textarea.fbModelo1, img.fbModelo2]
```
**getAttribute**: Seleciona um elemento por um atributo HTML específico.
```js
  const botaoAtivo = document.getAttribute('data-botao="ativo"')
  cnosole.log(botaoAtivo) // <button data-botao="ativo">Clique Aqui</button>
```

## If, Else e Else If
### O Que É?
Os **If, Else e Else If** são maneiras de dizer que uma coisa só pode acontecer com uma condição específica.
### Exemplo:
_Usando para avisar no console se a variavel X é maior, menor ou igual a 3._
```js
  x = 4

  if (x < 3) {
    console.log("X é menor que 3!")
  } else if (x > 3) {
    console.log("X é maior que 3!")
  } else {
    console.log("X é igual a 3!")
  }
```

## Switch Case
### O Que É?:
O **Switch Case** uma maneira de definir situações que acontecem de acordo com diversas opções.
### Exemplo
_Usando para usar que numero o usuário escolheu._
```js
  escolha = 3

  switch (escolha) {
    case 1:
      console.log("O usuário escolheu o 1.");
      break;
    case 2:
      console.log("O usuário escolheu o 2.");
      break;
    case 3:
      console.log("O usuário escolheu o 3.");
      break;
    case 4:
      console.log("O usuário escolheu o 4.");
      break;
    default:
      console.log("O usuário não escolheu nada.")
  }
```
