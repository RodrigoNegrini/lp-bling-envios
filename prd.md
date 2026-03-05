# PRD — Bling Envios Landing Page

## Visão Geral

Landing page interna ao ERP Bling para apresentação e ativação do produto **Bling Envios** (powered by Melhor Envio). O objetivo é converter usuários Bling já logados em usuários ativos do módulo de logística, apresentando benefícios, funcionalidades e removendo objeções via FAQ.

**Contexto de acesso:** A página é exibida dentro do shell do ERP Bling (navbar superior presente com menus: Cadastros, Suprimentos, Vendas, Finanças, Serviços, Contabilidade).

---

## Estrutura de Seções (ordem vertical)

1. Hero
2. "Sua expedição no piloto automático" (Tabs)
3. "Quanto mais você envia, menos paga na etiqueta"
4. "Condições exclusivas para alto volume de envios"
5. Benefícios em destaque (3 itens texto)
6. "Um time de especialistas jogando junto com você"
7. Perguntas Frequentes (FAQ Accordion)
8. Botão flutuante fixo (canto inferior direito)

---

## Componentes

---

### 1. Hero Section

**Layout:** Full-width, fundo verde escuro. Duas colunas: esquerda com conteúdo textual + CTA; direita com imagem de pessoa e UI mockups flutuantes.

**Elementos:**
- Logo "Envios por Melhor Envio" (superior esquerdo da seção)
- Dois badges/tags em pill:
  - "Sem mensalidade"
  - "100% dentro do Bling"
- **H1:** "Fretes mais baratos e logística completa sem sair do Bling"
- **Subtítulo:** "Transforme horas de expedição em minutos. Acesse fretes exclusivos, emita etiquetas, rastreie seus envios e tenha suporte logístico especializado direto do ERP."
- **CTA Button:** "Começar agora →"
- Coluna direita: foto de mulher segurando caixa parda + 3 cards de UI flutuantes simulando notificações de pedido/etiqueta/entregue

**UI Mockup cards (coluna direita):**
- Card 1: "Novo pedido de varejo" (linha verde destacada)
- Card 2: "2 etiquetas / Fique ainda mais barato e rápido" (em processamento)
- Card 3: "Entregue" (badge de status verde)

**Comportamento:**
- Estático; o CTA redireciona para ativação do módulo
- Badges não são clicáveis

---

### 2. Seção "Sua expedição no piloto automático"

**Layout:** Fundo verde claro/mint. Título centralizado + subtítulo. Abaixo: sistema de 3 tabs horizontais + área de conteúdo com lista de benefícios (esquerda) e screenshot de produto (direita).

**Tabs:**
| Tab         | Estado Padrão  |
|-------------|---------------|
| Cotação     | Ativa (default) |
| Postagem    | Inativa        |
| Pós-Envio   | Inativa        |

**Comportamento das Tabs:**
- Clicar em uma tab atualiza o conteúdo da área abaixo sem reload de página (SPA/JS toggle)
- Tab ativa: texto em verde, underline/indicador visual verde
- Tab inativa: texto em cinza escuro sem underline

**Conteúdo por Tab:**

#### Tab: Cotação (default ativa — LP_-_ME__2_.png)
- Ícone check + "Faça a cotação automática entre os principais transportadores direto do seu pedido de venda."
- Ícone check + "Compare opções (Correios, Jadlog, LATAM, Loggi) e tenha acesso a frete competitivas sem precisar de contratos individuais ou burocracias."
- Ícone check + "Recarregue seu saldo direto no Bling e pague apenas pelo que enviar, sem mensalidades ou taxas de adesão."
- Screenshot: tela de cotação com tabela de transportadoras e preços

#### Tab: Postagem (LP_-_ME__4_.png)
- Ícone check + "Elimine integrações externas que travam sua operação gerando a remessa instantaneamente dentro do Bling."
- Ícone check + "Tudo fica pronto para enviar logo após a emissão da nota, com a DANFE simplificada impressa junto com a etiqueta."
- Ícone check + "Selecione até 100 pedidos e imprima etiquetas de postagem em lote instantaneamente."
- Ícone check + "Conte com diversos pontos de coleta ou, se disponível, com a comodidade da coleta no seu endereço."
- Screenshot: tela de postagem com seleção de pedidos e modal de confirmação de logística

