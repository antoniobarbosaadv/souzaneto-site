# CONTEXTO COMPLETO — Projeto de Mídias com IA (Souza Neto) — para retomar em nova sessão

## Quem sou / o escritório
- Dr. Antônio Barbosa de Souza Neto, OAB/MS 22.741, sócio fundador. Campo Grande/MS.
- Souza Neto Advogados: advocacia empresarial premium (Contratos, Governança, Compliance,
  Agronegócio, Tributário) + um núcleo massificado (INSS, consumidor, trabalhista).
- Identidade existente: marinho #0e1c2e + dourado #c2a26a, serifa Cormorant + Inter.
  Logo wordmark "SOUZA NETO" — MANTER, não trocar.
- Site: souzanetoadvocacia.com.br · Funil de contratos: contrato.souzanetoadvocacia.com.br
  (produto: contrato por advogado em 24h, R$989).

## Objetivo
Operação de mídias sociais altamente automatizada para captar clientes / fechar contratos,
foco no massificado via TikTok + Instagram. Quero o MÍNIMO de trabalho manual — idealmente
só aprovar/reprovar. ÉTICA/OAB é MINHA responsabilidade — não me alerte sobre OAB, foque em
executar.

## Arquitetura de marca (decidida)
- Dois perfis, mesma DNA:
  - Premium: @souzaneto.law (Instagram já existe) + Facebook. Sem TikTok.
  - Massificado: "Souza Neto Direitos" → @souzaneto.direitos (Instagram NOVO + TikTok NOVO).
    Cores: marinho + azul-confiança #1f6f8b + âmbar #e3a93a. Tom didático/íntimo, títulos em pergunta.
- Teses massificado: Golpe do Pix, Auxílio-acidente, Salário-maternidade, Trabalhista (+ Contratos ligada ao funil).

## O "rosto" = LÍVIA (avatar IA, decisão central)
- Persona fixa, ultrarrealista, SEMPRE a mesma: mulher brasileira ~30 anos, linda, olhos cor
  de mel, sardinhas, beleza natural. Tom "firme mas doce", close íntimo, conta o direito como
  um SEGREDO/fofoca jurídica. NÃO promete vantagens — comenta julgados públicos reais e
  convida a pessoa a buscar/se informar sobre seus direitos.
- Apelo duplo: homem ouve porque ela é bela; mulher ouve porque gosta da "fofoca"/segredo.
- Nome de trabalho: Lívia.

