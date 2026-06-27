# Pesquisa: Claude como Gestor de Mídias (verificada)

> Relatório consolidado da pesquisa profunda (108 subagentes, 25 fontes primárias,
> 24 afirmações confirmadas por verificação tripla). Data: 2026-06-27.
> NÃO é aconselhamento jurídico — a leitura do Provimento 205/2021 deve ser
> validada com a OAB seccional.

## Conclusão em uma linha
Dá pra fazer, mas **não existe uma ferramenta única** que gere arte + legenda +
aprove + publique em FB/IG/TikTok. É preciso **montar um "stack"** de 3 peças:
(1) quem **gera** o conteúdo, (2) quem **gera a arte**, (3) quem **publica/agenda** —
com a **aprovação humana** entre o passo 2 e o 3.

---

## 1. Geração de conteúdo (legendas, roteiros, carrosséis) — skills do Claude Code
- **stevenflanagan1/social-ai-team** ⭐143 — o mais completo. "Time de social media"
  em skills do Claude Code: orquestrador, caption-writer (IG/FB/TikTok/X/LinkedIn),
  social-creative-designer (cria arte via Nano Banana MCP) e publisher.
  **Diferencial: tem "pause-and-approve gates" (aprovação humana a cada etapa).**
- **filnik/social-media-manager-AI** (MIT, ⭐5) — só GERA (carrossel, roteiro de
  vídeo p/ Reels/TikTok/YouTube, ideias). Não publica. Bom de "canibalizar" ideias.
- **zxkane/social-agents** ⭐25 — agentes via Claude Agent SDK (TypeScript).

## 2. Geração de arte/imagem — servidores MCP
- **shinpr/mcp-image** ⭐129 — Gemini (Nano Banana 2/Pro) + opção GPT-Image; tem
  preset "social media". Bom candidato para a identidade visual dos carrosséis.
- **GongRzhe/Image-Generation-MCP-Server** — modelo Flux (Replicate).
- **guinacio/claude-image-gen** — Gemini, integra via Skills ou MCP.
- **writingmate/imagegen-mcp** — GPT-Image-1/DALL-E, Imagen 4, Gemini, Flux.

## 3. Publicação/agendamento em FB/IG/TikTok
- **Postiz (gitroomhq/postiz-app)** ⭐32k, AGPL-3.0 — **a opção mais madura**.
  Agendador self-hostável (alternativa ao Buffer/Hootsuite), suporta FB/IG/TikTok.
  Tem repo irmão **postiz-agent** que conecta ao Claude. ⚠️ Licença AGPL-3.0 impõe
  obrigações se for modificado e oferecido via rede — avaliar.
- **posteverywhere/mcp** (MIT, ⭐1) — MCP que agenda via SaaS PostEverywhere.
  Fino e **pago** (conta + API key). Baixa adoção.
- **tn819/buffer-mcp** — MCP que usa a API do Buffer (exige token do Buffer).
- **jlbadano/ig-mcp** ⭐152 — MCP só de Instagram Business (Meta Graph API).
- **TikTok:** ⚠️ **não há MCP de publicação verificado**. O único MCP de TikTok
  (Seym0n/tiktok-mcp) é só leitura/análise. Publicar exige a **TikTok Content
  Posting API** via um agregador (Postiz/Blotato), com auditoria do app.

## 4. Voz dos vídeos
- **VibeVoice** (Microsoft, TTS open-source) — para narração. ⚠️ Confirmar licença
  de uso comercial e requisitos de hardware antes de adotar.

## 5. Requisitos de API (a real barreira não é a IA, é o onboarding)
- **Instagram + Facebook:** Meta Graph API + conta **Business/Creator** ligada a uma
  **Página do Facebook** + app no Facebook Developer + token de longa duração +
  **App Review** da Meta para permissões avançadas. (IG nunca publica em conta pessoal.)
- **TikTok:** Content Posting API + processo de **auditoria** do app (sem auditoria,
  só posta em modo privado/teste).

---

## 6. ⚠️ OAB — Provimento 205/2021 do CFOAB (o eixo que manda no projeto)

### PERMITIDO
- Publicidade de caráter **meramente informativo/institucional**.
- Conteúdo jurídico **educativo**; lives/vídeos com objetivo ilustrativo/instrutivo.
- Caixinha de perguntas para propagar conteúdo jurídico.
- Impulsionamento **moderado e informativo** (sem oferta de serviço / sem captação).
- Botão "Clique Aqui"/contato — **sem** chamadas tipo "contrate nossos serviços".
- Identificação discreta: nome, número OAB, telefone, e-mail, QR Code.
- Linguagem **moderada, discreta, sóbria** — sem teor persuasivo/comercial/sensacionalista.

### PROIBIDO (colide direto com "captar clientes automaticamente")
- **Captação mercantilizada** de clientela / oferta direta de serviços (inclusive **DM**).
- **Promessa/garantia de resultado** ("garantimos sua causa").
- Divulgação de **casos concretos** e **resultados** de processos (OAB/SP é expressa).
- Divulgação de **preços/honorários** ou valores recuperados.
- Consultoria **gratuita como isca**, brindes, adesivos/pintura em veículos.
- Uso de **logotipos/símbolos da OAB**.

> IMPLICAÇÃO: o objetivo precisa ser reformulado de "captar clientes" para
> **"presença informativa/educacional que gera autoridade"**. E a aprovação humana
> deve incluir uma **checagem de conformidade** (filtro p/ promessa de resultado,
> caso concreto, preço, oferta direta) antes de cada publicação.

---

## 7. Arquitetura recomendada (a confirmar com o cliente)
```
Claude (skills) ──gera legenda+roteiro──►  ┐
MCP de imagem  ──gera arte (id. visual)──► │──► RASCUNHO
VibeVoice      ──gera narração do vídeo──►  ┘        │
                                                     ▼
                                       [APROVAÇÃO HUMANA + check OAB]  ◄── advogado
                                                     │ (aprovado)
                                                     ▼
                                   Postiz (self-host) ──► FB / IG / TikTok
```

## Fontes primárias (GitHub / OAB)
- github.com/stevenflanagan1/social-ai-team · github.com/filnik/social-media-manager-AI
- github.com/zxkane/social-agents · github.com/gitroomhq/postiz-app (+ postiz-agent)
- github.com/posteverywhere/mcp · github.com/tn819/buffer-mcp · github.com/jlbadano/ig-mcp
- github.com/seym0n/tiktok-mcp · github.com/shinpr/mcp-image
- github.com/GongRzhe/Image-Generation-MCP-Server · github.com/guinacio/claude-image-gen
- github.com/writingmate/imagegen-mcp
- eticaedisciplina.oab.org.br/provimento · oab.org.br (cartilha de publicidade) · oabsp.org.br