#### Tab: Pós-Envio (LP_-_ME__3_.png)
- Ícone check + "Acompanhe cada passo do entrego em tempo real, com status atualizado no painel de pedidos."
- Ícone check + "Se houver qualquer imprevisto (atraso ou avaria), abra chamados de suporte diretamente pelo pedido."
- Ícone check + "Gere etiquetas de logística reversa para trocas e devoluções e rastreie cada pacote direto no Bling."
- Screenshot: tela de rastreamento com status de entrega por pedido

---

### 3. Seção "Quanto mais você envia, menos paga na etiqueta"

**Layout:** Fundo branco. Duas colunas: esquerda com texto, direita com foto editorial (homem idoso em ambiente de estoque/expedição).

**Elementos:**
- **H2:** "Quanto mais você envia, menos paga na etiqueta"
- **Parágrafo:** "Comece com taxas competitivas e desbloqueie descontos progressivos e serviços exclusivos automaticamente conforme seu volume de envios aumenta. Fazemos tudo de forma simples e integrada à sua rotina."
- Imagem: duas fotos em composição (homem com caixa, fundo logístico)

---

### 4. Seção "Condições exclusivas para alto volume de envios"

**Layout:** Full-width, fundo verde escuro. Conteúdo centralizado.

**Elementos:**
- **H2:** "Condições exclusivas para alto volume de envios"
- **Parágrafo:** "Desbloqueie negociações especiais para operações com mais de 10 envios por dia e tenha um time dedicado a otimizar seus custos e sua estratégia logística."
- **CTA Button:** "Cotar minha operação →" (estilo outline branco ou branco sólido)

**Comportamento:** CTA direciona para formulário ou fluxo de qualificação para alto volume.

---

### 5. Seção Benefícios em Texto (3 itens)

**Layout:** Fundo branco. Duas colunas: esquerda com foto editorial do mesmo homem; direita com 3 blocos de texto.

**Itens:**

#### "Logística nativa e pronta para usar"
Sua loja já nasce com a logística resolvida. Ative integrações com Correios e transportadoras privadas com poucos cliques, sem precisar de contratos individuais ou burocracias. É só ativar e começar a enviar.

#### "Etiqueta e DANFE em um clique"
Selecione o pedido e resolva a expedição de uma vez. Após a emissão da nota fiscal, com apenas um clique o sistema gera a etiqueta de envio já com a DANFE simplificada, pronta para imprimir.

#### "Resolva atrasos e extravios direto do pedido"
Esqueça as horas perdidas em filas de atendimento. Teve problema na entrega? Acione o suporte para atrasos ou extravios com um clique no tela do pedido, sem ping-pong entre sua logística e a transportadora.

---

### 6. Seção "Um time de especialistas jogando junto com você"

**Layout:** Full-width, fundo verde escuro. Conteúdo centralizado.

**Elementos:**
- **H2:** "Um time de especialistas jogando junto com você"
- **Parágrafo:** "Deixe a burocracia da logística com quem entende do assunto. Tenha à disposição um time dedicado dentro do Bling para orientar sobre boas práticas, apoiar com configurações e negociar condições e resoluções direto com as transportadoras."

---

### 7. FAQ — Perguntas Frequentes (Accordion)

**Layout:** Fundo cinza claro (desktop) / branco (mobile). Título "Perguntas frequentes" em H2 escuro.

**Comportamento:**
- Accordion: cada item pode ser expandido/colapsado individualmente
- Múltiplos itens podem estar abertos simultaneamente (comportamento não-exclusivo)
- Estado padrão: todos fechados (mobile) / todos abertos (versão desktop da imagem FAQ__1_.png)
- Ícone: chevron `∨` (fechado) / `∧` (aberto), cor verde
- Animação: slide suave ao expandir/colapsar

**Itens do FAQ:**

#### 1. "Preciso configurar APIs complexas para ativar o Bling Envios?"
Não. A integração é nativa e "plug & play". O Bling Envios já vem instalado no seu ERP. Você só precisa configurar suas preferências logísticas e sua loja já estará pronta para cotar e gerar etiquetas imediatamente, sem precisar de chaves de API ou ajuda técnica.

