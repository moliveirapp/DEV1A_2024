# Explicação das Tags HTML

## `<!DOCTYPE html>`
Declaração que informa ao navegador que o documento está escrito em HTML5.

## `<html lang="pt-BR">`
Elemento raiz do documento HTML. O atributo `lang="pt-BR"` define o idioma do conteúdo como português do Brasil.

## `<head>`
Contém meta-informações sobre o documento, como título, links para estilos, scripts, metadados, etc.

## `<meta charset="UTF-8" />`
Especifica a codificação de caracteres do documento como UTF-8, que suporta quase todos os caracteres de todas as línguas escritas.

## `<meta name="viewport" content="width=device-width, initial-scale=1.0" />`
Controla como a página é exibida em dispositivos móveis. `width=device-width` define a largura da página para seguir a largura da tela do dispositivo, e `initial-scale=1.0` define o nível de zoom inicial quando a página é carregada.

## `<title>Document</title>`
Define o título do documento, exibido na aba do navegador ou na barra de título da janela.

## `<body>`
Contém todo o conteúdo que será exibido na página web, como textos, imagens, links, tabelas, etc.

## `<!-- isso é um comentário do meu código, detalhe que, no HTML, os comentários FICAM VISÍVEIS -->`
Comentário no código HTML, que não é exibido na página renderizada, mas é visível no código-fonte.

## `<h1>Título usando H1</h1>`
Cabeçalho de nível 1, usado para títulos principais.

## `<h2>Título usando H2</h2>`
Cabeçalho de nível 2, usado para subtítulos.

## `<h3>Título usando H3</h3>`
Cabeçalho de nível 3, usado para subtítulos de menor importância.

## `<p>Isso é um parágrafo simples, sem nenhum tipo de formatação, estilização, usando a tag p</p>`
Define um parágrafo de texto.

## `<div>`
Elemento de bloco que serve como contêiner para outros elementos, permitindo a organização do conteúdo em seções.

## `<strong>negrito</strong>`
Define texto em negrito, com ênfase semântica.

## `<b>negrito</b>`
Define texto em negrito, sem ênfase semântica.

## `<i>itálico</i>`
Define texto em itálico, com ênfase semântica.

## `<strong><i>Negrito E itálico</i></strong>`
Combina tags para definir texto em negrito e itálico, com ênfase semântica.

---

```html
<!DOCTYPE html>
<html lang="pt-BR">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <!-- isso é um comentário do meu código, detalhe que, no HTML, os comentários FICAM VISÍVEIS -->
    <h1>Título usando H1</h1>
    <h2>Título usando H2</h2>
    <h3>Título usando H3</h3>
    <p>
      Isso é um parágrafo simples, sem nenhum tipo de formatação, estilização,
      usando a tag p
    </p>
    <div>
      <p>
        Aqui temos um texto DENTRO de uma DIV, a div serve para separarmos os
        conteúdos em seções. Iremos aprender a estilizar as divs.
      </p>
      <p>
        Aqui temos uma palavra em <strong>negrito</strong> usando a tag strong,
        ou podemos também usar a tag b para deixar o texto em <b>negrito</b>
      </p>
      <p>
        Também podemos criar palavras em <i>itálico</i>, usando a tag i Podemos
        misturar e deixar <strong><i>Negrito E itálico</i></strong>
      </p>
    </div>
  </body>
</html>
