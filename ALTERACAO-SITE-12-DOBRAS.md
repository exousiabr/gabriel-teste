# PLANO DE ALTERACOES — Aplicando as 12 Dobras na LP

> Documento de referencia com TODAS as mudancas que vamos fazer no arquivo `sites`,
> linha por linha, secao por secao. Cada alteracao tem: o que mudar, por que mudar,
> e o texto/codigo exato que vai entrar.

---

## VISAO GERAL: ANTES vs DEPOIS

### Estrutura ATUAL (13 secoes)
```
1. Credibility Bar
2. Hero (headline + bullets + CTA)
3. Common Enemy
4. Mechanism: 3 Steps
5. Features ("Por que funciona")
6. Mentor (Lucas Vignoli)
7. Social Proof (prints WhatsApp)
8. Audio Testimonials
9. What You Get
10. Pricing
11. Guarantee
12. FAQ
13. Final CTA
```

### Estrutura NOVA (15 secoes)
```
1.  Credibility Bar .................. (manter)
2.  Hero ............................. (ALTERAR headline)
3.  Common Enemy ..................... (manter)
4.  Mechanism: 3 Steps ............... (manter)
5.  Features ......................... (manter)
6.  Mentor ........................... (manter)
7.  Social Proof (prints) ............ (manter)
8.  Audio Testimonials ............... (manter)
9.  What You Get ..................... (REESCREVER — foco ferramenta)
10. "Vozes da Cabeca" ................ (CRIAR — secao nova)
11. "Papo Reto / Custo da Inacao" ... (CRIAR — secao nova)
12. Pricing .......................... (manter)
13. Guarantee ........................ (manter)
14. FAQ .............................. (manter)
15. Final CTA ........................ (manter)
```

**Resumo das mudancas:**
- 1 secao ALTERADA (Hero)
- 1 secao REESCRITA (What You Get)
- 2 secoes NOVAS (Vozes da Cabeca + Papo Reto)
- 11 secoes MANTIDAS como estao

---

## ALTERACAO 1 — HEADLINE DO HERO (Dobra 1)

### Por que mudar
A headline atual nao segue a formula completa: [Resultado] + [Tempo] + [Sem objecao principal].
Falta o elemento de TEMPO e a objecao esta separada no subtitulo.

### O que mudar

**HEADLINE ATUAL (linha 306-308):**
```html
<h1 class="hero-title reveal">
    O Método de 3 Passos Que Transforma Seu Instagram Em Uma <span class="text-accent">Máquina de Clientes</span>
</h1>
```

**HEADLINE NOVA:**
```html
<h1 class="hero-title reveal">
    Atraia Clientes Todos os Dias Pelo Instagram <span class="text-accent">— Sem Anúncios, Sem Dancinha, Sem Milhares de Seguidores</span>
</h1>
```

**SUBTITULO ATUAL (linha 310-312):**
```html
<p class="hero-subtitle reveal">
    Sem gastar com anúncios, sem fazer dancinha, sem precisar de milhões de seguidores. Funciona mesmo que você <strong>esteja começando do zero</strong>.
</p>
```

**SUBTITULO NOVO:**
```html
<p class="hero-subtitle reveal">
    O método de 3 passos que já gerou <strong>+30 mil vendas</strong>. Monte seu funil em 36 minutos e comece a receber clientes no WhatsApp <strong>ainda hoje</strong>.
</p>
```

### Justificativa
- Headline agora tem: resultado (clientes todos os dias) + objecoes (sem anuncios, sem dancinha, sem seguidores)
- Subtitulo agora tem: prova (30 mil vendas) + tempo (36 minutos) + urgencia (ainda hoje)
- Tudo numa leitura rapida de 3 segundos

---

## ALTERACAO 2 — REESCRITA "O QUE VOCE RECEBE" (Dobra 5)

### Por que mudar
A secao atual vende "informacao" (aula, tecnicas, entenda). Deveria vender "FERRAMENTA" (o que a pessoa SAI COM NA MAO). Cliente de low ticket compra ferramenta, nao conteudo.

### O que mudar

**MODULO 1 — ATUAL:**
```html
<div class="module-item__title">Masterclass Funil Invisível™</div>
<div class="module-item__desc">Aula direta de 36 minutos onde você monta o funil completo do zero. Sem enrolação — sai da aula com tudo pronto pra ativar.</div>
```

