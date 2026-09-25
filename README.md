# Site Azul Kids — protótipo v5

Site institucional + e-commerce da **Azul Kids** (mini veículos elétricos infantis).
Protótipo aprovado, publicado em **https://azulkids-prototipo.netlify.app**.

## Estrutura

```
index.html        → o site completo (HTML + CSS + JS + imagens e fontes embutidas)
docs/BRIEFING.md  → identidade da marca, catálogo, decisões e pendências
netlify.toml      → configuração de publicação (Netlify)
```

O `index.html` é auto-contido: abre em qualquer navegador e publica em qualquer hospedagem estática.

## Onde mexer

Dentro do `index.html`, no bloco `<script>`:

| O quê | Onde |
|---|---|
| Produtos (nome, código, categoria, cores, specs, descrição) | `const MODELS = [...]` |
| Categorias da barra | `const CATS = [...]` |
| Número do WhatsApp, Instagram, SAC | `const SETTINGS = {...}` |
| Exibir preços (quando o Bling alimentar) | `const SHOW_PRICES = false` |
| Pontos de integração (gateway de pagamento e Bling) | `const Integrations = {...}` |

Campos de cada produto prontos para integração: `sku`, `price_pf`, `price_pj`, `bling_id`, `stock`, `ncm`.

## Publicar

Netlify: conectado a este repositório, todo `git push` na branch `main` publica automaticamente.

## Próxima fase

Migração para stack modular (Next.js/Astro + Tailwind + GSAP), autenticação real, pedidos via Bling e gateway (Mercado Pago / Pagar.me). Ver `docs/BRIEFING.md`, seção 7.
