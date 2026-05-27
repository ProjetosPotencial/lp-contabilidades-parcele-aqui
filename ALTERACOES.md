# LP Parcele Aqui — Contabilidades

Clone estrutural exato da LP B2B (`lp-b2b-parcele-aqui`), com substituições apenas de texto, alt de imagens, hrefs de CTAs e meta tags. Nenhum atributo de layout (padding, margin, classe, posicionamento, cor) foi modificado.

---

## SEO / Meta / OG / Schema (head)

- `<title>`: `Parcele Aqui B2B | Destrave negociações B2B com parcelamento no cartão` → `Parcele Aqui para Contabilidades — Parcele tributos, encargos e honorários em até 12x`
- `meta description`: atualizada para foco em tributos, DAS, encargos e honorários, com boleto liquidado à vista para o emissor.
- `meta keywords`: trocada para termos de contabilidade (parcelamento tributos, DAS, honorários contábeis, encargos trabalhistas, escritório contábil etc).
- `canonical` / `og:url`: `/b2b` → `/contabilidades`
- `og:image`: `og-image-b2b.jpg` → `og-image-contabilidades.jpg` (asset a criar)
- `og:title`, `og:description`, `og:image:alt`: atualizados para contabilidades
- `twitter:title`, `twitter:description`, `twitter:image`: atualizados
- JSON-LD: `Service`, `WebPage` e `FAQPage` reescritos para o contexto contábil (6 perguntas/respostas batem com o FAQ visível).

---

## Dobra 1 — HERO

| Campo | Antes (B2B) | Agora (Contabilidades) |
|---|---|---|
| Kicker (full) | Parcelamento B2B sem risco para sua empresa | Como destravar negócios contábeis |
| Kicker (short) | Parcelamento B2B sem risco | Como destravar negócios |
| H1 | **Destrave negociações B2B com parcelamento** no cartão e receba à vista, sem inadimplência | Parcelamento inteligente para **tributos, boletos e honorários** |
| Subtítulo | Seus clientes parcelam em até 12x. / Sua empresa recebe à vista e sem risco. | Seus clientes parcelam em até 12x no cartão. / O boleto é liquidado à vista para o emissor. |
| Bullet 1 | Sua empresa recebe à vista | Tributos, DAS, encargos e honorários em até 12x |
| Bullet 2 | Zero risco de inadimplência | Até 3 cartões de crédito na mesma operação |
| Bullet 3 | Ativação rápida e 100% digital | Boleto liquidado à vista, com segurança e sem risco |
| Botão primário | "Ver como funciona no meu negócio" (msg: como funciona) | **"Quero simular parcelamento"** (msg: simulação) |
| Botão secundário | Falar com um especialista (msg: contato) | Falar com um especialista (msg: contato) — mantido |
| Imagem | `hero-slide-1.webp` | Mantida com TODO de troca + alt atualizado |

> ⚠️ A LP herda o slider de 3 slides do B2B em modo estático (apenas slide 0 visível). Os slides 2 e 3 não foram atualizados porque estão desabilitados (`data-slider-enabled="false"`) — mantidos para não alterar o JS / estrutura, mas devem ser reescritos se o slider for reativado.

---

## Dobra 2 — Infraestrutura / Tecnologia

| Campo | Antes | Agora |
|---|---|---|
| Kicker | Infraestrutura financeira confiável | Tecnologia e confiança |
| H2 | Infraestrutura sólida / **para operações financeiras B2B** | Prova de credibilidade que / **sustenta cada transação** |
| Subtítulo | Desenvolvido pela Potencial Tecnologia… / Infraestrutura certificada, segura e com liquidação à vista para o emissor. | Uma solução **desenvolvida para operar com segurança**, escala e estabilidade / no mercado financeiro e contábil. |
| Card 1 | Liquidação à vista e sem risco | **Fintech brasileira** — Solução desenvolvida no Brasil, alinhada às regras, tributos e rotinas do mercado contábil. |
| Card 2 | Infraestrutura certificada e escalável | **+25 anos de tecnologia** — Mais de duas décadas criando soluções financeiras robustas e escaláveis. |
| Card 3 | Plataforma 100% digital e automatizada | **Infraestrutura certificada** — Padrões rigorosos de proteção de dados, conformidade e operação contínua. |
| Card 4 | Fintech brasileira especializada em B2B | **Transações aprovadas com confiabilidade** — Integração com as principais adquirentes do mercado para liquidação em tempo real e alta taxa de aprovação. |

---

## Dobra 3 — Gargalo

