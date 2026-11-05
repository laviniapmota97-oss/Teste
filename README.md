# Especialista Jurídico — Agente e Skill para Claude Code

Um **subagente** e uma **skill** de Claude Code especializados em **direito brasileiro**: contratos, empresarial/LGPD, trabalhista, cível/consumidor e processo civil.

## Estrutura

```
.claude/
├── agents/
│   └── especialista-juridico.md        # Subagente (carrega a skill automaticamente)
└── skills/
    └── especialista-juridico/
        ├── SKILL.md                    # Método, fontes, formatos de entrega e limites éticos
        ├── referencias/
        │   ├── contratos.md
        │   ├── empresarial-lgpd.md
        │   ├── trabalhista.md
        │   ├── civel-consumidor.md
        │   └── processual-prazos.md
        └── modelos/
            ├── parecer.md
            ├── peticao-inicial.md
            ├── notificacao-extrajudicial.md
            ├── checklist-revisao-contrato.md
            └── contrato-prestacao-servicos.md
```

## Como usar

Abra o Claude Code na pasta deste repositório e:

- **Chame o agente:** "Use o especialista-juridico para revisar o contrato `contrato.pdf`."
- **Ou use só a skill:** digite `/especialista-juridico` e descreva o caso.

Exemplos de pedidos:
- "Fui demitido sem justa causa em 10/09/2026 após 4 anos e 3 meses. Quais verbas tenho direito e qual o prazo para pagamento?"
- "Revise este contrato de prestação de serviços do ponto de vista da contratante."
- "Redija uma notificação extrajudicial cobrando R$ 8.500 de aluguéis atrasados."
- "Comprei um celular pela internet há 5 dias e me arrependi. O que posso fazer?"
- "Faça um parecer sobre a responsabilidade do banco por um golpe do PIX."

Para usar em outros projetos, copie a pasta `.claude/` para o projeto ou para `~/.claude/` (uso global).

## Aviso

O conteúdo tem caráter informativo e de apoio. A legislação e a jurisprudência mudam: confira sempre as fontes oficiais. A análise não substitui a atuação de advogado inscrito na OAB.