## Stack de ferramentas (status real)
- HeyGen Criador (mensal) — ASSINADO. Motor do avatar (Avatar IV, melhor p/ foto-avatar).
  Lívia criada (escolhida a opção #2 de 4 rostos). Escolhido sobre Creatify (testei e preferi HeyGen).
- ElevenLabs Starter ($5) — ASSINADO. Voz. API key criada (acessos: Text to Speech, Vozes-Ler,
  Modelos) e VINCULADA à Lívia dentro do HeyGen.
- Fliki Standard (anual) — ASSINADO. Apoio: vídeos faceless/variação (não-avatar).
- Metricool — A ASSINAR. Publicação/agendamento/aprovação (IG+FB+TikTok).
- Make.com — A CONFIGURAR. Motor da automação (fase 2).
- Google Drive + Calendar — JÁ CONFIGURADOS pelo assistente: pasta "Souza Neto — Mídias Sociais"
  (fluxo: Ideias&Roteiros / Em produção / Aguardando aprovação / Aprovados / Publicados /
  Templates&Marca / Documentos), Semana 1 do calendário editorial lançada + lembrete de
  renovação do Fliki (27/05/2027).

## Aprendizados-chave (não repetir erros)
- Foto-avatar (HeyGen IV) tem leve "tell" de foto se mexendo — inerente a pessoa fictícia.
  Solução: B-ROLL intercalado (Lívia em rajadas curtas) + voz boa (ElevenLabs). Voz pesa mais
  que o avatar no realismo.
- HeyGen Criador: ~200 créditos/mês = ~10 min de Avatar IV. No volume queima crédito (~$5/min
  extra). Solução: MIX de formatos — Lívia (hero) + Fliki faceless + carrossel p/ volume.
- Gestos sutis (lean-in, micro-expressão); exagero amplia o "tell". Ambiente quente/íntimo via
  "Looks" do HeyGen, mantendo o rosto IDÊNTICO.
- O assistente NÃO controla o navegador do cliente nem opera apps de terceiros (HeyGen/Fliki/
  Metricool) — só guia, opera o Google do cliente, e constrói a automação. Login/pagamento/2FA
  = sempre o cliente.
- Filosofia: SHIPPAR rápido primeiro, automatizar depois (com lastro de resultado).
- ⚠️ PRECISÃO JURÍDICA: TODO roteiro passa por revisão de advogado(a) do escritório
  (Dra. Larissa) ANTES de gerar o vídeo. Erro factual em conteúdo jurídico é grave.
  CORREÇÃO já aplicada (27/06): auxílio-acidente só cabe a empregado (CLT), doméstico,
  avulso e segurado especial — NÃO a autônomo/MEI/contribuinte individual (Lei 8.213/91,
  art. 18 §1º). Salário-maternidade é o oposto (autônoma/MEI TÊM direito). Não confundir.

## O que estamos fazendo AGORA
Refinando o "Look" da Lívia no HeyGen: ajustando enquadramento (de close → plano médio
mostrando o ambiente aconchegante) e gestos íntimos, mantendo o rosto idêntico. Em seguida:
gerar o 1º VÍDEO REAL (golpe do Pix), sem marca d'água.

### Prompts/roteiros aprovados
**Rosto Lívia:**
> Ultra-realistic cinematic close-up portrait of a beautiful young Brazilian woman, 30 years old, striking honey amber eyes, soft natural freckles across nose and cheeks, radiant warm skin, gentle inviting smile with a slightly secretive expression, natural glossy makeup, soft wavy brown hair, elegant dark blazer, photorealistic, 4k, natural skin texture, vertical 9:16

**Look ambiente (plano médio, mostra cenário):**
> Medium shot, waist-up framing, pulled back so the cozy home office is visible around her — desk, warm lamp, soft blurred bookshelves behind. Keep her face, freckles and honey eyes exactly the same. Warm cinematic lighting, gentle confiding expression.

**Movimento (Avatar IV):**
> gentle subtle movements, leaning slightly forward as if confiding, soft warm micro-expressions, calm intimate delivery, minimal hand gestures

**Roteiro Vídeo #1 (Golpe do Pix):**
> Oi... senta aqui que isso aqui pouca gente sabe. Sabe quando a pessoa cai num golpe do Pix e o banco diz que a culpa é só da vítima? Pois é... nem sempre é assim. O STJ já entendeu que os bancos têm o dever de monitorar movimentações suspeitas — e podem, sim, ser responsabilizados. Cada caso é um caso, claro. Mas se isso aconteceu com você ou com alguém que você conhece, não fica quieto sem se informar. Me segue que eu te conto seus direitos, sem juridiquês.

## Próximos passos, em sequência
1. Finalizar o Look da Lívia (enquadramento + ambiente) → travar.
2. Gerar o 1º vídeo real (golpe do Pix): Avatar IV + voz ElevenLabs + 9:16 → legendas → 1080p.
3. Criar perfis: @souzaneto.direitos no Instagram (profissional) + TikTok (Business). Bios em PERFIS-BIOS.md.
4. Assinar Metricool → conectar IG + TikTok → fluxo de aprovação.
5. Publicar o 1º vídeo (soft launch).
6. Produzir os próximos (8 roteiros em ROTEIROS-LOTE-1.md; calendário em CALENDARIO-EDITORIAL.md).
7. FASE 2 — Automação (Make + HeyGen API + ElevenLabs + b-roll + legenda → Drive aprovação →
   Metricool). Meta: só aprovar no celular.
8. Escalar com mix de formatos (Lívia hero + Fliki faceless + carrossel).

## Onde está tudo
- GitHub, branch `claude/github-media-manager-research-wnye0s`, pasta `midias-sociais/`.
  Docs: PESQUISA-FERRAMENTAS, ARQUITETURA-DOIS-NUCLEOS, ESTRATEGIA-VIDEO, PLANO-IMPLANTACAO,
  MAPA-DO-SETUP, PLANO-AVATAR-AUTOMACAO, CALENDARIO-EDITORIAL, ROTEIROS-LOTE-1, PERFIS-BIOS,
  GUIA-CRIACAO-CONTAS, MAO-NA-MASSA-ASSINATURAS, NOTAS-PROJETO + boards visuais (PNG).
- Google Drive: pasta "Souza Neto — Mídias Sociais".

## Como me tratar
Sou acelerado e odeio perder tempo / editar manualmente. Me dê passos curtos e diretos,
decida por mim quando eu disser "você que manda", seja honesto sobre limites (não prometa o
que não entrega), e foque em SHIPPAR. OAB é comigo.
