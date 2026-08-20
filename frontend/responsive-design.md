# Responsive Design

> Uma forma de criar interfaces que se adaptam a diferentes tamanhos de tela.

---

## Sobre

Responsive Design, ou Design Responsivo, é uma forma de desenvolver interfaces que conseguem se adaptar a diferentes dispositivos e tamanhos de tela.

Uma mesma página pode ser acessada pelo celular, tablet ou computador, e o layout precisa continuar funcionando bem nesses diferentes contextos.

---

## O que eu entendi

É necessário pensar em como os elementos vão se reorganizar de acordo com o espaço disponível.

Por exemplo, uma estrutura que possui várias colunas no computador pode precisar ser reorganizada em uma ou duas colunas no celular.

---

## O que mais me chamou atenção

Não é interessante criar primeiro uma versão para computador e só depois tentar adaptar tudo para o celular.

É melhor considerar os diferentes tamanhos de tela durante o desenvolvimento.

---

## Principais conceitos

### Media Queries

Media Queries permitem aplicar diferentes estilos dependendo das características da tela.

Um exemplo simples:

```css
@media (max-width: 768px) {
  .container {
    grid-template-columns: 1fr;
  }
}
```

Nesse exemplo, quando a tela tiver até 768px de largura, o elemento passa a ter apenas uma coluna.

---

### Breakpoints

Breakpoints são pontos em que o layout pode mudar para se adaptar a outro tamanho de tela.

Por exemplo:

- Celular
- Tablet
- Desktop

Não existe necessariamente um único conjunto obrigatório de breakpoints. Eles devem fazer sentido de acordo com o conteúdo e com o layout.

---

### Mobile First

Mobile First é uma abordagem em que começamos pensando primeiro na versão para telas menores.

Depois, podemos adicionar mudanças para telas maiores.

Um exemplo:

```css
.container {
  display: grid;
  grid-template-columns: 1fr;
}

@media (min-width: 768px) {
  .container {
    grid-template-columns: 1fr 1fr;
  }
}
```

Nesse caso, começamos com uma coluna e depois adicionamos uma segunda coluna para telas maiores.

---

### Unidades relativas

Unidades como `%`, `rem`, `em`, `vw` e `vh` podem ajudar na criação de layouts mais flexíveis.

Por exemplo:

```css
.container {
  width: 90%;
}
```

Nesse caso, a largura do elemento pode acompanhar o tamanho disponível na tela.

---

## Responsive Design e CSS Grid

O Grid pode ser combinado com Responsive Design para criar layouts que se reorganizam conforme o espaço disponível.

Por exemplo:

```css
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 16px;
}

@media (max-width: 768px) {
  .container {
    grid-template-columns: 1fr;
  }
}
```

No desktop, temos três colunas.

Em uma tela menor, os elementos passam a ocupar uma coluna.

---

## Responsive Design e Flexbox

O Flexbox também pode ajudar na criação de layouts responsivos.

Podemos, por exemplo, alterar a direção dos elementos dependendo do tamanho da tela.

```css
.container {
  display: flex;
  flex-direction: row;
}

@media (max-width: 768px) {
  .container {
    flex-direction: column;
  }
}
```

Nesse caso, os elementos ficam em uma linha em telas maiores e passam para uma coluna em telas menores.

---

## Resumindo

- Responsive Design permite que uma interface se adapte a diferentes tamanhos de tela.
- O layout pode mudar de acordo com o espaço disponível.
- Media Queries ajudam a aplicar estilos diferentes.
- Breakpoints indicam momentos em que o layout pode mudar.
- Mobile First começa pensando primeiro em telas menores.
- Grid e Flexbox podem ser utilizados para criar layouts responsivos.
- É importante testar a interface em diferentes tamanhos de tela.

---

## Referências

- MDN Web Docs
- W3C
- Material Design