**MODULO 1 — NOVO:**
```html
<div class="module-item__title">Seu Funil Montado e Pronto pra Ativar</div>
<div class="module-item__desc">Em 36 minutos você sai com o funil completo configurado no seu Instagram. Não é teoria — é passo a passo prático. Terminou a aula, ativa no mesmo dia.</div>
```

---

**MODULO 2 — ATUAL:**
```html
<div class="module-item__title">MasterClass de Vendas no WhatsApp</div>
<div class="module-item__desc">Scripts testados em +30 mil vendas para converter mensagens em pagamentos. Copie, cole e adapte pro seu negócio.</div>
```

**MODULO 2 — NOVO:**
```html
<div class="module-item__title">5 Scripts de WhatsApp Prontos pra Copiar e Colar</div>
<div class="module-item__desc">Roteiros de conversa testados em +30 mil vendas. Abre o WhatsApp, cola o script, adapta pro seu produto. Sem precisar "saber vender".</div>
```

---

**MODULO 3 — ATUAL:**
```html
<div class="module-item__title">Fechamento Avançado</div>
<div class="module-item__desc">Técnicas para lidar com "vou pensar", "tá caro" e todas as objeções que travam a venda. Aumente sua taxa de conversão.</div>
```

**MODULO 3 — NOVO:**
```html
<div class="module-item__title">Checklist de Fechamento: 8 Respostas Prontas</div>
<div class="module-item__desc">Pra cada "vou pensar", "tá caro", "preciso ver com meu marido" — você tem a resposta exata na mão. Checklist prático que destrava a venda na hora.</div>
```

---

**MODULO 4 — ATUAL:**
```html
<div class="module-item__title">Entenda o Marketing de 2026</div>
<div class="module-item__desc">O que mudou, o que funciona agora e como se posicionar à frente da concorrência no cenário atual.</div>
```

**MODULO 4 — NOVO:**
```html
<div class="module-item__title">Guia Rápido: O Que Funciona AGORA no Instagram</div>
<div class="module-item__desc">Mapa direto do que parou de funcionar e o que está gerando resultado em 2026. Pra você não perder tempo com estratégia ultrapassada.</div>
```

### Justificativa
Cada item agora responde: "O que eu SAIO COM NA MAO?" — ferramenta, nao informacao.

---

## ALTERACAO 3 — CRIAR SECAO "VOZES DA CABECA" (Dobra 3) [NOVA]

### Por que criar
Objecoes estao escondidas no FAQ (la embaixo). Precisam ser matadas ANTES do preco. Isso e CRITICO pra conversao — a pessoa precisa se sentir entendida antes de ver o valor.

### Onde inserir
DEPOIS da secao "What You Get" (secao 9), ANTES do Pricing (secao 12).

### Codigo HTML completo da nova secao

