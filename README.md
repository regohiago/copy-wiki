# Wikipédia (clone moderno) — "Blank Space" (1 arquivo HTML)

Clone **estilo Wikipédia** com visual modernizado, feito em **um único arquivo HTML** (HTML + CSS + JavaScript) e com foco em **acessibilidade**.

## ✅ Recursos
- **Um arquivo só**: `index.html`
- **Responsivo**: layout em grid (sidebar + conteúdo) com fallback para mobile
- **Acessibilidade**:
  - Skip link (“Pular para o conteúdo principal”)
  - Landmarks (`header`, `nav`, `main`, `aside`, `footer`)
  - `aria-label`, `aria-selected`, `aria-pressed`, `role="region"`
  - Foco visível (`:focus-visible`)
  - Componentes nativos (ex.: `details/summary` no sumário)
- **Aparência (persistente via localStorage)**:
  - Texto: pequeno / padrão / grande
  - Largura: padrão / largo
  - Tema: automático / claro / escuro (respeita `prefers-color-scheme` no automático)
- **Modo foco**: esconde a sidebar e amplia o conteúdo

## 📦 Estrutura
Como é um arquivo único, não há pastas. O HTML contém:
- **CSS** com tokens (`:root`) e modos de cor
- **JS** para:
  - trocar tema/fonte/largura
  - persistir preferências (`localStorage`)
  - alternar modo foco
  - alternar abas (apenas visual)

## ▶️ Como executar
Opção simples:
1. Salve como `index.html`
2. Abra no navegador (duplo clique)

Opcional (servidor local):
```bash
# Python 3
python -m http.server 8000
# abra: http://localhost:8000