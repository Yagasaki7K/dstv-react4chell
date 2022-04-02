<p align="center">
  <a href="https://github.com/ApertureLaboratory">
    <img alt="Aperture Laboratories - Chell Series" src="https://github.com/ApertureLaboratory/4chell/blob/main/.github/ChellSeries.png" />
    </a>    
</p>

<p align="center">
  <h2 align="center">React - Básico ao avançado | IICA</h2>
  
  <p align="center">
    <br />
    <a href="#Sumário"><strong>Explore o sumário »</strong></a>
    <br />
    <br />
    <a href="https://github.com/Yagasaki7K/react4chell/issues">Reportar um problema</a>
    ·
    <a href="https://github.com/Yagasaki7K/react4chell/issues">Solicitar uma funcionalidade</a>
  </p>
</p>

## Sobre o Projeto
Nesse artigo você aprenderá os conceitos básicos e avançados do Desenvolvimento Web utilizando o React como ferramenta, um framework Javascript que veio para facilitar a vida do desenvolvimento.

Esse artigo possuí o selo IICA - Introdução, Instalação e Criação do Aplicativo.

## Sumário

- [Introdução](#o-que-é-desenvolvimento-web)
    - [O que significa ser reativo?](#o-que-significa-ser-reativo)
    - [Componentização do React](#componentização-do-react)
- [Aprendendo mais](#aprendendo-mais)
- [1. Instalação](https://github.com/Yagasaki7K/react4chell/blob/main/documenta%C3%A7%C3%A3o/1.instala%C3%A7%C3%A3o/README.md)
- [2. Create-react-app](https://github.com/Yagasaki7K/react4chell/blob/main/documenta%C3%A7%C3%A3o/2.create-react-app/README.md)
- [3. Componentes](https://github.com/Yagasaki7K/react4chell/blob/main/documenta%C3%A7%C3%A3o/3.%20componentes/README.md)
- [4. Estados](https://github.com/Yagasaki7K/react4chell/blob/main/documenta%C3%A7%C3%A3o/4.%20estados/README.md)
- [5. Eventos](https://github.com/Yagasaki7K/react4chell/tree/main/documenta%C3%A7%C3%A3o/5.%20eventos)
- [6. React Hooks](https://github.com/Yagasaki7K/react4chell/blob/main/documenta%C3%A7%C3%A3o/6.%20react%20hooks/README.md)
- [Como contribuir](#como-contribuir)

## Introdução
Inicialmente recomendamos fortemente que você tenha uma base sólida de HTML, CSS e Javascript, pois o React é uma linguagem Javascript que é utilizada para construir interfaces de usuário e caso você não tenha entendimento sobre a base, nada adianta tentar escalar o resto.

A história é simples, React é um framework reativo desenvolvido pela Facebook - atualmente Meta Platforms, Inc.

### O que significa ser reativo?
Significa que você consegue pegar um certo local da aplicação, um componente, e atualizar ele sem necessidade alguma de atualizar a página inteira. Imaginando esse conceito, imagine o quão trabalhoso seria para o Facebook atualizar seu feed de notícias toda vez que tivesse alguma coisa nova, mas atualizar no sentido completo, todo, usando basicamente um F5 para isso.

Isso iria levar um grande tempo - levando em conta a quantidade de conteúdo gerado diariamente - iria levar um grande pacote de dados consigo, usuários do mobile iriam chorar e sem falar que toda a aplicação ficaria demasiadamente pesada e talvez, impossível de ficar utilizando, sendo que a cada cinco minutos, teria atualizado umas três, quatro vezes.

Eis que em Maio de 2013, surge o React para resolver todo esse problema complexo e facilitando a vida de vários desenvolvedores. Claro que o React não é apenas uma biblioteca capaz de APENAS fazer isso, existem muitas outras funcionalidades que podem e devem ser utilizadas com o React como o sistema de componentização.

### Componentização do React
O que é componentes como foi comentado anteriormente? Isso é um esquema que tive uma dificuldade enorme para pegar e conseguir de fato entender, mas graças ao Vue.js, consegui ter mais facilidade em aprender como funcionava essa ambientação nova.

Imagine que você pega seu website desenvolvido em puro HTML e CSS e gostaria de quebrar ele em várias partes. Bom, você atualmente já faz isso utilizando divs, correto? Você vai lá, cria uma div chamada "header" para definir a cabeça da sua aplicação, "nav" da parte de navegação, "container" do corpo daquela estrutura e "footer" para definir o rodapé, correto? Isso é uma aplicação simples.

Agora imagine você componetizar isso? É uma maneira diferente, mas com o mesmo propósito e com mais facilidade, já que você vai pegar cada parte dessa quebra e definir com iniciais maiusculas. Ao invés de `<div class="header"></div>`, você chamará agora de `<Header></Header>` e você poderá passar propriedades para ele de uma maneira mais dinâmica, permitindo passar informações com muito mais facilidade entre os demais, como `<Nav>`, `<Container>` e `<Footer>`, o que permite uma estilização personalizada para cada um, utilizando o styled-components e bom, isso facilita demais, caso você precise utilizar o mesmo componente em várias partes da aplicação, dessa maneira, você não precisa ficar no Ctrl+C e Ctrl+V, o que precisa fazer é apenas importar o componente para quando for utilizar ele, as possibilidades são ilimitadas.

Vale lembrar que para criar um `<Container>`, você deverá criar um arquivo como container.js, container.jsx - caso esteja utilizando JSX - ou container.tsx - caso esteja utilizando Typescript e importar ele aonde você desejar.

Um exemplo disso, utilizando o container, seria:

Em caso de importar um componente:
```
import React from 'react';
import { Container } from './components/container;
return () => {
    <Container>
}
```

ou

Em caso de criação de um componente:
```
import React from 'react';
const Container = () => { 
    <p> Hello World </p> 
}

export default Container
```

Não existe um padrão de arquitetura que você pode seguir com o React - ainda

Mas cuidado com a organização e as declaração, procure se informar se o `<Header>` é uma propriedade privada da própria biblioteca, como o caso de `<Image>` no NextJS - o filho do React, mas é um tema para outro artigo - utilizado para fazer uma importação de imagem, substituindo o famoso `<img>` e deixando bem mais otimizado.

## Aprendendo mais ...

Mas não se preocupe, caso você não tenha entendido nada, isso é apenas uma introdução de uma das possibilidades que o React consegue fazer, quer aprender mais e se aprofundar? Então me siga nessa jornada e vamos mostrar o passo a passo do básico ao avançado no React.

O que é necessário para aprender React? HTML, CSS e Javascript. É ideal já ter o [NodeJS](https://nodejs.org/pt-br/download/) ou [Yarn](https://classic.yarnpkg.com/en/docs/install#windows-stable) instalado em sua máquina para seguir os próximos passos.

- [1. Instalação](https://github.com/Yagasaki7K/react4chell/blob/main/documenta%C3%A7%C3%A3o/1.instala%C3%A7%C3%A3o/README.md)
- [2. Create-react-app](https://github.com/Yagasaki7K/react4chell/blob/main/documenta%C3%A7%C3%A3o/2.create-react-app/README.md)
- [3. Componentes](https://github.com/Yagasaki7K/react4chell/blob/main/documenta%C3%A7%C3%A3o/3.%20componentes/README.md)
- [4. Estados](https://github.com/Yagasaki7K/react4chell/blob/main/documenta%C3%A7%C3%A3o/4.%20estados/README.md)
- [5. Eventos](https://github.com/Yagasaki7K/react4chell/tree/main/documenta%C3%A7%C3%A3o/5.%20eventos)
- [6. React Hooks](https://github.com/Yagasaki7K/react4chell/blob/main/documenta%C3%A7%C3%A3o/6.%20react%20hooks/README.md)

## Como Contribuir

Contribuições fazem com que a comunidade open source cresça, evoluia e você tenha reconhecimento por ter ajudado em um projeto tão maravilhoso
Todas contribuições são **extremamente apreciadas e avaliadas**

1. Realize um Fork do projeto
2. Crie um branch com a nova feature (`git checkout -b feature/nome-do-artigo`)
3. Realize o Commit (`git commit -m 'Adicionado novo item na enciclopédia'`)
4. Realize o Push no Branch (`git push origin feature/nome-do-artigo`)
5. Abra um Pull Request

## Autores do Artigo

- **Anderson "Yagasaki" Marlon** - _Dev Front-end e Graduado no CC50 de Harvard_ - [@Yagasaki7k](https://twitter.com/Yagasaki7K)
- Contribuidores - [Lista de contribuidores](https://github.com/Yagasaki7K/react4chell/graphs/contributors)