```html
<!-- ================= 10. VOZES DA CABECA (Objection Killer) ================= -->
<section class="section-padding">
    <div class="container">
        <div class="section-header reveal">
            <span class="section-tag" style="background: rgba(239, 68, 68, 0.08); color: #EF4444;">Eu Sei o Que Você Tá Pensando</span>
            <h2 class="section-title">Antes de Decidir,<br>Deixa Eu Ser Honesto.</h2>
        </div>

        <div class="objection-list reveal" style="max-width: 700px; margin: 0 auto; display: flex; flex-direction: column; gap: 16px;">

            <div class="objection-item" style="display: flex; align-items: flex-start; gap: 18px; background: var(--bg-card); border: 1px solid var(--border-light); border-radius: 16px; padding: 24px; transition: 0.3s;">
                <div style="width: 40px; height: 40px; background: rgba(239, 68, 68, 0.1); border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 18px; flex-shrink: 0; border: 1px solid rgba(239, 68, 68, 0.2);">🤔</div>
                <div>
                    <div style="font-family: var(--ff-heading); font-size: 16px; font-weight: 700; margin-bottom: 6px; color: #EF4444;">"Isso não funciona pro meu nicho"</div>
                    <div style="font-size: 14px; color: var(--text-muted); line-height: 1.6;">Já foi testado em +40 nichos diferentes. Dentistas, advogados, lojistas, personal trainers, freelancers, nutricionistas... O método é sobre <strong style="color:#fff;">comportamento de compra</strong>, não sobre nicho.</div>
                </div>
            </div>

            <div class="objection-item" style="display: flex; align-items: flex-start; gap: 18px; background: var(--bg-card); border: 1px solid var(--border-light); border-radius: 16px; padding: 24px; transition: 0.3s;">
                <div style="width: 40px; height: 40px; background: rgba(239, 68, 68, 0.1); border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 18px; flex-shrink: 0; border: 1px solid rgba(239, 68, 68, 0.2);">🤔</div>
                <div>
                    <div style="font-family: var(--ff-heading); font-size: 16px; font-weight: 700; margin-bottom: 6px; color: #EF4444;">"Não tenho seguidores suficientes"</div>
                    <div style="font-size: 14px; color: var(--text-muted); line-height: 1.6;">A Bruna fez a primeira venda com <strong style="color:#fff;">400 seguidores</strong>. O método não depende de audiência grande — depende de <strong style="color:#fff;">atrair a pessoa certa</strong>.</div>
                </div>
            </div>

            <div class="objection-item" style="display: flex; align-items: flex-start; gap: 18px; background: var(--bg-card); border: 1px solid var(--border-light); border-radius: 16px; padding: 24px; transition: 0.3s;">
                <div style="width: 40px; height: 40px; background: rgba(239, 68, 68, 0.1); border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 18px; flex-shrink: 0; border: 1px solid rgba(239, 68, 68, 0.2);">🤔</div>
                <div>
                    <div style="font-family: var(--ff-heading); font-size: 16px; font-weight: 700; margin-bottom: 6px; color: #EF4444;">"Não sei vender"</div>
                    <div style="font-size: 14px; color: var(--text-muted); line-height: 1.6;">Você recebe <strong style="color:#fff;">scripts prontos de WhatsApp</strong>. É copiar e colar. Não precisa de lábia, dom ou experiência. O script faz o trabalho pesado por você.</div>
                </div>
            </div>

            <div class="objection-item" style="display: flex; align-items: flex-start; gap: 18px; background: var(--bg-card); border: 1px solid var(--border-light); border-radius: 16px; padding: 24px; transition: 0.3s;">
                <div style="width: 40px; height: 40px; background: rgba(239, 68, 68, 0.1); border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 18px; flex-shrink: 0; border: 1px solid rgba(239, 68, 68, 0.2);">🤔</div>
                <div>
                    <div style="font-family: var(--ff-heading); font-size: 16px; font-weight: 700; margin-bottom: 6px; color: #EF4444;">"Já tentei de tudo e nada deu certo"</div>
                    <div style="font-size: 14px; color: var(--text-muted); line-height: 1.6;">Você tentou <strong style="color:#fff;">sem método</strong>. Postar sem estratégia não é tentar — é torcer. Isso aqui é um sistema com começo, meio e fim. Diferente de tudo que você já viu.</div>
                </div>
            </div>

            <div class="objection-item" style="display: flex; align-items: flex-start; gap: 18px; background: var(--bg-card); border: 1px solid var(--border-light); border-radius: 16px; padding: 24px; transition: 0.3s;">
                <div style="width: 40px; height: 40px; background: rgba(239, 68, 68, 0.1); border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 18px; flex-shrink: 0; border: 1px solid rgba(239, 68, 68, 0.2);">🤔</div>
                <div>
                    <div style="font-family: var(--ff-heading); font-size: 16px; font-weight: 700; margin-bottom: 6px; color: #EF4444;">"Será que vale o investimento?"</div>
                    <div style="font-size: 14px; color: var(--text-muted); line-height: 1.6;">Custa <strong style="color:#fff;">menos que um almoço</strong>. Se gerar 1 único cliente, já pagou o investimento. E você ainda tem <strong style="color:#10B981;">7 dias de garantia</strong> pra testar sem risco.</div>
                </div>
            </div>

            <div class="objection-item" style="display: flex; align-items: flex-start; gap: 18px; background: var(--bg-card); border: 1px solid var(--border-light); border-radius: 16px; padding: 24px; transition: 0.3s;">
                <div style="width: 40px; height: 40px; background: rgba(239, 68, 68, 0.1); border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 18px; flex-shrink: 0; border: 1px solid rgba(239, 68, 68, 0.2);">🤔</div>
                <div>
                    <div style="font-family: var(--ff-heading); font-size: 16px; font-weight: 700; margin-bottom: 6px; color: #EF4444;">"Não tenho tempo"</div>
                    <div style="font-size: 14px; color: var(--text-muted); line-height: 1.6;">A aula tem <strong style="color:#fff;">36 minutos</strong>. A execução é pelo celular, em 15 min por dia. Sem rotina complicada. Se você tem tempo pra rolar o feed, tem tempo pra aplicar isso.</div>
                </div>
            </div>

        </div>
    </div>
</section>
```

