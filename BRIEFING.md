# AZUL KIDS — Briefing do Projeto do Site
*Documento-mestre · atualizado em 22/07/2026 · versão do protótipo: v3.3*

## 1. Visão geral

Site institucional + e-commerce da **Azul Kids**, marca de mini veículos elétricos (carros elétricos infantis licenciados, triciclo drift e scooters elétricos 1000W). Estilo visual: **moderno, clean, elegante, referência Apple** — muito branco, produto em destaque, animações suaves de scroll e hover. Público: consumidor final e lojistas (preços só após login).

## 2. Identidade da marca

**Paleta (extraída dos arquivos oficiais):**
- Azul marinho: `#0B2D44` (fundos institucionais, header, footer, painel de specs)
- Azul marinho 2: `#0E3A57` (linhas alternadas do painel)
- Azul principal: `#0073BB` / ícones do header em `#0677BB` (ações, botões, links, hovers)
- Azul claro de apoio: `#DBEBF6`
- Fundo da página: `#F6F9FC` · Cards: branco

**Tipografia:** Montserrat (família completa em TTF disponível; também no Google Fonts).
Hierarquia: ExtraBold/Black para títulos (caixa alta), SemiBold para subtítulos, Regular/Medium para texto, Medium caixa alta com espaçamento para labels.

**Logo:** símbolo de 3 faixas em degrau (azul + faixa central BRANCA + azul — a faixa branca é parte do desenho, nunca remover) + wordmark AZUL (azul) KIDS (branco sobre marinho / marinho sobre branco). No header, o símbolo fica centralizado na barra marinho com as faixas inferiores atravessando a borda e invadindo o branco da página.

**Elemento gráfico:** padrão de "degraus" em outline — usado APENAS no footer, lado direito (decisão de projeto: removido do hero e dos cards).

**Tagline:** "A diversão começa aqui." (o "aqui." em azul)

## 3. Catálogo de produtos (13 modelos)

### Carros elétricos (3-8 anos, 30 kg máx, NCM 95030097)
| Modelo | Cód. | Bateria | Motor | Vel. | Tração | Preço tabela |
|---|---|---|---|---|---|---|
| Range Rover Evoque | ST-FRE99 | 12V 7Ah | 25W | 2-5 km/h | 4x4 | R$ 2.400 |
| UTV Max 12V | ST-KX603 | 12V 10Ah | 35W | 3-5 km/h | 4x4 | R$ 2.400 |
| Mercedes Benz GLC63S | ST-KX608 | 12V 7Ah | 35W | 3-5 km/h | 4x4 | R$ 3.000 |
| UTV Max 24V | ST-KX613 | 24V 7Ah | 45W | 3-5 km/h | 4x4 | R$ 3.000 |
| Lamborghini Poison | ST-KX615 | 12V 10Ah | 45W | 3-5 km/h | 4x4 | R$ 3.400 |
| Clash 24V | ST-D1928 | 2×12V 7Ah | 45W | 3-7 km/h | 4x4 | R$ 3.500 |
| Racing | ST-YA032 | 24V 7Ah | 200W | 3-7 km/h | 4x4 | R$ 3.500 |
| Range Rover HSE | ST-FR999 | 24V 7Ah | 2×200W | 3-7 km/h | 4x2 | R$ 3.500 |
| Toyota Hilux 2019 | ST-FL850 | 12V 10Ah | 35W | 3-5 km/h | 4x4 | R$ 3.700 |
| Can Am Maverick UTV | ST-FA001 | 24V 7Ah | 200W | 3-7 km/h | 4x4 | R$ 4.000 |

### Linha elétrica (NCM 87116000)
| Modelo | Cód. | Bateria | Motor | Vel. | Capacidade | Preço |
|---|---|---|---|---|---|---|
| Triciclo (3 Rodas) | ST-SDP31/B | 36V | 350W | 10-20 km/h | 80 kg (8+ anos) | sob consulta |
| Moto Elétrica 1000W c/ Cesta | VIP-EB0KZ | 48V lítio | 1000W | 35-55 km/h | 150 kg | sob consulta |
| Moto Elétrica 1000W | VIP-E00SL | 60V lítio | 1000W | 45 km/h | 200 kg | sob consulta |

Specs completas (carga, carregador, dimensões na caixa/montado, peso, cores por versão) estão no **catálogo 2026** e na **tabela de preços** (fontes oficiais; tabela de preços = versões vendáveis).

**Cores dos chips (gradientes suaves, amostrados do catálogo):** azul `#0098E1`→preto · verde `#70DA04`→preto · pink `#FF009C`→preto · vermelho→branco · laranja→branco · rosa→branco · amarelo→preto · tricolor preto→`#B80402`→bege `#D29872`.

## 4. Estrutura do site (aprovada no protótipo v3.3)