🔗 Link externo: "Integração nativa com a logística Envios por Melhor Envio"

#### 2. "Os fretes no Bling são mais baratos do que contratar direto no balcão?"
Sim, como o Bling negocia pelo volume somado de milhares de lojistas, conseguimos tabelas de preços muito mais agressivas do que uma negociação individual de balcão. Além da economia, você ganha a liberdade de escolher entre múltiplas transportadoras (Correios, Jadlog, Loggi, etc.) em um único lugar, sem precisar assumir compromissos de volume mínimo com cada uma delas.

#### 3. "Como funciona o pagamento das etiquetas?"
O pagamento é feito via Crédito em Carteira, garantindo total controle dos seus gastos. Você recarrega seu saldo no Bling (via Pix ou boleto) e o valor dos fretes é descontado automaticamente na hora da emissão.

🔗 Link externo: "Etiquetas da logística Envios por Melhor Envio"

#### 4. "É obrigatório emitir Nota Fiscal para usar o serviço?"
Para a maioria dos envios comerciais, a Nota Fiscal Eletrônica (NF-e) é obrigatória e garante a segurança da carga. No entanto, o sistema também permite a geração de etiquetas com Declaração de Conteúdo para casos específicos, desde que respeitadas as legislações estaduais e as regras da transportadora escolhida.

#### 5. "Onde acompanho o rastreamento das minhas encomendas?"
Tudo acontece dentro do Bling. O código de rastreio é gerado automaticamente assim que a etiqueta é criada e o status de entrega (postado, em trânsito, entregue) é atualizado diretamente no painel de pedidos.

🔗 Link externo: "Rastrear a encomenda da logística Envios por Melhor Envio"

#### 6. "Se houver atraso ou extravio, com quem eu falo?"
O Bling atua como seu intermediador junto às transportadoras. Em caso de avarias, extravios ou dúvidas sobre a entrega, você abre um chamado diretamente pelo painel do seu pedido e nossa equipe especializada resolve o problema com a logística parceira.

#### 7. "Existem restrições sobre o que posso enviar?"
Sim. O Bling Envios segue as políticas de transporte dos parceiros (Correios e transportadoras privadas). Não é permitido o envio de produtos ilícitos, perigosos, inflamáveis ou vivos. Além disso, fique atento aos limites de dimensão e peso de cada transportadora, que são informados automaticamente no momento da cotação.

🔗 Link externo: "Guia de produtos que podem ser enviados pelo Melhor Envio"

**Estilo dos links externos:**
- Ícone de "abrir em nova aba" à esquerda do texto
- Cor: `#1DB87E` (verde link)
- Prefixo de label: "Para mais detalhes, acesse:"

---

### 8. Botão Flutuante Fixo (FAB)

**Posição:** Fixo no canto inferior direito da viewport

**Elementos:**
- Label: "Vídeo" (ou ícone de play)
- Background: verde
- Shape: pill ou retangular arredondado

**Comportamento:** Abre modal ou inline player de vídeo de apresentação do produto

---

## Estados e Interações Globais

| Elemento        | Estado         | Comportamento                              |
|-----------------|----------------|--------------------------------------------|
| CTA buttons     | Hover          | Background escurece ~10%, cursor pointer   |
| FAQ item        | Fechado        | Só exibe pergunta + chevron ∨              |
| FAQ item        | Aberto         | Exibe resposta + links + chevron ∧         |
| Tab             | Ativa          | Verde + underline                          |
| Tab             | Inativa        | Cinza escuro, sem underline                |
| Links externos  | Hover          | Underline aparece                          |
| FAB Vídeo       | Hover          | Leve scale ou sombra adicional             |

---

## Acessibilidade

- Accordion FAQ deve ser navegável por teclado (Enter/Space para abrir/fechar)
- CTAs devem ter aria-label descritivo
- Contraste de texto sobre fundos verdes deve atender WCAG AA mínimo
- Imagens decorativas com `alt=""`; imagens de produto com alt descritivo

---

## Fora de Escopo (não presente nas imagens)

- Footer global do Bling (assumido como componente externo)
- Navbar superior (componente shell do ERP, não da LP)
- Fluxo pós-clique em "Começar agora" (onboarding separado)