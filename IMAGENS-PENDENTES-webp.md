# Imagens pendentes de conversão para .webp — LP Contabilidades

O `index.html` agora referencia **todas as imagens raster como `.webp`**. Os arquivos físicos `.png` e `.jpg` originais continuam dentro de `public/images/` no ZIP — você precisa **gerar versões `.webp` deles com o mesmo nome base** (só trocando a extensão) e salvar na mesma pasta. Pode deletar os `.png`/`.jpg` antigos depois.

## Imagens de seção (`public/images/sections/`)

Originais `.png` → versões `.webp` a gerar:

| Original | Novo nome (a gerar) | Dobra |
|---|---|---|
| `secao-gargalo.png` | `secao-gargalo.webp` | Dobra 3 (Gargalo) |
| `secao-solucao.png` | `secao-solucao.webp` | Dobra 4 (Solução) |
| `secao-faq.png` | `secao-faq.webp` | Dobra 11 (FAQ) |
| `secao-cta-final.png` | `secao-cta-final.webp` | Dobra 12 (CTA Final) |

> Essas 4 fotos são exatamente as imagens com pessoas + shape amarelo que aparecem nas dobras de problema, solução, FAQ e CTA final. As 4 imagens novas que você me enviou no chat parecem se encaixar nesses 4 slots — basta exportar cada uma como `.webp` (com transparência preservada, qualidade ~85) e salvar com o nome correspondente acima.

## Logos (`public/images/logos/`)

Originais `.jpg` → versões `.webp` a gerar:

| Original | Novo nome (a gerar) | Empresa |
|---|---|---|
| `Component 5.jpg` | `Component 5.webp` | SR Eis Contabilidade |
| `Component 6.jpg` | `Component 6.webp` | Capitale |
| `Component 7.jpg` | `Component 7.webp` | Contabilidade Diplomata |
| `Component 9.jpg` | `Component 9.webp` | Assescont |

## OG image

| Nome anterior | Novo nome (a gerar) | Dimensões |
|---|---|---|
| `og-image-contabilidades.jpg` (não existia ainda) | `og-image-contabilidades.webp` | 1200×630 |

## Como converter pra .webp em massa

**Online (mais simples, sem instalar nada):**
- https://squoosh.app (do Google) ou https://convertio.co/png-webp/
- Arrasta os arquivos, qualidade WebP 80–85, baixa.

**No Windows com ImageMagick instalado:**
```bash
cd public/images/sections
for f in *.png; do magick "$f" -quality 85 "${f%.png}.webp"; done
cd ../logos
for f in "Component 5.jpg" "Component 6.jpg" "Component 7.jpg" "Component 9.jpg"; do
  magick "$f" -quality 85 "${f%.jpg}.webp"
done
```

**Validação final:** depois de gerar e colocar os `.webp`, abre o site e confere se nenhuma imagem ficou quebrada. Se quiser, pode deletar os `.png` e `.jpg` antigos do repo pra limpar.