**Header (fiel ao PDF Menu-Superior):** barra marinho 86px · logo com símbolo saltando abaixo da borda · tagline · ícones azul-claro `#0677BB`: lupa (busca), casinha (home), login, carrinho com badge.

**Busca:** barra branca elegante que desliza abaixo do header, foco automático, busca ao vivo por nome/tipo/código/categoria (ignora acentos), resultados com miniatura → abre a página do modelo.

**Barra de categorias:** pílula branca com os 9 ícones oficiais; hover = "saltada" pra frente com sombra + revela cor + tooltip; clique filtra a grade (com chip "✕ Ver todos os modelos" para limpar).

**Home:** carrossel hero (modelo central grande e colorido, laterais menores em P&B, setas oficiais, auto-play, nome + badges) → grade "Nossos Modelos" (13 cards, foto P&B revelando cor no hover + bolinhas de cores) → frase da marca em reveal → footer.

**Página do modelo (uma por produto, template do PDF do Can Am):** abinha "✕ Todos os modelos" · ícone da categoria no canto · nome + badges + COMPRAR · foto grande com setas navegando entre modelos · card CORES (chips com gradiente e nome) · DESCRIÇÃO (Can Am = texto real; demais = fictícios provisórios) · painel de specs idêntico ao catálogo (card azul: medalha + diferenciais + tração + NCM; dois grupos de linhas marinho com ícone azul em cada linha) · segundo COMPRAR · reveals estilo Apple no scroll.

**Compra:** botão COMPRAR (pílula azul) que se transforma em seletor de quantidade [− n +] em marinho; carrinho soma por modelo. Abaixo do botão: cadeado oficial + "Faça login / para ver o / preço" (3 linhas, fiel ao PDF Login-preços). **Preços nunca aparecem sem login.**

**Footer (fiel ao PDF Menu-inferior):** cantos superiores arredondados, links Contato/Rede Social/SAC com ícones oficiais (sem ação por enquanto), logo à direita, padrão de degraus só no lado direito, barra final com selo + "Todos os direitos reservados a AzulKids".

## 5. Decisões registradas

1. Preços só após login (site atende consumidor e lojista).
2. Seletor de cores por enquanto é indicativo (sem trocar foto) — fotos por cor virão depois.
3. Descrições dos modelos (exceto Can Am) são fictícias, aguardando textos oficiais.
4. WhatsApp/Instagram/SAC sem links reais por enquanto.
5. Marca d'água/padrão gráfico apenas no footer.
6. Sem "Catálogo 2026" no hero.
7. Protótipo em arquivo único HTML; site final será modular no Claude Code.

## 6. Pendências (o que falta receber/decidir)

- [ ] Fotos PNG transparentes de cada variação de cor de cada modelo
- [ ] Descrições oficiais dos 12 modelos restantes
- [ ] Preços de Triciclo e Motos 1000W (ou confirmar "sob consulta")
- [ ] Número do WhatsApp, @ do Instagram, canal de SAC
- [ ] Definição do fluxo de login/cadastro e checkout (design ou aprovação de proposta)
- [ ] Domínio, hospedagem e meio de pagamento (fase final)
- [ ] Dados de rodapé: CNPJ/cidade (se desejar exibir)

## 7. Próxima fase — desenvolvimento real

Migrar o protótipo aprovado para o **Claude Code** com stack: **Next.js (ou Astro) + Tailwind CSS + GSAP/ScrollTrigger + Lenis**, estrutura modular (um arquivo por seção; dados dos produtos em JSON central; design tokens da marca centralizados). Depois: autenticação (preços pós-login), carrinho/checkout com gateway (Mercado Pago/Pagar.me), deploy.

## 8. Arquivos-fonte do projeto

| Arquivo | Conteúdo |
|---|---|
| LOGOS-AZUL-KIDS.pdf | Logos positivo/negativo + padrão gráfico |
| Menu-Superior.pdf / Menu-inferior.pdf | Header e footer oficiais |
| Í_CONES.pdf | 9 ícones de categorias + home/user/carrinho/setas |
| CARACTERISTICAS.pdf | Painel de specs + 12 ícones das linhas |
| Login-prec_os.pdf | Bloco COMPRAR + cadeado + texto de login |
| AZULKIDS-Cata_logo-2026-ATT.pdf | Specs completas dos 13 modelos |
| AZULKIDS-Tabela-de-Precos.pdf | Preços e versões de cores vendáveis |
| LAYOUT-PA_GINAS-AZULKIDS.pdf | Layout: Home, Nossos Modelos, página de produto |
| Montserrat-*.ttf (18 arquivos) | Família tipográfica completa |
| 13 PNGs transparentes (freepik/magnific) | Fotos oficiais dos produtos |
| magnifying-glass_12080183.svg | Ícone da lupa |
| azulkids-prototipo-v3-3.html | **Protótipo aprovado (estado atual)** |
