# NullTrust-ByeJack

## 1) O que é
Um laboratório prático de Zero Trust focado em **Entra ID + Conditional Access + (opcional) Intune Compliance** e um **script Python** que audita postura via **Microsoft Graph** e gera um relatório.

## 2) Por que existe (objetivo)
- Consolidar fundamentos reais de identidade e acesso (Zero Trust) com decisões justificadas.
- Construir um portfólio “arquitetura + segurança + automação” (não só UI).
- Criar um trilho de estudo aplicado para AZ-305/AZ-500 enquanto evoluo nos cursos.

## 3) Escopo (o que entra / o que fica fora)
### Entra agora
- Entra ID: usuários fictícios, grupos, papéis básicos, contas break-glass.
- Conditional Access: 5 políticas demonstráveis com exceções documentadas.
- Evidências: prints/outputs + notas de decisão.
- Automação (Python): coletar políticas de CA e principals privilegiados via Graph e gerar relatório Markdown.

### Fora por enquanto
- SIEM/SOC (Sentinel), detecções/alertas avançados.
- Pentest, varredura de rede, scanners, hardening de infra extensa.
- Qualquer “feature” nova antes de fechar uma fase com entregável.

## 4) Entregáveis (o que vira portfólio)
- `README.md`: escopo, fases, decisões e critérios de pronto.
- `docs/decisions.md`: registro curto de decisões (por quê / impacto / trade-off).
- `docs/threat-model.md`: threat model simples (o que protejo, de quem, como).
- `src/`: script Python gerador de relatório.
- `evidence/`: evidências por fase (prints com dados mascarados quando necessário).

## 5) Roadmap (fases)
- **Fase 0 — Governança:** escopo fechado + estrutura do repo + templates de docs.
- **Fase 1 — Identidades:** usuários/grupos (admin bootstrap, 2 break-glass, perfis Finance/IT/Contractor) + MFA.
- **Fase 2 — Conditional Access:** 5 políticas + validação e evidências.
- **Fase 3 — Intune Compliance (opcional):** perfis de compliance + teste compliant vs non-compliant.
- **Fase 4 — Python Report:** script Graph → relatório Markdown (CA + privileged principals).

## 6) Critério de pronto por fase
Uma fase só está “concluída” quando:
- existe evidência em `evidence/`,
- existe ao menos 1 decisão registrada em `docs/decisions.md`,
- e o README/roadmap foi atualizado se algo mudou.

## 7) Avisos de segurança
- Nunca commitar secrets/tokens.
- Dados fictícios sempre que possível.
- Evidências devem mascarar informações sensíveis.
