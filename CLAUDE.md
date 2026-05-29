# Ágora — IA: leia só isto

## O que é este repositório

Arquivos de configuração da **Ágora** — comitê multidisciplinar de análise de ideias de negócios físicos e operacionais. Roda no Claude.ai como projeto.

Este repositório não tem código. Tem apenas `.md` que definem o comportamento de cada membro do comitê e do orquestrador.

## Estrutura

```
ORQUESTRADOR.md       ← regras de operação do comitê (ponto de entrada do projeto Claude.ai)
squad/
├── MAESTRO.md        ← consolida e dá o veredicto final
├── FINANCEIRO.md     ← viabilidade econômica, investimento, retorno
├── MERCADO.md        ← demanda, concorrência, posicionamento
├── OPERACIONAL.md    ← estrutura física, equipamentos, processos
├── JURIDICO.md       ← licenças, registro, tributação, obrigações
├── SETOR.md          ← cria especialista dinâmico do setor
├── AUDITOR.md        ← aponta falhas, riscos e otimismo excessivo
└── experts/          ← especialistas criados dinamicamente pelo SETOR
```

## Como editar

Cada `.md` é o system prompt de um membro. Edite diretamente — sem build, sem dependências.

**Para melhorar um membro:** edite o `.md` e faça commit. Remova e reanexa o arquivo no projeto Claude.ai para usar a versão atualizada.

**Para adicionar um membro fixo:** crie um novo `.md` em `squad/`, anexe ao projeto e atualize o `ORQUESTRADOR.md` para incluí-lo no fluxo.

## Relação com o Quorum

A Ágora é irmã do [Quorum](https://github.com/seuuser/quorum). O Quorum analisa produtos digitais. A Ágora analisa negócios físicos e operacionais. Mesma filosofia, contextos diferentes.

## Como montar no Claude.ai

1. Crie um projeto no Claude.ai com o nome **Ágora**
2. Anexe todos os `.md` do squad + o `ORQUESTRADOR.md`
3. Em **Project instructions**, escreva apenas:
   > Leia o arquivo ORQUESTRADOR.md e siga as instruções.
4. Abra uma conversa no projeto e apresente sua ideia
