# Travelgram — Página de Perfil de Viagens

Projeto de estudo focado na prática de **CSS Flexbox**, desenvolvido como exercício para consolidar os principais conceitos de layout com `display: flex`.

## Sobre o projeto

O Travelgram é uma página estática que simula o perfil de uma viajante fictícia chamada Isabela Torres. A interface é inspirada em redes sociais de fotos e conta com:

- **Navbar** com logo e menu de navegação
- **Header** com foto de perfil, nome, bio e estatísticas (localização, países visitados e quantidade de fotos)
- **Galeria** com 12 fotos de viagens dispostas em grade
- **Footer** com copyright e links

## Estrutura de arquivos

```
travel-page/
├── index.html
├── assets/
│   ├── icons/          # SVGs (logo, lupa, avião, mapa, imagem)
│   ├── pictures/       # Fotos da galeria (Image 01.png … Image 12.png)
│   └── Profile pic.png
└── styles/
    ├── index.css       # Ponto de entrada — importa todos os outros arquivos CSS
    ├── global.css      # Reset, variáveis CSS (cores, tipografia) e estilos base
    ├── nav.css         # Estilos da barra de navegação
    ├── header.css      # Estilos do cabeçalho de perfil
    ├── main.css        # Estilos da galeria de fotos
    └── footer.css      # Estilos do rodapé
```

## Conceitos de Flexbox aplicados

Cada seção da página exercita um aspecto diferente do Flexbox:

| Seção | Propriedades utilizadas |
|---|---|
| `nav` | `display: flex`, `justify-content: space-between`, `align-items: center` |
| `nav ul` (menu) | `display: flex`, `align-items: center`, `gap` |
| `header .container` | `display: flex`, `justify-content: space-between`, `align-items: center` |
| `#profile` (foto + bio) | `display: flex`, `align-items: center`, `gap` |
| `#info` (estatísticas) | `display: flex`, `flex-direction: column`, `gap` |
| `#info li` | `display: flex`, `align-items: center`, `gap` |
| `main` (galeria) | `display: flex`, `flex-wrap: wrap`, `gap` |
| `footer` | `display: flex`, `gap`, `margin-right: auto` para empurrar itens |

Vale notar o uso de `margin-right: auto` no footer para separar o copyright dos links — uma técnica clássica com Flexbox para criar espaçamento automático entre grupos de itens.

## Tecnologias

- HTML5
- CSS3 (Flexbox, variáveis CSS, `@import`)
- Google Fonts (Poppins)

## Design

A paleta de cores e a tipografia são definidas como variáveis CSS em `global.css`, centralizando os tokens de design:

- **Cor de destaque:** `#EF5F4C` (laranja-avermelhado)
- **Fundo:** `#FFFFFF` / Superfície: `#F5F5F5`
- **Texto primário:** `#313131` / Secundário: `#6C6C6C`
- **Fonte:** Poppins (400 e 700)
