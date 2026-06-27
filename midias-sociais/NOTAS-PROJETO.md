# Projeto: Gestão de Mídias do Escritório com IA

> Documento de trabalho. Reúne decisões, referências e ferramentas levantadas
> ao longo da conversa para automatizar a produção e publicação de conteúdo
> (Instagram, Facebook e TikTok) com **aprovação humana antes de postar**.
> Última atualização: 2026-06-27.

## Objetivo
Produzir e gerenciar conteúdo informativo (carrosséis, posts estáticos e vídeos)
para atrair clientes para as teses do escritório, com identidade visual forte e
fluxo: **IA cria → advogado aprova → publica/agenda**.

## Plataformas (ordem de início)
- Instagram (conta Business + Meta Graph API)
- Facebook (Página + Meta Graph API — mesmo ecossistema)
- TikTok (Content Posting API, com revisão de app)

## Posicionamento de marca (decisão do cliente)
Vender **transformação, não serviço**: segurança, autoridade, experiência,
tempo/tranquilidade e sofisticação. Estética premium e sóbria.
> Régua OAB: NÃO prometer/garantir resultado, valores, urgência artificial,
> superlativos ("melhor"), nem ostentação. Vender "estar em boas mãos".

## "Rosto" do escritório
Cliente quer ver opções antes de decidir. Avaliar 3 conceitos:
1. Anfitrião de marca assumidamente virtual (mais seguro p/ OAB).
2. Identidade visual sem rosto (logo/paleta/tipografia/templates).
3. Personagem fotorrealista (maior risco ético — conteúdo jurídico não pode
   ser atribuído a "pessoa" fictícia que aparente ser advogado real).

## Conformidade OAB (eixo central do projeto)
Provimento 205/2021 do CFOAB + Código de Ética. Conteúdo informativo/educativo
é permitido; captação/mercantilização é proibida. Aprovação humana obrigatória
antes de qualquer publicação.

---

## Ferramentas e referências salvas

### Voz / narração de vídeo
- **VibeVoice** — modelo open-source de Text-to-Speech (TTS) da Microsoft,
  voltado a áudio longo e conversacional (estilo podcast/multi-locutor).
  Uso pretendido: gerar a **narração das vozes dos vídeos** do escritório.
  - A confirmar na pesquisa: repositório oficial/mirror atual, licença de uso,
    requisitos de hardware/execução e se a licença permite uso comercial.

### Referências de conteúdo (benchmark)
- Perfil @guilherme.craus (Instagram) — citado pelo cliente como referência de
  quem ensina o fluxo de IA para conteúdo. Usar como inspiração de estrutura,
  não para cópia de arte/texto.

---

## Stack recomendado (pós-pesquisa — ver PESQUISA-FERRAMENTAS.md)
- Geração de conteúdo: skills do Claude Code (base: stevenflanagan1/social-ai-team).
- Geração de arte: MCP de imagem (base: shinpr/mcp-image — Gemini Nano Banana).
- Publicação/agendamento: Postiz self-host (FB/IG/TikTok), com staging/aprovação.
- Voz de vídeo: VibeVoice (confirmar licença comercial).
- Trava obrigatória: aprovação humana + checagem de conformidade OAB antes de postar.

## Decisões travadas (2026-06-27 — cliente delegou a direção ao Claude)
- **Premium — direção de arte:** C (Selo/monograma heráldico "SN") + lógica editorial
  (Dossiê) nos carrosséis. Marinho + dourado.
- **Massificado — nome:** "Souza Neto Direitos".
- **Massificado — identidade:** azul-confiança (#1f6f8b) + âmbar (#e3a93a) + marinho +
  muito branco; títulos em pergunta; selo SN ligando à casa-mãe.
- **Estrutura:** dois perfis separados (premium institucional + massificado varejo).

## Pendência externa
- [ ] Entender `contrato.souzanetoadvocacia.com.br` (não acessível pelo ambiente —
  bloqueio de rede). Cliente vai descrever. Provável destino de lead / onboarding.

## Pendências
- [x] Finalizar relatório de pesquisa → ver PESQUISA-FERRAMENTAS.md.
- [ ] Confirmar dados do VibeVoice (repo oficial/mirror, licença, requisitos).
- [ ] Apresentar 3 conceitos de identidade/"rosto".
- [ ] Decidir entre Postiz self-host vs. SaaS (Buffer/Blotato) para publicar.
- [ ] Montar passo a passo de configuração técnica (Meta Business + App Review; TikTok audit).
- [ ] Modelos de carrossel/vídeo + CTAs OAB-safe.
- [ ] Validar interpretação do Provimento 205/2021 com a OAB seccional.
