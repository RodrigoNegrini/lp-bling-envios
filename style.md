# Style Guide — Bling Envios Landing Page

## Identidade Visual

O produto é o **Bling Envios**, uma solução de logística integrada ao ERP Bling, desenvolvida em parceria com o **Melhor Envio**. O visual deve transmitir: confiança, praticidade e modernidade para lojistas.

---

## Paleta de Cores

| Token           | Hex       | Uso                                                     |
|-----------------|-----------|---------------------------------------------------------|
| Primary Green   | `#1A6B3C` | Hero background, CTAs principais, seções de destaque    |
| Secondary Green | `#2D9E60` | Botões secundários, ícones de check, chevrons do FAQ    |
| Light Mint      | `#E8F5EE` | Background de seções alternadas (ex.: "Piloto automático") |
| Dark Navy       | `#1A2B3C` | Títulos e headings principais                           |
| Body Text       | `#3D4D5C` | Parágrafos e textos de suporte                          |
| Link/Accent     | `#1DB87E` | Links externos, texto de destaque em verde claro        |
| White           | `#FFFFFF` | Background padrão, cards do FAQ, texto sobre fundos escuros |
| Light Gray BG   | `#F5F6F7` | Background da seção FAQ (versão desktop expandida)      |
| Border Gray     | `#E2E6EA` | Bordas de cards e separadores                           |

---

## Tipografia

### Famílias

A LP utiliza **duas famílias** tipográficas com papéis bem definidos:

| Família        | Variações utilizadas             | Uso                                      |
|----------------|----------------------------------|------------------------------------------|
| **Gilroy**     | `Gilroy-Bold`, `Gilroy-Medium`   | Toda a LP — headings, corpo, FAQs, CTAs  |
| **Arial**      | `Arial` weight `700`             | Exclusivamente nos badges/tags do Hero   |

> **Nota:** Gilroy é uma fonte paga (Radomir Tinkov). Para ambientes web, deve ser carregada via `@font-face` com os arquivos licenciados. Fallback recomendado: `'Gilroy', 'Helvetica Neue', Arial, sans-serif`.

---

### Escala e Aplicação por Elemento

| Elemento                        | Fonte             | Tamanho aprox. | Cor            |
|---------------------------------|-------------------|----------------|----------------|
| H1 Hero                         | `Gilroy-Bold`     | 32–40px        | `#FFFFFF`      |
| H2 Seções (fundo escuro)        | `Gilroy-Bold`     | 26–32px        | `#FFFFFF`      |
| H2 Seções (fundo claro)         | `Gilroy-Bold`     | 26–32px        | `#1A2B3C`      |
| H3 Benefícios / Cards           | `Gilroy-Bold`     | 17–20px        | `#1A2B3C`      |
| Subtítulo Hero                  | `Gilroy-Medium`   | 14–16px        | `#FFFFFF`      |
| Subtítulo de seção              | `Gilroy-Medium`   | 14–16px        | `#3D4D5C`      |
| Itens com check (tabs)          | `Gilroy-Medium`   | 13–15px        | `#3D4D5C`      |
| Corpo / Parágrafos gerais       | `Gilroy-Medium`   | 14–15px        | `#3D4D5C`      |
| Perguntas do FAQ                | `Gilroy-Bold`     | 14–15px        | `#1A2B3C`      |
| Respostas do FAQ                | `Gilroy-Medium`   | 13–14px        | `#3D4D5C`      |
| "Para mais detalhes, acesse:"   | `Gilroy-Medium`   | 13–14px        | `#3D4D5C`      |
| Links externos do FAQ           | `Gilroy-Bold`     | 13–14px        | `#1DB87E`      |
| Labels das tabs (ativa)         | `Gilroy-Bold`     | 13–14px        | `#2D9E60`      |
| Labels das tabs (inativa)       | `Gilroy-Medium`   | 13–14px        | `#3D4D5C`      |
| Texto dos botões CTA            | `Gilroy-Bold`     | 14–15px        | `#FFFFFF`      |
| Badges / Tags ("Sem mensalidades", "100% dentro do Bling") | `Arial` weight `700` | 11–13px | `#1A2B3C` ou `#FFFFFF` |

---

## Espaçamento e Layout

- **Max-width do conteúdo:** ~1200px, centralizado
- **Padding lateral (desktop):** 40–60px
- **Padding lateral (mobile):** 16–24px
- **Espaçamento entre seções:** 60–80px vertical
- **Gap entre itens de lista/cards:** 16–24px
- **Border-radius padrão (cards, FAQs):** 8–12px

---

## Iconografia

- Ícones de check: círculo verde (`#2D9E60`) com checkmark branco
- Chevron do accordion FAQ: seta simples, cor `#2D9E60`, rotaciona 180° quando aberto
- Ícone de link externo: ícone de "abrir em nova aba" em verde

---

## Botões

### CTA Principal (Hero)
- Background: `#2D9E60`
- Texto: Branco, SemiBold
- Border-radius: 6–8px
- Padding: 12px 24px
- Hover: escurecer ~10%
- Ícone de seta → à direita do texto

### CTA Secundário (Seção escura)
- Border: 1px solid `#FFFFFF` ou background branco com texto verde
- Mesmo shape do principal

---

## Badges / Tags

- Shape: pill (border-radius: 999px)
- Background: branco semi-transparente ou verde claro com borda
- **Fonte: `Arial`, weight `700`** — exceção tipográfica exclusiva deste componente
- Tamanho: 11–13px
- Cor do texto: `#1A2B3C` ou `#FFFFFF` conforme contraste com o fundo
- Exemplos: "Sem mensalidades", "100% dentro do Bling"

---

## Imagens e Mídias

- Hero: fotografia de pessoa (mulher segurando caixa), fundo verde, composição com UI mockups flutuantes
- Seção benefícios: foto de homem idoso (empresário), tom quente, estilo editorial
- Screenshots de produto: bordas arredondadas, leve sombra
- Proporção das fotos: livre, mas bem enquadradas com assunto centrado

---

## Seções — Fundos Alternados

| Seção                           | Fundo          |
|---------------------------------|----------------|
| Hero                            | Verde `#1A6B3C` |
| "Piloto automático"             | Mint `#E8F5EE`  |
| "Quanto mais você envia..."     | Branco          |
| "Condições exclusivas"          | Verde `#1A6B3C` |
| Benefícios (3 cards texto)      | Branco          |
| "Um time de especialistas"      | Verde `#1A6B3C` |
| FAQ                             | Cinza claro `#F5F6F7` (desktop) / Branco (mobile) |

---

## Responsividade

- **Desktop:** Layout em colunas (2 colunas na maioria das seções)
- **Mobile:** Stack vertical; hero com texto empilhado acima da imagem; FAQ accordion fechado por padrão
- Tabs de "Cotação / Postagem / Pós-Envio": horizontais no desktop, scrollável horizontalmente no mobile