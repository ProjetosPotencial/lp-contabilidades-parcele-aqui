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
2. **OG Image**: criar `og-image-contabilidades.jpg` (1200×630) e publicar no caminho indicado no `<head>`.
3. **Logos da Dobra 7**: confirmar com o time se a lista atual (herdada da B2B) vale para contabilidades ou se há um conjunto específico de logos parceiras de escritórios contábeis.
4. **Revisão jurídica/comercial do FAQ**: as respostas 2 a 6 foram redigidas a partir do PDF de contabilidades (Figma estava vazio/com texto herdado). Validar com Daniel antes de publicar.
5. **URLs externas**: confirmar que `parceleaqui.com.br/sobre-nos`, `/login`, `/simulacao`, `/politica-de-privacidade`, `/termos-de-servico`, `/preciso-de-ajuda` e `/politica-pld` existem para não gerar 404.
6. **Tracking**: adicionar GTM container ID e Meta Pixel ID (se for diferente da B2B).
7. **Tailwind em produção**: o `cdn.tailwindcss.com` é recomendado apenas para desenvolvimento. Em produção, trocar por Tailwind compilado (build step) para melhor performance.

## Notas de manutenção
- Mudanças mobile vivem dentro de `@media (max-width: 767px)` e não devem afetar o desktop.
- A trava `overflow-x: clip/hidden` em html/body previne rolagem horizontal.
- Carrosséis (Impacto, Quem está por trás) e slider do hero inicializados em `initAll()` no fim do arquivo.
- O hero está em modo estático (`data-slider-enabled="false"`) — slides 2 e 3 estão no HTML mas escondidos. Se reativar o slider, **atualizar também o conteúdo dos slides 2 e 3** (continuam com texto da B2B).

## Mapa CTA → mensagem WhatsApp

Todos os CTAs apontam para `https://wa.me/5531973322921`. Prefixo padrão na mensagem: `Olá! Vim da Landing Page Parcele Aqui Negócios e `.

| Botão | Mensagem |
|---|---|
| Quero simular parcelamento / Simule agora / Simular uma operação | `quero fazer uma simulação de parcelamento para o meu negócio.` |
| Ver como funciona no meu negócio | `quero entender como o Parcele Aqui funciona no meu negócio.` |
| Falar com um especialista | `gostaria de falar com um especialista.` |
| Ver exemplos de uso | `gostaria de ver exemplos de uso do Parcele Aqui.` |
| Entender qual modelo escolher | `quero entender qual modelo (whitelabel ou marca Parcele Aqui) faz mais sentido para mim.` |
| Fale com um especialista (FAQ) | `tenho uma dúvida e gostaria de falar com um especialista.` |
