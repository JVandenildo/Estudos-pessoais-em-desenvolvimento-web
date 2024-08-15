# About HTML and Internet

Antes de mergulhar no que é HTML, é interessante apresentar alguns conceitos importantes para o ambiente que o HTML se encaixa:

- **Internet**. É a rede mundial de computadores que permite a comunicação de usuários do mundo todo. A **intranet** é uma rede privada que permite ao usuário interagir com pessoas da mesma organização;
- _**World Wide Web**_. Também conhecida como _web_, é um sistema que une dados dos sistemas de internet. Ou seja, internet é algo referente ao componentes físicos da rede global, enquanto a _web_ ao conjunto de dados compartilhados por esta rede. As páginas w*eb* visitadas em sites são esses dados;
- **Servidores _web_**. São servidores robustos que processam pedidos recebidos dos navegadores;
- _**Home page**_. É a primeira página recebida de um site por um servidor _web_. Uma Home Page é normalmente chamada de index.htm ou de default.htm. Os arquivos também podem possuir a extensão .html como padrão;
- **URL** (_**Universal Resource Locator**_). É o sistema de endereçamento usado pelos navegadores para localizar redes, computadores e arquivos na internet.

A internet é regida por **protocolos** para comunicação em rede. Eles determinam a comunicação entre computadores: como iniciar, como manter e como encerrar a comunicação. Alguns deles são:

- **HTTP** (_**Hyper Text Transfer Protocol**_). É o protocolo usado pelos servidores _web_ para transmitir documentos HTML pela internet;
- **FTP** (_**File Transfer Protocol**_). É outro protocolo muito utilizado para transmitir arquivos, porém sua interface gráfica não é tão agradável como do HTTP;
- **TCP** (_**Transfer Control Protocol**_). É um conjunto de protocolos para a transmissão de informação pela _web_, com função de verificar se os dados são transferidos de forma correta, na sequência apropriada e sem erros;
- **IP** (_**Internet Protocol**_). É um protocolo de endereçamento, que fornece o endereço de computadores na rede.

As páginas _web_ são armazenadas em arquivos com extensão **.htm** ou **.html**. Isto assegura que elas serão acessíveis por qualquer tipo de navegador por qualquer parte do mundo.

## Sumário

1. [HTML e a web](#html-e-a-web);
2. [HTML semântico e não semântico](#html-semântico-e-não-semântico).

## HTML e a _web_

_HyperText Markup Language_ (HTML), ou Linguagem de Marcação de [HiperTexto](https://www.w3.org/WhatIs.html), é uma das linguagens mais usadas para criação de páginas _web_, e que utiliza um formato simples de código, que pode ser gerado sem ajuda de aplicativos especiais.
Tudo que precisa para criar um documento HTML é um editor de texto [ASCII](http://www.asciitable.com/) como _NotePad_ (Bloco de Notas). Se for necessário verificar a formatação do documento durante a criação, pode usar qualquer navegador, já que todos são capazes de interpretar o código.
O HTML é uma linguagem que possibilita apresentar informações na internet. Aquilo que você vê quando abre uma página na internet é a interpretação que seu navegador faz do HTML.
Foi inventado em 1'990 por um cientista chamado [Tim Berners-Lee](https://www.w3.org/People/Berners-Lee/). A finalidade inicial era a de tornar possível o acesso e a troca de informações e de documentação de pesquisas, entre cientistas de diferentes universidades.
Uma função importante em aplicações _web_, que são programas que você incorporar em sites para gerenciar tarefas adicionais como, o gerenciamento de pedidos de usuários. Quando informações são inseridas em uma página _web_, o navegador a envia para um conjunto especial de programas chamados [Common Gateway Interface (CGI)](https://web.fe.up.pt/~goii2000/M9/cgi.htm) _scripts_. Estes programas processam a informação e exibem o resultado no navegador.
O HTML é usado para gerar uma interface básica para interação com aplicações _web_, como também para criar interfaces gráficas entre o banco de dados usados nestas aplicações e o usuário final.

## HTML semântico e não semântico

==Elementos semânticos== de HTML são os elementos que descrevem claramente o seu significado em uma leitura feita tanto pela máquina quanto por um humano. Esses elementos são pensados para aperfeiçoar a estrutura e acessibilidade de páginas _web_. Elementos semânticos comuns:

- `<header>`: define um cabeçalho para um documento ou seção;
- `<nav>`: define um conjunto de links de navegação;
- `<main>`: especifica o conteúdo principal de um documento;
- `<section>`: define uma seção em um documento;
- `<article>`: especifica um conteúdo independente e autocontido;
- `<aside>`: define um conteúdo além do conteúdo em que está incluído (como uma barra lateral);
- `<footer>`: define um rodapé para um documento ou seção;
- `<figure>`: especifica um conteúdo autocontido, como ilustrações, diagramas, fotos, etc.;
- `<figcaption>`: define uma legenda para o elemento `figure>`;
- `<time>`: define um tempo específico (ou uma data).

Exemplo de layout usando elementos semânticos:

![[HTMLsemantic_bm.svg]]

Exemplo de um código usando elementos semânticos:

```html
<header>
	<h1>My Website</h1>
	<nav>
		<a href="#home">Home</a>
		<a href="#about">About</a>
		<a href="#contact">Contact</a>
	</nav>
</header>
<main>
	<h2>Welcome</h2>
	<p>This is the main content of the website.</p>
</main>
<footer>
	<p>2024 My website</p>
</footer>
```

Os benefícios de elementos semânticos são:

- **Acessibilidade**: leitores de tela e outras tecnologias de assistência conseguem entender melhor a estrutura e o conteúdo de uma página _web_;
- **SEO**: sistemas de pesquisa podem entender melhor o conteúdo e a estrutura, potencialmente melhorando os rankings de procura;
- **Manutenção**: código é mais fácil de ler e manter;
- **Futuras atualizações**: aderir aos padrões assegura melhor suporte por diferentes navegadores e tecnologias futuras.

==Elementos não semânticos== de HTML são aqueles que não tem algum significado específico sobre seu conteúdo. Esses elementos são mais sobre estilização e _layout_ do que descrição de conteúdo. Alguns elementos não semânticos comuns são:

- `<div>`: um container genérico para fluxo de conteúdo;
- `<span>`: um container _inline_ genérico para conteúdo fraseado.

O uso desse tipo de elemento pode incluir:

- **Estilização**: usado como container para aplicar estilos de CSS;
- **_Hooks_ do JavaScript**: usado como _hooks_ para o JavaScript manipular partes de uma página _web_;
- **Layout**: usado para estruturar a página _web_ na falta de alternativas semânticas.

Exemplo de código HTML usando elementos não semânticos:

```html
<div class="header">
	<h1>My Website</h1>
	<div class="nav">
		<a href="#home">Home</a>
		<a href="#about">About</a>
		<a href="#contact">Contact</a>
	</div>
</div>
<div class="main">
	<h2>Welcome</h2>
	<p>This is the main content of the website.</p>
</div>
<div class="footer">
	<p>2024 My website</p>
</div>
```
