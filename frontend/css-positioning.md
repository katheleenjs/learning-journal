# CSS Positioning

> Uma forma de controlar a posição dos elementos dentro de uma página.

---

## Sobre

CSS Positioning é um recurso do CSS que permite controlar como um elemento será posicionado na página.

Ele pode ser usado para deixar um elemento na posição normal do layout ou para posicioná-lo de uma forma diferente.

Alguns dos valores mais utilizados são:

- `static`
- `relative`
- `absolute`
- `fixed`
- `sticky`

---

## O que eu entendi

O `position` muda a forma como um elemento se comporta dentro da página.

O valor padrão é o `static`, onde o elemento segue o fluxo normal do documento.

Já outros valores permitem criar situações diferentes, como colocar um elemento sobre outro, deixar algo fixo na tela ou fazer um elemento acompanhar a rolagem.

---

## Principais valores

### position: static

É o comportamento padrão dos elementos.

```css
.elemento {
  position: static;
}
```

Nesse caso, o elemento segue o fluxo normal da página.

---

### position: relative

O elemento continua ocupando seu espaço no layout, mas pode ser deslocado em relação à sua posição original.

```css
.elemento {
  position: relative;
  top: 10px;
  left: 20px;
}
```

Nesse exemplo, o elemento é deslocado para baixo e para a direita.

---

### position: absolute

O elemento pode ser posicionado em relação ao seu elemento de referência mais próximo.

```css
.elemento {
  position: absolute;
  top: 0;
  right: 0;
}
```

Esse tipo de posicionamento pode ser útil quando queremos colocar um elemento em uma posição específica.

Um exemplo comum é um ícone dentro de um campo ou um botão sobre uma imagem.

---

### position: fixed

O elemento fica fixo em relação à janela do navegador.

```css
.elemento {
  position: fixed;
  bottom: 20px;
  right: 20px;
}
```

Mesmo quando a página é rolada, o elemento continua no mesmo lugar da tela.

Pode ser utilizado em elementos como botões de ação ou alguns tipos de navegação.

---

### position: sticky

O elemento começa seguindo o fluxo normal, mas pode ficar preso a uma posição durante a rolagem.

```css
.elemento {
  position: sticky;
  top: 0;
}
```

Um exemplo seria um menu que permanece visível enquanto a pessoa rola determinada parte da página.

---

## top, right, bottom e left

Essas propriedades podem ser utilizadas para indicar o deslocamento de elementos posicionados.

```css
.elemento {
  position: relative;
  top: 10px;
  left: 20px;
}
```

Nesse exemplo:

- `top` movimenta o elemento verticalmente.
- `right` controla a posição em relação à direita.
- `bottom` controla a posição em relação à parte inferior.
- `left` controla a posição em relação à esquerda.

---

## Relative + Absolute

Uma combinação que achei importante entender é utilizar `relative` em um elemento pai e `absolute` em um elemento dentro dele.

Exemplo:

```css
.card {
  position: relative;
}

.botao {
  position: absolute;
  top: 10px;
  right: 10px;
}
```

Nesse caso, o botão pode ser posicionado dentro do card.

Esse tipo de combinação pode ser útil em interfaces, principalmente quando precisamos colocar elementos em posições específicas dentro de um componente.

---

## O que mais me chamou atenção

`position: absolute` não significa simplesmente "colocar em qualquer lugar".

A posição do elemento depende do contexto em que ele está.

Por isso, entender a relação entre o elemento e seu elemento pai é importante.

---

## Como quero aplicar

Quero praticar posicionamento criando pequenos componentes de interface.

Alguns exemplos que quero testar:

- Cards com ícones.
- Botões sobre imagens.
- Badges.
- Menus.
- Elementos fixos na tela.

Também quero praticar junto com Flexbox e Grid para entender quando cada recurso faz mais sentido.

---

## Uma coisa que aprendi

Uma coisa que ficou mais clara para mim é que não preciso usar `position` para organizar tudo na página.

Flexbox e Grid são mais adequados para organizar estruturas e layouts.

O posicionamento pode ser utilizado quando preciso controlar a posição específica de determinados elementos.

---

## Resumindo

- `position` controla como um elemento é posicionado.
- `static` é o comportamento padrão.
- `relative` permite deslocar um elemento mantendo seu espaço no layout.
- `absolute` permite posicionar um elemento em relação ao seu contexto.
- `fixed` mantém um elemento fixo na tela.
- `sticky` pode manter um elemento visível durante a rolagem.
- `top`, `right`, `bottom` e `left` ajudam a controlar o posicionamento.
- `position` pode ser utilizado junto com Flexbox e Grid.

---

## Referências

- MDN Web Docs — CSS position
- W3C — CSS Positioning
