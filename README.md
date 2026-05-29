# Ágora

Um comitê multidisciplinar para avaliar ideias de negócios físicos e operacionais. Você apresenta uma ideia — abrir uma empresa de limpeza de PCs, comprar uma impressora 3D para vender produtos, montar uma barbearia — e um time de especialistas analisa sob diferentes ângulos, com honestidade, sem otimismo fácil.

Irmã do [Quorum](https://github.com/lluizllucas/quorum), que faz o mesmo para produtos digitais.

## O que é

O comitê é composto por membros fixos: Financeiro, Mercado, Operacional, Jurídico, Setor e Auditor. Cada um analisa a ideia sob sua perspectiva específica. O Maestro consolida tudo em um veredicto final de viabilidade com próximos passos concretos.

O **Setor** tem um papel especial: ele identifica o nicho específico da ideia e cria dinamicamente um especialista com experiência real naquele mercado — alguém que sabe o que os números não mostram.

O **Auditor** fala por último, depois de ler tudo, e tem permissão explícita para ser duro e apontar o que ninguém quis dizer.

## Arquivos do repositório

```
README.md
CLAUDE.md              ← para editar o projeto via Claude Code
ORQUESTRADOR.md        ← instruções completas para o Claude orquestrar o comitê
squad/
├── MAESTRO.md
├── FINANCEIRO.md
├── MERCADO.md
├── OPERACIONAL.md
├── JURIDICO.md
├── SETOR.md
└── AUDITOR.md
```

## Como montar no Claude.ai

### 1. Crie um Projeto

No [Claude.ai](https://claude.ai), clique em **Projects** e crie um novo projeto chamado **Ágora**.

### 2. Anexe os arquivos

Em **Project content**, anexe todos os `.md`:

- `ORQUESTRADOR.md`
- `squad/MAESTRO.md`
- `squad/FINANCEIRO.md`
- `squad/MERCADO.md`
- `squad/OPERACIONAL.md`
- `squad/JURIDICO.md`
- `squad/SETOR.md`
- `squad/AUDITOR.md`

### 3. Configure a instrução do projeto

Em **Project instructions**:

> Leia o arquivo ORQUESTRADOR.md e siga as instruções.

### 4. Pronto

Abra uma conversa no projeto e apresente sua ideia.

## Como usar

**Análise completa:** apresente sua ideia em linguagem natural. Inclua a localização se for relevante.

```
Quero comprar uma impressora 3D e vender produtos personalizados online.
Estou em Curitiba, PR.
```

```
Tenho vontade de abrir uma empresa de limpeza, montagem e manutenção de PCs
para pessoa física e pequenas empresas. Sou de São Paulo, zona leste.
```

O comitê executa todas as fases e entrega o relatório final diretamente no chat.

**Consulta direta:** após o relatório, faça perguntas a membros específicos.

```
FINANCEIRO, como ficaria o ponto de equilíbrio se eu começar em casa?
```

```
AUDITOR, o que mais te preocupa nessa ideia?
```

## Especialistas de setor dinâmicos

Quando o Setor cria um especialista (ex: `VENDEDOR_MARKETPLACE.md`), o conteúdo aparece na resposta do Setor. Salve esse conteúdo como `.md` e anexe ao projeto para reutilizar nas próximas sessões.

## Diferença entre Ágora e Quorum

| | Quorum | Ágora |
|---|---|---|
| Foco | Produtos digitais e software | Negócios físicos e operacionais |
| Membros | Dev, Infra, Arquiteto, DevOps, Comercial | Financeiro, Mercado, Operacional, Jurídico |
| Localização | Geralmente irrelevante | Frequentemente crítica |
| Output | Briefing para o Atelier (time de dev) | Relatório de viabilidade com próximos passos |
