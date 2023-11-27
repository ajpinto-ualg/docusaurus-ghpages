---
sidebar_position: 5
---

# Sintaxe Markdown Extendida

A sintaxe básica do Markdown adicionou muitos dos elementos necessários no dia a dia, mas não foi suficiente para algumas pessoas. É aí que entra a sintaxe estendida.

Vários indivíduos e organizações se encarregaram de estender a sintaxe básica, adicionando elementos adicionais como tabelas, blocos de código, realce de sintaxe, auto-link de URL e notas de rodapé. Esses elementos podem ser ativados usando uma linguagem de marcação leve que se baseia na sintaxe básica do Markdown ou adicionando uma extensão a um processador Markdown compatível.

## Suporte

Nem todos os aplicativos Markdown suportam elementos de sintaxe estendida. Você precisará verificar se a linguagem de marcação leve que seu aplicativo está usando suporta os elementos de sintaxe estendida que deseja usar. Se não for, ainda pode ser possível habilitar extensões em seu processador Markdown.

## Linguagens de Marcação

Existem várias linguagens de marcação leve que são superconjuntos do Markdown. Eles incluem a sintaxe básica e a constroem adicionando elementos adicionais como tabelas, blocos de código, realce de sintaxe, auto-link de URL e notas de rodapé. Muitos dos aplicativos Markdown mais populares usam uma das seguintes linguagens de marcação leve:

- CommonMark
- GitHub Flavored Markdown
- Markdown Extra
- MultiMarkdown

## Processadores de Markdown

Existem dezenas de processadores Markdown disponíveis. Muitos deles permitem que você adicione extensões que ativam elementos de sintaxe estendida. Verifique a documentação do seu processador para obter mais informações.

## Tabelas

Para adicionar uma tabela, use três ou mais hifens ( ---) para criar o cabeçalho de cada coluna e use pipes ( |) para separar cada coluna. Por compatibilidade, você também deve adicionar um pipe em cada extremidade da linha.

```md
| Sintaxe | Descrição |
| ----------- | ----------- |
| Cabeçalho | Título |
| Parágrafo | Texto |
```

As larguras das células podem variar, conforme mostrado abaixo. A saída renderizada ficará igual.

| Sintaxe | Descrição |
| --- | ----------- |
| Cabeçalho | Título |
| Parágrafo | Texto |

> **Dica:** Criar tabelas com hifens e pipes pode ser tedioso. Para acelerar o processo, experimente usar o Gerador de Tabelas Markdown ou o AnyWayData Markdown Export. Construa uma tabela usando a interface gráfica e copie o texto formatado em Markdown gerado para o seu arquivo.

Você pode alinhar o texto nas colunas à esquerda, direita ou centro adicionando dois pontos (:) à esquerda, direita ou em ambos os lados dos hifens na linha do cabeçalho.

```md
| Sintaxe | Descrição | Texto de teste |
| :--- | :----: | ---: |
| Cabeçalho | Título | Aqui está isso |
| Parágrafo | Texto | E mais |
```

| Sintaxe | Descrição | Texto de teste |
| :--- | :----: | ---: |
| Cabeçalho | Título | Aqui está isso |
| Parágrafo | Texto | E mais |

Você pode formatar o texto dentro das tabelas. Por exemplo, você pode adicionar links, código (palavras ou frases entre acentos agudos ( `) apenas, não blocos de código) e ênfase.

Você não pode usar cabeçalhos, blocos de citação, listas, regras horizontais, imagens ou a maioria das tags HTML.

Dica: Você pode usar HTML para criar quebras de linha e adicionar listas dentro das células da tabela.

Você pode exibir um caractere pipe ( |) em uma tabela usando seu código de caractere HTML ( | ).

## Listas de tarefas

As listas de tarefas permitem que você crie uma lista de itens com caixas de seleção que podem ser marcadas como concluídas ou não. Este recurso é útil para acompanhar o progresso de um projeto ou uma lista de verificação. Para criar uma lista de tarefas, use um hífen e um par de colchetes com um espaço ( [ ]) na frente dos itens da lista. Para marcar uma caixa de seleção como concluída, use um x entre os colchetes ( [x] ).

```md
- [x] Terminar o relatório
- [ ] Revisar o relatório
- [ ] Enviar o relatório
```

O resultado renderizado fica assim:

- [x] Terminar o relatório
- [ ] Revisar o relatório
- [ ] Enviar o relatório

> **Dica:** As listas de tarefas só serão renderizadas corretamente no GitHub.

## Usar emojis

É possivel adicionar um emoji à escrita digitando :EMOJICODE:.

>``` @octocat :+1: This PR looks great - it's ready to merge! :shipit: ```

**Output:**

@octocat :+1: This PR looks great - it's ready to merge! :shipit:

## Alertas

Os alertas são uma extensão da sintaxe *blockquote* que pode ser usada para dar ênfase a informações críticas. No GitHub, os alertas são exibidos com cores e ícones distintos para indicar a importância do conteúdo.

Há 3 tipos de alertas disponivéis. Pode-se adicionar um alerta com uma linha de *blockquote* especial que indica o tipo de alerta e, em seguida, adicionar as informações de alerta num *blockquote* standard imediatamente depois.

```md
> [!NOTE]
> Highlights information that users should take into account, even when skimming

> [!IMPORTANT]
> Crucial information necessary for users to succeed.

> [!WARNING]
> Critical content demanding immediate user attention due to potential risks.
```

**Output:**

> [!NOTE]
> Highlights information that users should take into account, even when skimming

> [!IMPORTANT]
> Crucial information necessary for users to succeed.

> [!WARNING]
> Critical content demanding immediate user attention due to potential risks.

## Notas de rodapé

Pode-se adicionar notas de rodapé ao conteúdo usando a seguinte sintaxe:

```md
Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].

[^1]: My reference.
[^2]: To add line breaks within a footnote, prefix new lines with 2 spaces.
  This is a second line.
```

A nota de rodapé será interpretada da seguinte forma:

Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].


[^1]: My reference.
[^2]: To add line breaks within a footnote, prefix new lines with 2 spaces.
  This is a second line.
