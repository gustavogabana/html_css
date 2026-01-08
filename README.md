# HTML 5 e CSS 3

HTML é uma linguagem de marcação e CSS é uma linguagem de estilização feita para estilizar páginas em HTML.

## URL

```bash
www.github.com/gustavoguanabara
```

Uniform Resource Locator: Serve para enviar e buscar dados para um endereço DNS/IP exato.
A URL é feita de partes:
    - Dominio: Em <www.github.com> o github é o domínio. É a identidade e marca única do site.
    - Sub-dominio: É o que vem antes do domínio. Por exemplo, www é o subdomain principal. Um site    pode ter vários subdomains.
    - TLD: Dentro do domínio, tem o .com. Esse .com é o TLD (Top Level Dmain).
    - GTLD: É o TLD, porém genérico, algum nome fora dos escopos comuns.
    - CCTLD: CC significa country code, por exemplo: .com.br, .com.it, .com.pt, etc.
    - Caminho/rota: É o que vem depois da / na URL. É definida pelo site/software.

## Exemplo de display flex para justificar (linha) e alinhar (altura)

```css
button {
    display: flex;
    justify-content: center; /* Centraliza horizontalmente */
    align-items: center;     /* Centraliza verticalmente */
    height: 50px;
}
```

## Text align vs display flex

Text align mexe no fluxo do texto, enquanto o display flex mexe na estrutura da caixa do elemento.

## Box-shadow

```css
/* box-shadow: [eixo X] [eixo Y] [desfoque] [espalhamento] [cor];*/
.meu-elemento {
    box-shadow: 
        2px   /* Desloca a sombra 2px para a DIREITA */
        2px   /* Desloca a sombra 2px para BAIXO */
        7px   /* Blur (desfoque): deixa a borda da sombra suave/esfumaçada */
        7px   /* Spread (espalhamento): aumenta o tamanho da sombra em todas as direções */
        black; /* Cor da sombra */
}
```

## Variaveis no CSS

```css
:root {
    /* Definição das cores e tamanhos padrão */
    --cor-primaria: #2980b9;
    --largura-sidebar: 250px;
    --tamanho-fonte: 16px;
}

.sidebar {
    width: var(--largura-sidebar);
    background-color: var(--cor-primaria);
}
```

## Responseividade no CSS

```css
:root {
    --largura-sidebar: 250px;
    --padding-container: 40px;
}

/* Quando a tela for menor que 768px (Tablet/Celular) */
@media (max-width: 768px) {
    :root {
        --largura-sidebar: 80px; /* A sidebar encolhe automaticamente */
        --padding-container: 15px; /* Os espaços internos diminuem */
    }
}

.sidebar {
    width: var(--largura-sidebar);
    transition: width 0.3s; /* Animação suave na mudança */
}
```

## FlexBox

É focado em um eixo por vez (vertizal ou horizontal). Ideal para alinhar itens dentro de um container.

 ```css
 .menu {
    display: flex;
    justify-content: space-between; /* Espaça os itens igualmente */
    align-items: center;            /* Centraliza na vertical */
}
```

### Eixos

Main axis é de cima pra baixo, Cross Axis é da esquerda para direita, na configuração de display:flex normal (flex-direction: row;).

Na configuração reverse-row, inverte o main axis espelhado, o cross mantém.

No flex-direction: column;, o mais axis se torna vertical, de cima para baixo, e o cross-axis se torna horizontal, da esquerda para direita.

No reverse-column, inverte o main axis espelhado.
