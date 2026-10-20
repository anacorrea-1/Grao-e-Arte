# Grão & Arte - Torrefação e Café Especial

## 1. Visão Geral e Objetivo do Projeto
O **Grão & Arte** é uma aplicação web front-end desenvolvida para representar uma marca de torrefação artesanal e comercialização de cafés especiais. O projeto foi construído para simular um ambiente de desenvolvimento profissional, atendendo aos requisitos funcionais e não funcionais estabelecidos para a Turma A.

O objetivo principal da aplicação é proporcionar uma experiência moderna, elegante e intuitiva para entusiastas de café especial, permitindo a navegação pelos microlotes disponíveis, apresentação do processo de torra, contratação de planos do clube de assinatura, esclarecimento de dúvidas frequentes (FAQ) e contato direto via API do WhatsApp.

---

## 2. Tecnologias e Conceitos Aplicados

### **HTML5 Semântico e Acessibilidade**
* **Estrutura Clara:** Utilização rigorosa das tags semânticas (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<details>`, `<summary>`, `<footer>`, `<address>`).
* **Navegação Suave e FAQ Interativo:** Implementação da seção de dúvidas com elementos nativos `<details>` e `<summary>`, além de links internos para rolagem fluida.

### **CSS3, Arquitetura e Design System**
* **Metodologia BEM (Block Element Modifier):** Padrão rigoroso de nomenclatura de classes HTML e seletores CSS (`.brand-card`, `.brand-card__image`, `.brand-card__title`) garantindo modularidade e reuso.
* **Separação Estrita de Responsabilidades:** Organização modular do CSS em arquivos distintos (`variables.css`, `reset.css`, `style.css`, `responsive.css`) sem inline styles ou blocos `<style>`.
* **Design System com Custom Properties (`:root`):** Centralização de tokens de cores, paleta do café artesanal, tipografia, sombras (`--shadow-card`, `--shadow-hover`), raios de borda e tempos de transição.
* **Escala Base em REM (62.5%):** Ajuste proporcional no elemento raiz (`html { font-size: 62.5%; }`), fazendo com que `1rem = 10px` e mantendo a tipografia e os espaçamentos dinâmicos e acessíveis.
* **Google Fonts:** Importação e aplicação das famílias tipográficas **Merriweather** (pesos 400 e 700 para títulos) e **Open Sans** (pesos 400, 600 e 700 para corpo de texto).

### **Layout e Responsividade**
* **Flexbox & CSS Grid:** Utilização de CSS Grid na seção de catálogo (`.brands__grid`) e Flexbox no cabeçalho, cards de assinatura e rodapé.
* **Posicionamento Fixo e Compensação:** Cabeçalho (`.header`) e rodapé (`.footer`) fixados na tela (`position: fixed`), com tratamento de compensação do recuo de rolagem (`scroll-margin-top`).
* **Botão Flutuante do WhatsApp:** Ícone fixado no canto inferior da tela (`position: fixed`), integrado diretamente à API do WhatsApp com o número oficial da Escola SENAI Henrique Lupo (`551633033800`).
* **Media Queries (Adaptabilidade):** Regras de responsividade configuradas em `responsive.css` ajustando o layout para telas de smartphones e tablets.

---

## 3. Arquitetura de Arquivos

O repositório está estruturado com a separação clara de responsabilidades:

```text
grao-e-arte/
├── css/
│   ├── reset.css        # Reset de estilos globais e configuração do rem (62.5%)
│   ├── responsive.css   # Regras de responsividade e media queries para dispositivos móveis
│   ├── style.css        # Estilos gerais da aplicação, componentes e seções
│   └── variables.css    # Design System, variáveis globais (:root) e tokens de design
├── src/
│   └── img/             # Imagens locais do projeto e botões de mídia
├── index.html           # Estrutura principal da aplicação em HTML5 semântico
└── README.md            # Documentação técnica completa do projeto
```