### Design
- Mantém o design system atual (bg-card, border-light, ff-heading, text-muted)
- Icone de 🤔 em circulo vermelho pra cada objecao
- Objecao em vermelho (#EF4444) — resposta em muted com palavras-chave em branco
- Mesmo pattern visual dos module-items (familiaridade)

---

## ALTERACAO 4 — CRIAR SECAO "PAPO RETO" (Dobra 10) [NOVA]

### Por que criar
Nao fazemos a math do custo de NAO agir. O preco de R$97 precisa parecer ridiculo comparado ao prejuizo de continuar sem metodo.

### Onde inserir
DEPOIS da secao "Vozes da Cabeca" (nova secao 10), ANTES do Pricing (secao 12).

### Codigo HTML completo da nova secao

```html
<!-- ================= 11. PAPO RETO — Custo da Inacao ================= -->
<section class="section-padding" style="background: rgba(239, 68, 68, 0.02); border-top: 1px solid rgba(239, 68, 68, 0.08); border-bottom: 1px solid rgba(239, 68, 68, 0.08);">
    <div class="container">
        <div style="max-width: 700px; margin: 0 auto; text-align: center;" class="reveal">
            <span class="section-tag" style="background: rgba(239, 68, 68, 0.08); color: #EF4444;">Papo Reto</span>
            <h2 class="section-title" style="margin-bottom: 30px;">Quanto Custa<br><span style="color: #EF4444;">NÃO</span> Resolver Isso?</h2>

            <div style="display: flex; flex-direction: column; gap: 16px; text-align: left; margin-bottom: 40px;">

                <div style="display: flex; align-items: center; gap: 16px; background: rgba(239, 68, 68, 0.04); border: 1px solid rgba(239, 68, 68, 0.1); border-radius: 14px; padding: 18px 22px;">
                    <span style="font-size: 24px; flex-shrink: 0;">📉</span>
                    <span style="color: rgba(255,255,255,0.7); font-size: 15px;">Mais um mês <strong style="color:#fff;">sem clientes previsíveis</strong> — dependendo de indicação e sorte</span>
                </div>

                <div style="display: flex; align-items: center; gap: 16px; background: rgba(239, 68, 68, 0.04); border: 1px solid rgba(239, 68, 68, 0.1); border-radius: 14px; padding: 18px 22px;">
                    <span style="font-size: 24px; flex-shrink: 0;">🔥</span>
                    <span style="color: rgba(255,255,255,0.7); font-size: 15px;">Mais <strong style="color:#fff;">R$500 jogados em tráfego</strong> que não converte — ou horas criando conteúdo sem retorno</span>
                </div>

                <div style="display: flex; align-items: center; gap: 16px; background: rgba(239, 68, 68, 0.04); border: 1px solid rgba(239, 68, 68, 0.1); border-radius: 14px; padding: 18px 22px;">
                    <span style="font-size: 24px; flex-shrink: 0;">⏰</span>
                    <span style="color: rgba(255,255,255,0.7); font-size: 15px;">Mais <strong style="color:#fff;">3 meses postando todo dia</strong> sem resultado — tempo que você nunca recupera</span>
                </div>

            </div>

            <div style="background: var(--bg-card); border: 2px solid rgba(16, 185, 129, 0.2); border-radius: 20px; padding: 32px; margin-bottom: 30px;">
                <p style="color: var(--text-muted); font-size: 15px; margin-bottom: 16px;">A math é simples:</p>

                <div style="display: flex; justify-content: center; align-items: center; gap: 20px; flex-wrap: wrap; margin-bottom: 20px;">
                    <div style="text-align: center;">
                        <div style="font-family: var(--ff-heading); font-size: 28px; font-weight: 900; color: #EF4444;">R$500</div>
                        <div style="font-size: 12px; color: var(--text-muted); text-transform: uppercase; letter-spacing: 1px;">por mês em tráfego</div>
                    </div>
                    <div style="font-size: 24px; color: var(--text-muted);">=</div>
                    <div style="text-align: center;">
                        <div style="font-family: var(--ff-heading); font-size: 28px; font-weight: 900; color: #EF4444;">R$6.000</div>
                        <div style="font-size: 12px; color: var(--text-muted); text-transform: uppercase; letter-spacing: 1px;">por ano jogados fora</div>
                    </div>
                </div>

                <div style="width: 60px; height: 2px; background: rgba(255,255,255,0.1); margin: 20px auto;"></div>

                <p style="font-family: var(--ff-heading); font-size: 22px; font-weight: 800; color: #10B981; margin-bottom: 8px;">
                    R$97 resolve isso.
                </p>
                <p style="color: var(--text-muted); font-size: 14px;">
                    O custo da inação é <strong style="color:#fff;">SEMPRE</strong> maior que o preço da solução.
                </p>
            </div>

            <a href="#pricing" class="btn-glow btn-green" style="max-width: 420px; margin: 0 auto;">Resolver Isso Agora por R$97</a>
        </div>
    </div>
</section>
```

### Design
- Fundo com leve tint vermelho pra criar urgencia visual (diferente das outras secoes)
- Math visual com numeros grandes em vermelho vs solucao em verde
- CTA direto pro pricing
- Contrast forte: R$6.000 (vermelho) vs R$97 (verde)

---

## RESUMO DO CSS NECESSARIO

Nao precisa de CSS novo. Todas as secoes usam classes e estilos inline ja existentes no design system:
- `var(--bg-card)`, `var(--border-light)`, `var(--ff-heading)`, `var(--text-muted)`
- Classes: `.section-padding`, `.section-tag`, `.section-title`, `.container`, `.reveal`, `.btn-glow`, `.btn-green`

A unica coisa que pode ser adicionada no CSS pra hover dos objection-items:

```css
/* Hover nos objection items */
.objection-item:hover {
    border-color: rgba(239, 68, 68, 0.2);
}
```

---

## ORDEM DE EXECUCAO

| # | Acao | Risco | Dificuldade |
|---|------|-------|-------------|
| 1 | Alterar headline e subtitulo do Hero | Baixo | Facil (troca de texto) |
| 2 | Reescrever "O Que Voce Recebe" | Baixo | Facil (troca de texto) |
| 3 | Criar secao "Vozes da Cabeca" | Medio | Medio (HTML novo) |
| 4 | Criar secao "Papo Reto" | Medio | Medio (HTML novo) |

Tempo estimado de implementacao: todas as 4 alteracoes podem ser feitas de uma vez.

---

## O QUE NAO VAMOS MEXER

- Credibility Bar (ta ok)
- Common Enemy (ta solido)
- Mechanism / 3 Steps (ta claro)
- Features (ta funcional)
- Mentor (ta bom)
- Social Proof — prints (ta forte)
- Audio Testimonials (ta bom)
- Pricing — estrutura e valores (manter)
- Guarantee (ta clara)
- FAQ (manter — mas algumas respostas agora sao redundantes com a "Vozes da Cabeca", podemos revisar depois)
- Final CTA (manter)
- Todo o CSS/JS existente (manter)
- Pixel do Facebook (manter)
- Sticky mobile CTA (manter)

---

## CHECKLIST FINAL

- [ ] Headline do Hero alterada (formula completa)
- [ ] Subtitulo do Hero alterado (prova + tempo + urgencia)
- [ ] Modulo 1 "What You Get" reescrito (ferramenta)
- [ ] Modulo 2 "What You Get" reescrito (ferramenta)
- [ ] Modulo 3 "What You Get" reescrito (ferramenta)
- [ ] Modulo 4 "What You Get" reescrito (ferramenta)
- [ ] Secao "Vozes da Cabeca" criada (6 objecoes)
- [ ] Secao "Papo Reto" criada (custo da inacao)
- [ ] CSS hover adicionado (.objection-item)
- [ ] Testar responsividade mobile
- [ ] Testar que todos os links/CTAs funcionam
- [ ] Testar scroll reveal nas secoes novas
