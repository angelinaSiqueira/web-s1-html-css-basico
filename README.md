### Aula 01 - Introdução à HTML e CSS

Iniciaremos com assuntos básicos de estrutura, nomenclatura e anatomia de HTML e CSS.
- [Editores de texto e organização de pastas](#editores-de-texto);
- [HTML: anatomia e introdução de tags](#html);
- [CSS: anatomia e introdução de propriedades](#css);
- [Classes, id](#classes-e-id);
- [Github Desktop](#github-desktop).

#### Editores de texto
Para se modificar um arquivo `.html` e `.css`, precisamos de editor de texto. Apesar de que um simples bloco de notas pode ser a ferramenta para criação desses arquivos, vários softwares foram lançados no mercado para gostos dos programadores, oferecendo funcionalidades e plugins para facilitar o desenvolvimento. Alguns  notáveis são:
- [Sublime Text](https://www.sublimetext.com/);
- [Notepad++](https://notepad-plus-plus.org/);
- [Atom](https://atom.io/);
- O que vamos usar durante as aulas é o [Visual Studio Code](https://code.visualstudio.com/);

A estrutura de pastas básicas é:
```
index.html
/css
    style.css
/img
    imagem.jpg
```
Ou seja, uma pasta com um arquivo `index.html` na raiz e duas pastas: uma `/css` para inserção de nossos estilos `.css` e outra `/img`, para inserção de nossas imagens.


#### HTML
HTML é a abreviação de **Hyper Text Markup Language** (linguagem de marcação em hipertexto). Ou seja, não se trata de uma linguagem de programação, pois não tem lógica (algoritmos, processos etc). Ele cria a **estrutura** de uma página ou aplicação web, determinando a separação de layout e seu conteúdo.

Documentos `.html` possuem tags de estruturação básica:
```html
<!doctype html>
<html>
    <head></head>
    <body></body>
</html>
```

Internamente, as tags html possuem uma anatomia básica também:
```html
<nome-da-tag atributo="valor do atributo">
    conteúdo
</nome-da-tag>
```

Comentários em HTML:
```html
<!-- Isso é um comentário. Comentários em qualquer linguagem são pedaços de código que são ignorados na renderização (na leitura do computador), mas são úteis para entedimento humano -->
```

#### CSS
CSS é abreviação de **Cascading Style Sheet** (folha de estilos em cascata). É a linguagem que define **estilos** para o HTML, portanto, não se trata de linguagem de programação. CSS tem "cascata" no nome, devido a sua forma de determinar a propriedade de um elemento - levando em consideração *hierarquia de seletores* e de chamadas de estilo (_inline, internal e external_).

Para fazer o link de um arquivo `.css` em um documento `.html`, devemos inserir a tag `<link>` no `<head>` do documento, com o `href` do caminho do arquivo.
```html
<!doctype html>
<html>
    <head>
        <link rel="stylesheet" href="css/style.css">
    </head>
    <body></body>
</html>
```

Dentro do arquivo `.css`, a anatomia é:
```css
seletor {
    propriedade: valor;
}
```

Exemplo:
```css
p {
    color: red;
}
```

Comentários em CSS:
```css
/* Sou um comentário CSS */
```


> **ATENÇÃO!**
> Não esqueçam de **indentar** o código! Isso ajuda na sua legibilidade, manutenção e colaboração com outros desenvolvedores.
>
> Para indentar, selecione a linha do código e aperte *tab*.

#### Classes e id
Classes e ids são atributos que podem ser inseridos em qualquer tag dentro da `<body>`. Eles são **atributos de nomeação**, sendo `class` usada majoritariamente para referência em CSS e `id` para Javascript.
Uma diferença entre os dois é que podem haver várias classes com o mesmo valor, ao passo que ids devem ser **únicos**.


#### Propriedades e tags
Verificar os arquivos de exercícios para vê-los em prática.

HTML | CSS
------------ | -------------
Tags de **estrutura**: !doctype, html, head, body | Propriedades de **background**: background-imagem, background-color
Tags no **head**: meta (charset), title, link | Propriedades de **texto**: text-align, font-family, font-size, text-decoration, font-size, text-transform
Tags de **divisão**: div | Propriedades de **layout**: width, margin, padding, display (inline-block)
Tags de **texto**: h1 ao h6, p | Propriedade de **cor**: color
Tag de **link**: a | Propriedade de **decoração**: box-shadow, border
Tag de **imagem**: img |

**Macete de centralização**: apenas para elementos block.
1. Definir um tamanho para seu elemento através da propriedade `width`;
2. Definir `margin: 0 auto;`


#### Github Desktop
Github é uma rede de repositórios de códigos abertos, muito utilizada por desenvolvedores.

Para a primeira semana, vamos utilizar a versão software do [Github](https://desktop.github.com/).
