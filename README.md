# 🎮 Pokémon Higher or Lower Game

> Um jogo web responsivo de "Maior ou Menor" baseado em pesos de Pokémon, desenvolvido como projeto de portfólio para consolidação de conceitos avançados de Front-End.

---

## 🚀 Sobre o Projeto

O **Pokémon Higher or Lower** é um jogo de trivia e comparação rápida. O objetivo do jogador é simples: adivinhar se o Pokémon desafiante na tela possui um peso maior ou menor do que o Pokémon de referência. Cada acerto aumenta a sua pontuação (_streak_) e traz um novo desafio.

Este projeto foi construído com foco estrito em boas práticas de engenharia Front-End, sem o uso de frameworks pesados, priorizando o domínio nativo das tecnologias da web.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5:** Marcação semântica (`<main>`, `<article>`, `<section>`, `<dialog>`) e acessibilidade (`ARIA`, navegação por teclado).
- **CSS3:** Diagramação flexível com Flexbox, layout responsivo via Media Queries, posicionamento absoluto/relativo, efeitos de renderização (`filter: drop-shadow()`) e variáveis CSS para suporte a temas.
- **Vanilla JavaScript (ES6+):** Programação assíncrona (`fetch`, `async/await`), manipulação dinâmica do DOM, Delegação de Eventos, gerenciamento de estado global e persistência local (`localStorage`).
- **PokéAPI:** Consumo de endpoints públicos para extração de artes oficiais em alta resolução e dados de espécies.

---

## 📋 Especificações Funcionais e Arquitetura

1. **Arena Principal:**
   - **Card 1 (Referência):** Exibe imagem oficial, peso revelado (kg/lbs) e nome clicável.
   - **Card 2 (Desafiante):** Exibe imagem, nome clicável, peso oculto e botões de ação flutuantes (`↑` Maior / `↓` Menor).
   - **Fluxo de Jogo:** Validação de palpite, incremento de streak, alternância de cartas e gatilho de _Game Over_.

2. **Modais e Recursos Explicativos (Pokédex):**
   - Utilização da tag nativa `<dialog>` para exibição de detalhes e descrições dos Pokémons, com sanitização de texto via Expressões Regulares (Regex)
