# Layout - Programa de Embaixadores MEDsimple

Este documento especifica o design completo de cada seção da página de embaixadores, seguindo a identidade visual refinada (Background Grid, Albert Sans + Caveat, High Contrast).

## Identidade Visual Base
- **Background**: `#fcfcfc` com Grid de 40px em `#f1f1f1`.
- **Primary Text**: `#171717` (Neutral 900).
- **Secondary Text**: `#737373` (Neutral 500).
- **Blue**: `#6366f1` (Blue 500 / Ação).
- **Emerald**: `#10b981` (Emerald 500 / Acentos Manuscritos).
- **Fontes**: Albert Sans (Heading/Body) e Caveat (Destaques).

---

## Seção 1: Hero (Já Demonstrado)
### Arquetipo e Constraints
- Arquetipo: Single Focus (Centralizado)
- Constraints: Hand-drawn underline (Caveat), Hero Social Proof Badge, Background Grid
- Justificativa: Cria impacto imediato e autoridade, alinhado ao design atual do site principal.

### Conteúdo
- Headline: "Seja o nosso representante na sua universidade"
- Subheadline: "Estamos selecionando apenas 1 embaixador por instituição. Garanta sua vaga e tenha acesso a benefícios que nenhum outro estudante possui."
- CTA: "Quero me candidatar agora"

### Layout & Animações
- Padding: `96px 0` (py-24).
- Título: `clamp(2rem, 8vw, 3.75rem)`, font-weight 700.
- Transições: Hover no botão principal com `translateY(-2px)` e expansão da sombra.

---

## Seção 2: Oportunidade Única (Já Demonstrado)
### Arquetipo e Constraints
- Arquetipo: Contained Center
- Constraints: Badge Outline, Hand-drawn accent
- Justificativa: Foca na escassez ("Um único líder") de forma clean.

### Conteúdo
- Título: "Uma vaga. Uma universidade. Um líder."
- Conteúdo: "O Programa de Embaixadores MEDsimple não é para todos..."

---

## Seção 3: Benefícios Exclusivos
### Arquetipo e Constraints
- Arquetipo: Bento Box
- Constraints: Hover Glow, Scale In (Stagger)
- Justificativa: Permite mostrar múltiplos benefícios de pesos diferentes de forma moderna e organizada.

### Conteúdo
- Lista de benefícios: 
  - Acesso privilegiado a novidades.
  - Condições especiais (Cupons).
  - Networking com fundadores.
  - Reconhecimento oficial (Certificado).
  - Premiações por desempenho.

### Layout
- Grid: `lg:grid-cols-6` para layout bento.
- Card 1 (Acesso): Ocupa 3 colunas.
- Card 2 (Cupom): Ocupa 3 colunas.
- Card 3, 4, 5: Ocupam 2 colunas cada.
- Padding interno dos cards: `32px`.
- Border: `1px solid #e5e7eb`, fundo branco puro.

### Interatividade
- Hover Lift: `translateY(-8px)` com `box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1)`.
- Glow suave: Borda muda para `#10b981` no hover.

---

## Seção 4: Como funciona (O Caminho)
### Arquetipo e Constraints
- Arquetipo: Scroll Storytelling (Flow Vertical)
- Constraints: Draw SVG Path (Linha conectora), Sequential Reveal
- Justificativa: Guia o usuário pelo processo de seleção de forma linear e atraente.

### Conteúdo
1. Inscrição: Formulário.
2. Seleção: Análise de perfil.
3. Onboarding: Treinamento.
4. Atuação: Resultados.

### Elementos Visuais
- Linha pontilhada animada (Emerald) que percorre os números `1, 2, 3, 4` conforme o scroll.
- Números grandes em Background: Font-size `120px`, Opacity `0.05`, Color `Neutral-900`.

---

## Seção 5: FAQ & Objeções
### Arquetipo e Constraints
- Arquetipo: Split Assimetrico (70/30)
- Constraints: Glassmorphism (no bloco de resposta), Fade Up
- Justificativa: Mantém as perguntas visíveis à esquerda enquanto as respostas são reveladas à direita, evitando o layout de sanfona comum.

### Layout
- Coluna Esquerda: Título "Dúvidas Frequentes" + Lista de perguntas.
- Coluna Direita: Box fixo (Sticky) que atualiza a resposta conforme a pergunta selecionada.

---

## Seção 6: CTA Final (Escassez Máxima)
### Arquetipo e Constraints
- Arquetipo: Poster (Impacto total)
- Constraints: Headline >150px (Background text), Floating Elements
- Justificativa: Cria o fechamento com urgência, reforçando o branding.

### Conteúdo
- Headline: "A próxima vaga pode ser sua. Ou do seu colega."
- Botão: "Aplicar para vaga exclusiva" (Tamanho grande).

---

## Responsividade Geral
- Mobile: Padding vertical reduzido para `64px`. Layouts Grid convertidos para `grid-cols-1`.
- Tablet: Bento Box se torna `grid-cols-2`.
- Desktop: Full implementation dos arquetipos descritos.
