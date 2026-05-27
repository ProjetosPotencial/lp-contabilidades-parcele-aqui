# LP Parcele Aqui — Contabilidades

Landing page do Parcele Aqui para o segmento de contabilidades. Clone estrutural exato da LP B2B (`lp-b2b-parcele-aqui`), com substituições apenas de texto, alt de imagens, hrefs de CTAs e meta tags. Nenhum atributo de layout (padding, margin, classe, posicionamento, cor) foi modificado. Responsiva (mobile + desktop).

## Stack

- HTML estático + Tailwind (via CDN — ver nota de produção abaixo)
- Fontes: Kufam (headings), DM Sans (body)
- Design System Parcele Aqui aplicado via Tailwind config inline
- Carrosséis e slider em JS vanilla (sem dependências externas)

## Deploy

Sem build step necessário. Servir como conteúdo estático.

### Vercel
```
vercel --prod
```
Configurado em `vercel.json` (sem framework, com headers de segurança e cache de imagens).

### Domínio
Apontar `parceleaqui.com.br/contabilidades` para o deploy (vide canonical no `<head>`).

## Estrutura
- `index.html` — página única (mobile + desktop no mesmo arquivo, responsivo via @media max-width:767px)
- `ALTERACOES.md` — diff dobra a dobra vs LP B2B (texto antigo → novo)
- `IMAGENS-PENDENTES.md` — lista das imagens marcadas com `<!-- TODO: imagem contabilidades -->`
- `robots.txt` — SEO crawlers
- `sitemap.xml` — SEO indexação
- `public/images/` — assets (sections, logos, icons)

## SEO (implementado)
- Title, meta description, keywords, canonical, robots — atualizados para contabilidades
- Open Graph + Twitter Card — atualizados (image `og-image-contabilidades.jpg` ainda **a criar**)
- Schema.org JSON-LD: Organization + Service + WebPage + FAQPage — todos contextualizados para contabilidades

## Origem e relação com a LP B2B

Esta LP é uma variação da LP B2B "Mar Aberto" (`https://github.com/ProjetosPotencial/lp-b2b-parcele-aqui`). Mantém estrutura HTML, CSS e JS idênticos — apenas conteúdo (textos, alt de imagens, hrefs de CTAs e meta tags) foi substituído para o contexto contábil.

⚠️ **Não fazer push para o repositório original `lp-b2b-parcele-aqui`.** Este projeto deve viver em um repositório próprio (a criar).

## PENDÊNCIAS antes de ir ao ar

1. **Imagens de seção**: trocar as 6 imagens marcadas com `<!-- TODO: imagem contabilidades -->` por versões em contexto contábil. Lista completa em `IMAGENS-PENDENTES.md`. Manter os mesmos nomes de arquivo, dimensões e proporções para preservar o layout.
2. **OG Image**: criar `og-image-contabilidades.jpg` (1200×630) e publicar no caminho indicado