| Campo | Antes | Agora |
|---|---|---|
| Kicker | O gargalo está no pagamento | O desafio da rotina contábil |
| H2 | O que realmente trava **negociações no B2B** | A falta de caixa trava **a regularização das empresas** |
| Subtítulo | O problema raramente é falta de interesse… | Tributos acumulados, encargos elevados e honorários em atraso aumentam a inadimplência e prejudicam a saúde financeira das empresas. |
| Bullet 1 | Vendas que não avançam | Multas, juros e bloqueios de CNPJ |
| Bullet 2 | Ciclo de fechamento mais longo | Inadimplência de honorários do escritório |
| Bullet 3 | Risco ao oferecer parcelamento próprio | Falta de previsibilidade financeira |
| Texto final | E assumir parcelamento internamente gera risco… | E sem fôlego de caixa, o cliente posterga obrigações e o escritório sofre o impacto na recorrência. |
| CTA | "Entender se faz sentido para minha empresa" (msg: entender) | **"Simular uma operação"** (msg: simulação). Texto mobile: "Simular agora". |
| Imagem | `secao-gargalo.png` | Mantida com TODO + alt atualizado |

---

## Dobra 4 — Solução

| Campo | Antes | Agora |
|---|---|---|
| Kicker | Solução Parcele Aqui | Nova dinâmica de pagamento |
| H2 | Pagamento não / pode ser o motivo de / **um negócio não fechar.** | Seu cliente parcela. / **O boleto é liquidado / à vista.** |
| Subtítulo | Permita que seus **clientes parcelem no cartão** enquanto sua empresa recebe à vista… | Com o Parcele Aqui, o cliente ganha **fôlego financeiro ao parcelar no cartão**, enquanto o emissor do boleto recebe à vista… |
| Bullet 1 | Redução do ciclo de vendas | Jornada 100% digital, simples e segura |
| Bullet 2 | Aumento da taxa de conversão | Regularização imediata para o cliente |
| Bullet 3 | Preservação total do caixa | Recebimento à vista para o emissor |
| Bullet 4 | Zero inadimplência para sua empresa | Zero risco de inadimplência para o escritório |
| CTA | "Simular uma operação" (msg: simulação) | **"Ver como funciona no meu negócio"** (msg: como funciona) |
| Imagem | `secao-solucao.png` | Mantida com TODO + alt atualizado |

---

## Dobra 5 — Como Funciona

H2 e estrutura visual (vinheta + card 4 passos) **mantidos**. Apenas os 4 passos foram trocados (desktop **e** mobile):

| Passo | Antes | Agora |
|---|---|---|
| 01 | Sua empresa emite o boleto normalmente | O cliente recebe o boleto ou obrigação |
| 02 | O cliente escolhe parcelar com o Parcele Aqui | O escritório envia o link do Parcele Aqui |
| 03 | O cliente escolhe as parcelas e paga no cartão | O cliente escolhe as parcelas e paga no cartão (mantido) |
| 04 | Boleto liquidado à vista para sua empresa | O boleto é liquidado à vista para o emissor |

Imagens `secao-como-funciona.webp` e `secao-como-funciona-mobile.webp`: mantidas com TODO.

---

## Dobra 6 — Obrigações (Impacto)

Header atualizado:

| Campo | Antes | Agora |
|---|---|---|
| Kicker | Impacto real no B2B | Flexibilidade para o cliente |
| H2 | Onde o Parcele Aqui gera / **impacto real no seu negócio** | As principais obrigações do / **dia a dia empresarial** |
| Subtítulo | O Parcele Aqui **se adapta às necessidades reais da sua empresa.** | O Parcele Aqui **se adapta às necessidades reais das empresas** atendidas pelo seu escritório. |

6 cards reescritos (desktop **e** carrossel mobile):

| # | Antes | Agora |
|---|---|---|
| 1 | Mais conversão de vendas | **Tributos federais, estaduais e municipais** — Facilite o pagamento de impostos recorrentes e evite multas, juros e bloqueios… |
| 2 | Redução do tempo de fechamento | **DAS e guias do MEI** — Regularize pendências do Simples Nacional e do MEI sem comprometer o fluxo de caixa do cliente. |
| 3 | Aumento do ticket médio | **Encargos trabalhistas** — Dilua custos da folha e obrigações legais, reduzindo riscos de atraso e passivos trabalhistas. |
| 4 | Zero risco de inadimplência | **Boletos atrasados** — Permita a quitação de débitos em atraso, evitando protestos, negativação e restrições fiscais. |
| 5 | Operação simples e escalável | **Honorários contábeis** — Facilite o pagamento dos honorários e aumente a recorrência, sem gerar atrito na relação com o cliente. |
| 6 | Mais valor percebido pelo cliente | **Taxas e obrigações recorrentes** — Resolva despesas operacionais e obrigações periódicas que impactam a saúde financeira da empresa. |

CTA central: "Ver exemplos de uso" (msg: ver exemplos) — **mantido**.

---

## Dobra 7 — Empresas / Logos

| Campo | Antes | Agora |
|---|---|---|
| Kicker | Empresas que já utilizam | Quem já confia |
| H2 | Presente em empresas que utilizam / **o parcelamento como estratégia de fechamento** | Contabilidades e parceiros / **que já operam com o Parcele Aqui** |
| Subtítulo | (texto B2B) | Empresas que utilizam o Parcele Aqui para destravar negociações e acelerar fechamentos, com operações processadas pela adquirência **Cielo**, garantindo segurança, confiabilidade e liquidação à vista para o emissor. |

