# Plano — Rosto IA Fixo + Automação 100% (você só aprova)

> Decisão do cliente (2026-06-27): rosto IA ultrarrealista, sempre a mesma pessoa,
> que comenta julgados públicos e convida a buscar direitos. Zero edição manual —
> cliente só aprova/reprova. Ética sob responsabilidade do cliente.

## Stack desta fase
| Função | Ferramenta | Por quê |
|---|---|---|
| Avatar ultrarrealista | **HeyGen** | Melhor avatar fotorrealista + voz + **API** p/ automação |
| Voz | HeyGen (PT-BR) ou **ElevenLabs** | Consistente; ElevenLabs = premium |
| Automação/orquestração | **Make.com** (ou n8n) | Liga roteiro → HeyGen → Drive → Metricool |
| Publicação | **Metricool** | Agenda/aprova nas redes |
| Faceless/apoio | **Fliki** (já assinado) | Conteúdo b-roll/repurpose secundário |

## A PERSONA (proposta para aprovação)
- **Quem:** "rosto" recorrente do **Souza Neto Direitos** — uma comentarista jurídica
  acessível e confiável (não promete resultado; comenta julgado real e convida a informar-se).
- **Sugestão de look:** mulher brasileira, ~35 anos, ar profissional e simpático, blazer
  escuro / blusa clara, fundo de estúdio/escritório desfocado, luz suave. (Aberto a masculino
  ou outro perfil — é só falar.)
- **Nome de marca (sugestão):** a definir com o cliente (ex.: um primeiro nome + "Souza Neto
  Direitos"). Sem título que implique advogada real, se o cliente preferir.
- **Voz:** PT-BR feminina, clara e calorosa (HeyGen nativa p/ começar; ElevenLabs depois).

### Prompt do avatar (para gerar no HeyGen / image-gen) — aprovar
> "Ultra-realistic photographic portrait of a Brazilian woman, ~35 years old, professional
> and approachable, trustworthy warm expression, dark tailored blazer over white blouse,
> modern blurred office/studio background, soft professional key light, looking straight at
> camera, head-and-shoulders, vertical 9:16, photorealistic, 4k, natural skin texture."
- Gerar UMA vez → salvar como **avatar fixo** → reutilizar em todos os vídeos (mesma pessoa sempre).

## Pilar de conteúdo do avatar: "Julgado da vez"
- Comenta um **julgado público real** (STJ/TJ/TST/INSS) em linguagem simples.
- Estrutura: gancho → o que o tribunal decidiu → o que isso significa pra você →
  convite a se informar/buscar direito (CTA).
- Fonte dos julgados: bases públicas (eu trago e resumo).

## Arquitetura da automação (você só aprova)
```
1. Eu gero o roteiro (comentário do julgado) → cai numa planilha/pasta no Drive.
2. Make.com lê o roteiro → chama a API do HeyGen (avatar fixo + voz) → renderiza o vídeo.
3. Vídeo + legenda caem na pasta Drive "3 · Aguardando aprovação".
4. Você recebe um aviso (WhatsApp/Telegram/e-mail) → APROVA ou REPROVA (1 toque).
5. Aprovado → Make envia ao Metricool → agenda/publica nos perfis.
```
- Legendas: HeyGen gera (ou passo extra no Make).
- Reprovado → volta pra mim ajustar. Nada vai ao ar sem o seu toque.

## O que cada um faz
- 🧑‍💼 **Você:** cria contas + paga + cola as API keys (1 vez) + aprova/reprova.
- 🤖 **Eu:** roteiros, persona, prompts, blueprint da automação, condução.
- ⚙️ **Make + HeyGen + Metricool:** executam sozinhos.

## Assinaturas desta fase (criar/pagar)
1. **HeyGen** — plano com **API** habilitada (confirmar tier; avatar custom + créditos de API).
2. **Make.com** — começar no Free; subir pro Core (~$9/mês) conforme volume.
3. **Metricool** — (já planejado) conectar os perfis.
4. **ElevenLabs** — opcional (voz premium).
5. **Fliki** — já assinado; vira apoio (faceless/repurpose).

## Ordem de execução
1º Aprovar persona (look/voz/nome) e os prompts.
2º Criar/pagar HeyGen + Make + Metricool.
3º Gerar o avatar fixo (1 vez) + travar a voz.
4º Eu monto o blueprint do Make (HeyGen → Drive → aprovação → Metricool).
5º Vídeo-piloto do avatar → você aprova → publica → escala.
