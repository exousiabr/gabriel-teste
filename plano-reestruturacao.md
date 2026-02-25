# Plano: Reestruturar Página de Vendas do Funil Invisível

## Contexto

A página de vendas atual (`/home/user/gabriel-teste/sites`) está com **ROAS negativo**: R$300/dia em ads → R$200/dia de retorno (ROAS 0.67). O produto é uma masterclass de 36 min por R$97 chamada "Funil Invisível™" do Lucas Vignoli. Tráfego misto (frio + retargeting), público de interesse "vendedores", criativos variados sem alinhamento com a página, **sem VSL**.

A página será completamente reestruturada para corrigir os problemas de conversão identificados na auditoria.

---

## Diagnóstico: Os 7 Assassinos de Conversão

### 1. QUIZ GATE OBRIGATÓRIO (Linhas 380-530)
**Impacto: CRÍTICO** — O visitante precisa completar **7 micro-conversões** (nome, 4 perguntas, animação fake de IA, WhatsApp) antes de ver UMA ÚNICA PALAVRA da oferta. Para tráfego frio, isso elimina ~70-85% dos visitantes. **Este é o principal motivo do ROAS negativo.**

### 2. MECANISMO NUNCA EXPLICADO
A página nunca explica O QUE É o "Funil Invisível". Diz o que ele faz ("ativa desejo de compra") mas não mostra os passos. Sem entender o mecanismo, o visitante frio não tem motivo para acreditar na promessa.

### 3. PROMESSA GENÉRICA E INACREDITÁVEL
"10 Clientes por Dia" — todo mundo no mercado promete isso. Para um dentista ou prestador de serviço que luta pra fechar 5 clientes por semana, 10/dia soa fantasioso. A promessa não é diferenciada da concorrência.

### 4. PROVAS QUE PARECEM FABRICADAS
Os depoimentos de WhatsApp são HTML/CSS renderizado (não screenshots reais). Público sofisticado reconhece isso como fake. Resultados exagerados ("3 clientes antes do almoço no primeiro dia") destroem credibilidade.

### 5. DOIS PREÇOS CAUSAM CONFUSÃO
R$67 (básico) vs R$97 (combo) — a diferença de R$30 é pequena demais pra criar ancoragem, mas grande o suficiente pra canibalizar vendas. O card básico com X vermelhos aparece PRIMEIRO no mobile.

### 6. CHECKBOX BLOQUEIA O BOTÃO DE COMPRA
O "Yes Ladder" desabilita fisicamente o botão de compra até o visitante marcar um checkbox. Isso transforma uma técnica psicológica em barreira funcional.

### 7. ESCASSEZ FALSA + SEM FAQ + SEM VSL
Timer de bônus via localStorage (resetável), zero seção de FAQ, nenhum vídeo de vendas. Para tráfego frio no Brasil, a ausência de VSL é o maior gap competitivo.

---

## Estratégia: Reestruturação Completa

### Nova Promessa + Ângulo

**Antes:** "Ganhe 10 Novos Clientes Todos os Dias Usando o Funil Invisível™"
**Depois:** "O Método de 3 Passos Que Transforma Seu Instagram Em Uma Máquina de Clientes — Sem Gastar Com Anúncios, Sem Fazer Dancinha, Sem Ter Milhões de Seguidores"

**Raciocínio:** A nova promessa é mais específica (3 passos), mais crível (não promete 10/dia logo de cara) e ataca 3 objeções reais ao mesmo tempo. O "Funil Invisível™" continua como mecanismo único mas agora a promessa sustenta ele.

### Nova Estrutura da Página

