---
sidebar_position: 4
---

# Sintaxe Markdown

## Títulos

Para criar um título, adicione um ou mais símbolos # antes do texto do título. O número de # que você usa determina a hierarquia e o tamanho da fonte dos tipos de título.

```md
# Um título de primeiro nível
## Um título de segundo nível
### Um título de terceiro nível
```

# Estilo do texto

Você pode indicar ênfase com negrito, itálico, tachado, subscrito ou sobrescrito em campos de comentários e ficheiros .md.

Estilo | Atalho do teclado | Exemplo | Saída
------ | ----------------- | ------- | -----
Negrito | CTRL + B (Windows/Linux) ou ⌘ + B (Mac) | `**texto**` ou `__texto__` | **texto**
Itálico | CTRL + I (Windows/Linux) ou ⌘ + I (Mac) | `*texto*` ou `_texto_` | *texto*
Tachado | CTRL + T (Windows/Linux) ou ⌘ + T (Mac) | `~~texto~~` | ~~texto~~
Subscrito | CTRL + = (Windows/Linux) ou ⌘ + = (Mac) | `H~2~O` | H<sub>2</sub>O
Sobrescrito | CTRL + SHIFT + = (Windows/Linux) ou ⌘ + SHIFT + = (Mac) | `X^2^` | X<sup>2</sup>
Código | CTRL + K (Windows/Linux) ou ⌘ + K (Mac) | `` `texto` `` ou `` ```texto``` `` | `texto`

# Listas

Você pode criar uma lista não ordenada precedendo uma ou mais linhas de texto com `*` ou `-`.

```md
- George Washington
* John Adams
- Thomas Jefferson
```

**Output:**

- George Washington
- John Adams
- Thomas Jefferson

## Listas Ordenadas

Para ordenar a lista, coloque um número na frente de cada linha.

```md
1. James Madison
2. John Quincy Adams
```

**Output:**

1. James Madison
2. John Quincy Adams

## Listas com Letras

Para criar uma lista com letras, coloque uma letra seguida de um ponto na frente de cada linha.

```md
A. George Washington  
B. John Adams  
B. Thomas Jefferson  
```

**Output:**

A. George Washington  
B. John Adams  
C. Thomas Jefferson

## Listas aninhadas

Você pode criar uma lista aninhada recuando um ou mais itens da lista abaixo de outro item.

Para criar uma linha aninhada usando o editor Web do GitHub ou um editor de texto que use uma fonte mono espaçada, como o VS Code, você pode alinhar a lista visualmente. Digite os caracteres de espaço na frente do item de lista aninhado até que o caractere do marcador da lista(`-` ou `*`) fique diretamente abaixo do primeiro caractere do texto no item acima dele.

```md
1. First list item
2. Second list item
   - First nested list item
     - Second nested list item
```

**Output:**

1. First list item
2. Second list item
   - First nested list item
     - Second nested list item

# Texto de referência

Você pode citar um texto com >

```md
Text that is not a quote

> Text that is a quote
```

**Output:**

Text that is not a quote

> Text that is a quote

# Links

Você pode criar um link embutido colocando o texto do link entre colchetes [ ] e colocando a URL entre parênteses ( ).

```md
This site was built using [GitHub Pages](https://pages.github.com).
```

**Output:**

This site was built using [GitHub Pages](https://pages.github.com).

## Links relativos

É possível definir links relativos e caminhos de imagens em ficheiros representados para ajudar os leitores a aceder um outros ficheiros no repositório .

Por exemplo, se você tiver um ficheiro CONTRIBUTING.md no repositório e outro ficheiro em docs/CONTRIBUTING.md, o link relativo para o ficheiro em docs/CONTRIBUTING.md poderá ter um texto como:

```md
[Contribution guidelines for this project](docs/CONTRIBUTING.md)
```

**Output:**

[Contribution guidelines for this project](docs/CONTRIBUTING.md)

GitHub transformará automaticamente o link relativo caminho da imagem baseado em qualquer branch em que você estiver no momento, para que o link ou caminho funcione sempre. O caminho do link será relativo ao ficheiro atual. Os links que começam com `/` serão relativos à raiz do repositório. Você pode usar todos os operandos de links relativos, como `./` e `../`.

Os links relativos são mais fáceis para utilizadores que clonam o seu repositório. Os links absolutos podem não funcionar em clones - recomendamos usar links relativos para referir-se a outros ficheiros do seu repositório.

# Imagens

Você pode exibir uma imagem adicionando `!` e colocando o text Alt entre []. O texto alternativo é um texto curto equivalente às informações da Imagem. Em seguida, coloque o link da imagem entre pârenteses ().

>```![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](https://myoctocat.com/assets/images/base-octocat.svg)```

**Output:**

![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](https://myoctocat.com/assets/images/base-octocat.svg)

## Citar Código

Você pode chamar código ou um comando em uma frase com aspas simples. O texto entre as aspas não será formatado.

```md
Use `git status` to list all new or modified files that haven't yet been committed.
```

Use `git status` to list all new or modified files that haven't yet been committed.

Para formatar código ou texto no próprio bloco distinto, use acentos agudos triplos

```md
    Some basic Git Commands are:
    ```git
    git status
    git add
    git commit
    ```
```

**Output:**

Some basic Git Commands are:

```git
git status
git add
git commit
```
