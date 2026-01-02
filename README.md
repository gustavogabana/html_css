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