```
PÁGINA REESTRUTURADA (sem quiz gate — acesso direto)
═══════════════════════════════════════════════════

1. BARRA DE ALERTA (topo)
   → "Método usado por +30.000 pessoas | R$10M+ faturados"
   → Credibilidade instantânea, substitui o "Mind Reader"

2. HERO SECTION
   → Nova headline com promessa específica
   → Subheadline que conecta com a dor principal
   → 3 bullets de benefício
   → CTA primário
   → Placeholder para VSL futuro (imagem clicável ou embed)

3. SEÇÃO "POR QUE NADA FUNCIONOU ATÉ AGORA" (Inimigo Comum)
   → Copy aprofundado sobre o problema real
   → Ataca: "postar sem estratégia", "gastar com ads", "depender de indicação"
   → Mais profundo e específico que o atual

4. SEÇÃO "O FUNIL INVISÍVEL — COMO FUNCIONA" (Mecanismo Único) ★ NOVO
   → 3 passos visuais do método (alto nível, sem entregar tudo)
   → Passo 1: "O Post Magnético" — atrai sem parecer venda
   → Passo 2: "O Gatilho Invisível" — filtra curiosos, atrai compradores
   → Passo 3: "O Fechamento no WhatsApp" — script que converte
   → Isso cria ENTENDIMENTO e DESEJO

5. MENTOR (Lucas Vignoli)
   → Credenciais: R$10M faturados, 30k vendas
   → Foto + bio curta
   → CTA secundário

6. PROVA SOCIAL (reformulada)
   → Manter prints de WhatsApp MAS como imagens reais (não HTML)
   → Se não tiver screenshots reais: manter HTML mas com resultados
     mais realistas e detalhados
   → Manter áudios (são bons)
   → Adicionar contador: "Junte-se a +30.000 alunos"

7. O QUE VOCÊ RECEBE (detalhamento do produto) ★ NOVO
   → Lista dos módulos/aulas com descrição curta de cada
   → Bônus com valor individual
   → Isso mostra que R$97 vale muito mais

8. OFERTA ÚNICA (sem card básico)
   → Remover o card de R$67 — só o combo completo por R$97
   → Stack de valor reformulado com valores mais críveis
   → Botão SEMPRE ativo (sem checkbox bloqueante)
   → Checkbox de compromisso vira opcional (não bloqueia)

9. GARANTIA (expandida)
   → "Garantia Blindada de 7 Dias" com copy mais forte
   → "Se você aplicar os 3 passos e não atrair pelo menos 1
     cliente novo em 7 dias, devolvemos cada centavo."
   → Garantia condicional = mais poderosa que incondicional genérica

10. FAQ / QUEBRA DE OBJEÇÕES ★ NOVO
    → 8-10 perguntas mais comuns:
      "Funciona pra quem tem poucos seguidores?"
      "Preciso investir em tráfego pago?"
      "Quanto tempo até ver resultado?"
      "Funciona pro meu nicho?"
      "E se eu não souber vender?"
      etc.

11. CTA FINAL + URGÊNCIA
    → Último CTA com reforço de benefício
    → Remover timer fake de localStorage
    → Urgência real: "Preço promocional por tempo limitado"
      ou sem urgência nenhuma (melhor que urgência fake)

12. FOOTER
    → Disclaimer legal
```

### Mudanças Específicas no Código

| O que | Ação | Linhas atuais |
|-------|------|---------------|
| Quiz overlay inteiro | **REMOVER** completamente (HTML + CSS + JS) | 72-168, 380-530, 1023-1177 |
| Mind Reader Alert | **SUBSTITUIR** por barra de credibilidade estática | 167-169, 375-377 |
| Hero headline | **REESCREVER** com nova promessa | 540-542 |
| Hero subtitle | **REESCREVER** | 544-546 |
| Seção Inimigo Comum | **REESCREVER** copy mais profundo | 561-569 |
| Seção Mecanismo (3 passos) | **CRIAR** nova seção após inimigo comum | — (nova) |
| Prints WhatsApp | **AJUSTAR** textos mais realistas | 599-654 |
| Seção "O que você recebe" | **CRIAR** detalhamento do produto | — (nova) |
| Pricing card básico (R$67) | **REMOVER** inteiro | 743-764 |
| Pricing grid | **MUDAR** para single column centralizado | 298-299 |
| Pricing card premium | **MANTER** mas refatorar (botão sempre ativo) | 767-797 |
| Commitment checkbox | **TORNAR** opcional (não bloqueia botão) | 757-762, 789-796, 971-996 |
| Stack de valor | **AJUSTAR** valores mais críveis | 773-779 |
| Timer fake | **REMOVER** | 781-783, 998-1021 |
| Feature cards (mecanismo) | **MOVER** para antes da prova social | 803-829 |
| Garantia | **EXPANDIR** com copy mais forte | 832-840 |
| FAQ section | **CRIAR** nova | — (nova) |
| Sticky mobile CTA | **MANTER** | 847-849 |
| Pixel events | **MANTER** | 1179-1206 |
| devSkip function | **REMOVER** | 383-398 |

### Sobre o VSL

O Lucas não tem VSL gravado. Na página reestruturada, vamos:
1. Colocar um **placeholder visual** no hero (imagem do Lucas com play button)
2. Estruturar a página para funcionar SEM vídeo (texto puro otimizado)
3. Adicionar um comentário HTML indicando onde o VSL deve ser embedado quando disponível

**Recomendação forte:** O VSL é o upgrade de maior impacto que pode ser feito depois. Mesmo um vídeo simples de 10 min gravado no celular pode dobrar a conversão.

---

## Arquivos a Modificar

- `/home/user/gabriel-teste/sites` — reestruturação completa do HTML/CSS/JS

## Verificação

1. Abrir o arquivo no navegador e verificar visualmente
2. Testar no mobile (responsive)
3. Verificar que o quiz foi removido e a página abre direto
4. Verificar que o botão de compra funciona sem checkbox
5. Verificar que links de checkout (Eduzz) estão corretos
6. Commit e push para a branch
