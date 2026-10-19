# Grão & Arte - Torrefação e Café Especial

## Visão Geral e Objetivo
O Grão & Arte é uma aplicação front-end desenvolvida para representar uma marca de torrefação e comercialização de cafés especiais[cite 1, 4]. O objetivo do projeto é oferecer uma interface moderna, semântica, acessível e totalmente responsiva[cite 1], permitindo que apreciadores de cafés naveguem pelos microlotes disponíveis, entendam o processo artesanal de torra e conheçam os planos do clube de assinatura.

Este projeto foi construído para aplicar conceitos de desenvolvimento front-end profissional com foco em arquitetura de código CSS, acessibilidade, semântica HTML e responsividade[cite 1].

---

## Tecnologias e Conceitos Aplicados

- HTML5 Semântico Uso de elementos semânticos (`header`, `main`, `section`, `article`, `details`, `summary`, `footer`) para garantir acessibilidade e estrutura clara[cite 1, 4, 5].
- CSS3 Moderno
  - Metodologia BEM (Block Element Modifier) Padrão rigoroso de nomenclatura de classes HTML e seletores CSS[cite 1].
  - Design System com Custom Properties (Variáveis CSS) Centralização de tokens de cores, fontes, sombras e transições no `root`[cite 3, 6].
  - Escala de Fontes REM e Porcentagem Raiz Unidades relativas para tipografia (`rem`) e ajuste proporcional nos elementos raiz.
  - Flexbox Layout Utilizado para organização de cards e componentes flexíveis[cite 3, 4].
  - Navegação Suave e Compensação do Header Aplicação de `scroll-behavior smooth` com ajuste de recuo para o menu fixo.
  - Microinterações e Transições Pseudo-classes `hover` em botões, cards e links para aprimorar a experiência do usuário[cite 5].
- Responsividade (Media Queries) Estruturação fluida de layout com pontos de quebra (breakpoints) adaptáveis a smartphones, tablets e desktops[cite 2, 3].
- Google Fonts Importação e aplicação das famílias Merriweather (títulos) e Open Sans (corpo de texto)[cite 2, 6, 7].
- Integração Externa (WhatsApp API) Botão flutuante para contato direto configurado com a API do WhatsApp utilizando o número oficial da Escola SENAI Henrique Lupo.

---

## Organização da Arquitetura de Arquivos

A estrutura do projeto segue a separação estrita de responsabilidades organizando o CSS de forma modular[cite 1, 11]

```text
grao-e-arte
├── assets
│   └── images          # Imagens do projeto e recursos visuais
├── css
│   ├── reset.css        # Normalização e reset dos estilos padrão do navegador
│   ├── responsive.css   # Regras de responsividade e media queries
│   ├── style.css        # Estilos principais da aplicação e componentes
│   └── variables.css    # Design system, paleta de cores e tokens CSS
├── index.html           # Estrutura HTML5 da página
└── readme.md            # Documentação do projeto