# CSS Grid

> Uma ferramenta do CSS que ajuda a organizar elementos em linhas e colunas.

---

## Sobre

CSS Grid é um sistema de layout do CSS usado para organizar elementos em linhas e colunas.

Ele facilita a criação de estruturas mais complexas, permitindo controlar o tamanho e o posicionamento dos elementos dentro de uma área.

Assim como o Flexbox, o Grid ajuda na criação de layouts responsivos.

---

## O que eu entendi

Depois de estudar Flexbox, percebi que o CSS Grid funciona de uma forma um pouco diferente.

Enquanto o Flexbox costuma ser muito útil para organizar elementos em uma direção, como uma linha ou uma coluna, o Grid permite trabalhar com linhas e colunas ao mesmo tempo.

Isso faz com que ele seja bastante útil para estruturar páginas e layouts maiores.

---

## O que mais me chamou atenção

Flexbox e Grid não precisam competir entre si.

Eles podem ser utilizados juntos.

Por exemplo, o Grid pode organizar a estrutura principal de uma página enquanto o Flexbox pode organizar os elementos dentro de um componente.

---

## Como quero aplicar

Quero praticar Grid criando diferentes tipos de layouts para entender melhor como as linhas, colunas e espaços funcionam.

Também quero aprender a escolher entre Grid e Flexbox dependendo do problema que preciso resolver, em vez de utilizar sempre a mesma ferramenta.

---

## Principais conceitos

### `display: grid`

Ativa o CSS Grid em um elemento.

```css
.container {
  display: grid;
}
```

### `grid-template-columns`

Define as colunas do layout.

Exemplo:

```css
.container {
  grid-template-columns: 1fr 1fr;
}
```

Nesse exemplo, são criadas duas colunas com o mesmo tamanho.

### `grid-template-rows`

Define as linhas do layout.

Exemplo:

```css
.container {
  grid-template-rows: 100px 200px;
}
```

Nesse caso, são criadas duas linhas com alturas diferentes.

### `gap`

Define o espaço entre as linhas e colunas.

Exemplo:

```css
.container {
  gap: 16px;
}
```

### `grid-column`

Permite definir em quais colunas um elemento será posicionado.

Exemplo:

```css
.item {
  grid-column: 1 / 3;
}
```

Nesse exemplo, o elemento ocupa duas colunas.

### `grid-row`

Permite definir em quais linhas um elemento será posicionado.

Exemplo:

```css
.item {
  grid-row: 1 / 3;
}
```

---

## Grid x Flexbox

### Flexbox

É bastante útil quando quero organizar elementos principalmente em uma direção.

Exemplos:

- Menus
- Botões
- Itens de uma lista
- Elementos dentro de um card
- Barras de navegação

### Grid

É útil quando preciso trabalhar com linhas e colunas.

Exemplos:

- Galerias
- Layouts de páginas
- Grades de cards
- Estruturas mais complexas

---

## Um exemplo simples

### HTML

```html
<div class="container">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
  <div>Item 4</div>
</div>
```

### CSS

```css
.container {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 16px;
}
```

Nesse exemplo, os quatro elementos serão organizados em duas colunas.

---

## Resumindo

- CSS Grid organiza elementos em linhas e colunas.
- É muito útil para criar layouts mais estruturados.
- Pode ser utilizado junto com Flexbox.
- `grid-template-columns` e `grid-template-rows` ajudam a definir a estrutura.
- `gap` controla o espaço entre os elementos.
- É importante entender quando utilizar Grid e quando utilizar Flexbox.

---

## Referências

- MDN Web Docs
- CSS-Tricks
- Material de estudos
