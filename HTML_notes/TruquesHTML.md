# Truques no HTML

Abaixo um _cheatsheet_ de atributos do HTML:

| Nome              | Descrição                                                                                                                                                                                                                  | Exemplo                                                  |
| ----------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| _preload_         | otimizar o carregamento de mídias como áudio e vídeo. adicionar, o atributo _preload_ a um elemento `<link>` para indicar ao navegador que pré-carregue um recurso                                                         | `<link rel="stylesheet" href="style.css" preload>`       |
| _translate_       | adicionar o atributo `translate="no"` a um elemento HTML para indicar que o conteúdo não deve ser traduzido automaticamente pelo navegador.                                                                                | `<p translate="no">Texto que não deve ser traduzido</p>` |
| _hidden_          | adicionar o atributo `hidden` a um elemento HTML para ocultá-lo. pode ser útil para mostrar ou ocultar elementos com base em ações do usuário, como um botão “Mostrar mais” que revela conteúdo adicional.                 | `<div hidden>Conteúdo oculto</div>`                      |
| _contenteditable_ | transformar elementos em áreas editáveis. é ideal para criar conteúdos interativos em que os usuário poderão editar diretamente na página.                                                                                 | `<p contenteditable="true">Texto editável</p>`           |
| _spellcheck_      | desabilitar a verificação ortográfica automática nos campos de texto do _site_. isso pode ser útil para permitir que os usuários insiram palavras personalizadas ou gírias sem que sejam marcadas como erros ortográficos. | `<input type="text" spellcheck="false">`                 |

## Sumário

1. [Carregamento de imagem lento (lazy)](#carregamento-de-imagem-lento-lazy);
2. [Sugestões de entrada](#sugestões-de-entrada);
3. [Document refresher](#document-refresher);
4. [URL base](#url-base);
5. [A tag "picture"](#a-tag-picture).

## Carregamento de imagem lento (`lazy`)

O carregamento de lento previne o carregamento de imagens que não são realmente necessárias na tela imediatamente. A medida que se aproxima da imagem, a imagem começa carregar. Exemplo:

```html
<img src="image.png" loading="lazy" width="200" height="200" />
```

## Sugestões de entrada

Para usar sugestões úteis e relevantes quando está tentar procurar por algo realmente interessante.

```html
<label for="country">Choose your country from the list:</label>
<input list="countries" name"country" id="country">

<datalist id="countries">
	<option value="UK"></option>
	<option value="Germany"></option>
	<option value="USA"></option>
	<option value="Japan"></option>
	<option value="India"></option>
</datalist>
```

## Document refresher

O exemplo abaixo irá redirecionar o usuário para a URL que é "[https://google.com](https://google.com/)" em 4 segundos e então coloca para 0 para um redirecionamento imediato.

```html
<meta http-equiv="refresh" content="4, URL='https://google.com'" />
```

## URL base

Esta _tag_ ajuda quando se tem muitas _tags_ _anchor_ redirecionando a uma mesma URL e todas URLs começam com o mesmo endereço base.
Exemplo:

```html
<head>
	<base href="https://www.twitter.com/" target="_blank" />
</head>
<body>
	<a href="ElonMusk">Elon Musk</a>
</body>
```

## A _tag_ `picture`

Usar a _tag_ `<picture>` permite adicionar múltiplas imagens encaixando diferentes larguras ao invés de ter a única imagem. Exemplo:

```html
<picture>
	<source media="(min-width:769px)" srcset="medium.jpg" />
	<source media="(min-width:495px)" srcset="small.jpg" />
	<img src="high_image.jpg" alt="Flags" style="width:auto" />
</picture>
```
