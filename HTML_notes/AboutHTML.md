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

1. [HTML e a _web_](#html-e-a-web);
2. [HTML semântico e não semântico](#html-semântico-e-não-semântico);
3. [Boas práticas em HTML](#boas-práticas-em-html);
4. [Referências](#referências).
   1. [Referências em artigos da _web_](#referências-em-artigos-da-web);
   2. [Referências em vídeos](#referências-em-vídeos).

## HTML e a _web_

_HyperText Markup Language_ (HTML), ou Linguagem de Marcação de [HiperTexto](https://www.w3.org/WhatIs.html), é uma das linguagens mais usadas para criação de páginas _web_, e que utiliza um formato simples de código, que pode ser gerado sem ajuda de aplicativos especiais.  
É uma linguagem usada no _frontend_, sendo a estrutura da página _web_ que pode ser estilizada usando CSS e ser interativa com JavaScript.  
Tudo que precisa para criar um documento HTML é um editor de texto [ASCII](http://www.asciitable.com/) como _NotePad_ (Bloco de Notas). Se for necessário verificar a formatação do documento durante a criação, pode usar qualquer navegador, já que todos são capazes de interpretar o código.
O HTML é uma linguagem que possibilita apresentar informações na internet. Aquilo que você vê quando abre uma página na internet é a interpretação que seu navegador faz do HTML.
Foi inventado em 1'990 por um cientista chamado [Tim Berners-Lee](https://www.w3.org/People/Berners-Lee/). A finalidade inicial era a de tornar possível o acesso e a troca de informações e de documentação de pesquisas, entre cientistas de diferentes universidades.
Uma função importante em aplicações _web_, que são programas que você incorporar em sites para gerenciar tarefas adicionais como, o gerenciamento de pedidos de usuários. Quando informações são inseridas em uma página _web_, o navegador a envia para um conjunto especial de programas chamados [Common Gateway Interface (CGI)](https://web.fe.up.pt/~goii2000/M9/cgi.htm) _scripts_. Estes programas processam a informação e exibem o resultado no navegador.
O HTML é usado para gerar uma interface básica para interação com aplicações _web_, como também para criar interfaces gráficas entre o banco de dados usados nestas aplicações e o usuário final.

## HTML semântico e não semântico

Elementos semânticos de HTML são os elementos que descrevem claramente o seu significado em uma leitura feita tanto pela máquina quanto por um humano. Esses elementos são pensados para aperfeiçoar a estrutura e acessibilidade de páginas _web_. Elementos semânticos comuns:

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

Elementos não semânticos de HTML são aqueles que não tem algum significado específico sobre seu conteúdo. Esses elementos são mais sobre estilização e _layout_ do que descrição de conteúdo. Alguns elementos não semânticos comuns são:

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

## Boas práticas em HTML

Aqui faz presente uma lista com boas práticas em HTML

1. Declarar o _doctype_ HTML5 corretamente;

   ```html
   <!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
   ```

   _doctype rigoroso para HTML 4.01._

   ```html
   <!DOCTYPE html:
   ```

   _doctype para HTML5._

2. Usar somente um elemento `<h1>` em uma única página HTML para melhor SEO (Search Engine Optimization). [Artigo](https://rockcontent.com/br/blog/o-que-e-seo/) sobre SEO;
3. Usar o elemento figure para adicionar legendas às imagens no HTML;

   ```html
   <div>
   	<img
   		src="a-man-coding.png"
   		alt="A man working on his
    computer"
   	/>
   	<p>This is a picture of a man working on his computer</p>
   </div>
   ```

   _Sem o elemento figure._

   ```html
   <figure>
   	<img
   		src="a-man-coding.jpg"
   		alt="A man working on his
    computer"
   	/>
   	<figcaption>This is a picture of a man working on his computer</figcaption>
   </figure>
   ```

   _Com o elemento figure._

4. Não usar divs para criar _headers_ e _footers_, usar elementos apropriados;

   ```html
   <div class="header">
   	<a href="index.html">Home</a>
   	<a href="#">About</a>
   	<a href="#">Contact</a>
   </div>

   <div class="footer">
   	<a href="index.html">Home</a>
   	<a href="#">About</a>
   	<a href="#">Contact</a>
   </div>
   ```

   _Sem os elementos apropriados._

   ```html
   <header>
   	<h1>Brand Name</h1>
   </header>

   <footer>
   	<a href="index.html">Home</a>
   	<a href="#">About</a>
   	<a href="#">Contact</a>
   </footer>
   ```

   _Com os elementos apropriados._

5. Evitar o uso de `<b>` e `<i>` para tornar os textos negrito e itálico em uma página web, use as tags `<strong>` e `<em>`;

   ```html
   <p><i>Code at your own pace</i></p>
   <p></p>
   <p><b>Code at your own pace</b></p>
   <p></p>
   ```

   ```html
   <p><strong>Code at your own pace</strong></p>
   <p><em>Code at your own pace</em></p>
   ```

6. Não colocar elementos a nível de bloco dentro de elementos de linha;

   ```html
   <a href="#">
   	<p>Visit Blog Site</p>
   </a>
   ```

   _Não é tão interessante._

   ```html
   <p>
   	Visit <a href="www.myblog.com" target="_blank"> My Blog Site</a> to learn
   	JavaScript.
   </p>
   ```

   _Mais interessante._

7. Minimize o CSS externo e vincule-o ao documento HTML;
8. Nunca use CSS dentro de um documento HTML;
9. Não use _divs_ para tudo;
10. Feche todas as _tags_ HTML;
11. Use marcação em minúsculo;
12. Use o atributo _alt_ nas imagens;
13. Evite comentários em excesso;
14. Siga a hierarquia para elementos de cabeçalho.

## Referências

1. [roadmap.sh/frontend](https://roadmap.sh/frontend);
2. [app.daily.dev/tags/html?ref=roadmapsh](https://app.daily.dev/tags/html?ref=roadmapsh.).

### Referências em artigos da _web_

1. [w3schools.com/html/html_intro.asp](https://www.w3schools.com/html/html_intro.asp);
2. [Artigo no MDN Docs](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started) com introdução ao HTML;
3. [Artigo no web.dev](https://web.dev/learn/html) sobre introdução ao HTML;
4. [cs.fyi/guide/writing-semantic-html](https://cs.fyi/guide/writing-semantic-html);
5. [cs.fyi/guide/writing-semantic-html](https://cs.fyi/guide/writing-semantic-html);
6. [w3schools.com/html/html5_semantic_elements.asp](https://www.w3schools.com/html/html5_semantic_elements.asp);
7. [hackernoon.com/how-to-write-semantic-html-dkq3ulo](https://hackernoon.com/how-to-write-semantic-html-dkq3ulo);
8. [blog.hubspot.com/website/semantic-html](https://blog.hubspot.com/website/semantic-html);
9. [html.com/semantic-markup](https://html.com/semantic-markup);
10. [web.dev/learn/html/semantic-html/](https://web.dev/learn/html/semantic-html/).

### Referências em vídeos

1. Vídeo "[HTML Full Course - Build a Website Tutorial](https://youtu.be/pQN-pnXPaVg)" do canal [@freecodecamp](https://www.youtube.com/@freecodecamp).;
2. Vídeo "[HTML Tutorial for Beginners: HTML Crash Course](https://youtu.be/qz0aGYrrlhU)" do canal [@programmingwithmosh](https://www.youtube.com/@programmingwithmosh).