> Grid de logos: **mantido idêntico** ao da B2B (mesmos arquivos, posições e dimensões). Time deve confirmar se as logos atuais cabem nesta LP — vide ponto de atenção #2.

---

## Dobra 8 — Modelos (Whitelabel vs Marca)

| Campo | Antes | Agora |
|---|---|---|
| Kicker | Flexibilidade para o seu modelo de negócio | Escolha estratégica |
| H2 | Você escolhe como / **operar com o Parcele Aqui** | Você escolhe como operar: / **com a sua marca ou com a marca Parcele Aqui.** |
| Subtítulo | (texto B2B) | O mesmo produto, **a mesma segurança e eficiência**, no formato que melhor fortalece o posicionamento do seu escritório. |
| Modelo 1 título | Com a sua marca (Whitelabel) | Com a sua marca (Whitelabel) — mantido |
| Modelo 1 bullets | O cliente percebe a solução como parte do seu negócio / Mais valor agregado à sua operação / Experiência personalizada | Plataforma com a identidade do escritório / Mais valor percebido / Sensação de serviço exclusivo |
| Modelo 2 título | Com a marca Parcele Aqui | **Plataforma Parcele Aqui** |
| Modelo 2 bullets | Solução pronta e validada no mercado / Implementação ainda mais rápida / Comunicação clara e objetiva | Marca consolidada e reconhecida / Pronta para uso imediato / Evolução contínua da tecnologia |
| Slogan inferior | Dois modelos, o mesmo objetivo: **fechar mais negócios sem risco.** | **Você escolhe.** A segurança e a performance são as mesmas. |
| CTA | "Entender qual modelo escolher" (msg: qual modelo) | mantido |

---

## Dobra 9 — Quem Somos

H2, parágrafos e 6 cards (25 anos / 100% digital / 24/07 / Infraestrutura / Parcerias / Especialista): **já idênticos ao briefing**. Nenhuma alteração.

---

## Dobra 10 — Segurança

Kicker, H2, parágrafos e selos de certificação: **já idênticos ao briefing**. Nenhuma alteração.

---

## Dobra 11 — FAQ

Header atualizado:

| Campo | Antes | Agora |
|---|---|---|
| H2 | Pronto para fechar / **mais negócios sem / risco financeiro?** | Entenda melhor / a parceria **e o funcionamento / do Parcele Aqui** |
| Subtítulo | Pagamentos são uma das principais objeções no fechamento de **negócios imobiliários**… | Pagamentos são uma das principais objeções no fechamento de **negócios contábeis**… |

6 perguntas (desktop **e** mobile) — todas reescritas conforme briefing:

| # | Antes | Agora |
|---|---|---|
| 1 | Quem assume o risco da operação? | **O Parcele Aqui é seguro?** |
| 2 | É seguro oferecer parcelamento para meus clientes? | **Os boletos são liquidados à vista para o emissor?** |
| 3 | Em quanto tempo o valor é liquidado? | **O cliente pode usar mais de um cartão?** |
| 4 | Quais pagamentos podem ser parcelados? | **Quais pagamentos podem ser parcelados?** (resposta reescrita para contexto contábil) |
| 5 | Existe risco de inadimplência para o escritório? | **Existe risco de inadimplência para o escritório?** (resposta reescrita) |
| 6 | O cliente pode usar mais de um cartão? | **O escritório precisa ser uma instituição financeira?** |

Link final do FAQ: "Fale com um especialista." → msg `tenho uma dúvida e gostaria de falar com um especialista.` — **mantido**.

> ⚠️ Respostas 2 a 6 foram redigidas a partir do PDF de contabilidades (Figma estava vazio/com texto herdado). **Revisar com time comercial/jurídico antes de publicar.**

---

## Dobra 12 — CTA Final

| Campo | Antes | Agora |
|---|---|---|
| Kicker | Hora de fechar mais negócios | Próximo passo |
| H2 | mantido (Transforme barreiras financeiras em **oportunidades de fechamento**) | mantido |
| Corpo | Ofereça **parcelamento sem risco**, aumente suas conversões e **entregue mais valor aos seus clientes** com o Parcele Aqui. | Leve **parcelamento inteligente** para seus clientes e fortaleça o posicionamento do seu escritório com uma **solução segura, digital e sem risco.** |
| CTA | "Ver como funciona no meu negócio" (msg: como funciona) | mantido |
| Imagem | `secao-cta-final.png` | Mantida com TODO + alt atualizado |

---

## Footer / Header

**Preservados 100%**: estrutura, classes, paddings, todos os links externos do footer (parceleaqui.com.br/sobre-nos, /login, /simulacao, /politica-de-privacidade, /termos-de-servico, /preciso-de-ajuda, /politica-pld), CNPJ, endereço com link Maps, redes sociais (LinkedIn, Instagram), logo Potencial (powered by), ghost button "Fazer uma simulação", telefone (11) 3159-1380 e suporte técnico.

Único ajuste no header: texto do botão primário atualizado para "Quero simular parcelamento" + link já apontando para a mensagem de simulação (já estava correto na B2B).
