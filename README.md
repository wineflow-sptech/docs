# WineFlow Docs

Documentação central do projeto **WineFlow** — sistema de monitoramento de esteiras de engarrafamento de vinho, desenvolvido como projeto acadêmico do curso de Ciência da Computação.

## Visão Geral

O WineFlow monitora em tempo real a etapa de engarrafamento em esteiras vinícolas, coletando dados de 3 sensores instalados na linha de produção:

| Sensor | Grandeza monitorada | Objetivo |
|---|---|---|
| Velocidade | Velocidade da esteira | Detectar variações que indiquem falhas mecânicas ou gargalos de produção |
| Vibração | Vibração estrutural | Identificar desalinhamentos, desgaste de componentes ou anomalias mecânicas |
| Temperatura | Temperatura do ambiente/equipamento | Monitorar condições que possam afetar o processo ou os equipamentos |

## Arquitetura do Projeto

O projeto está dividido em múltiplos repositórios, cada um responsável por uma camada:

| Repositório | Responsabilidade |
|---|---|
| `wineflow-docs` (este) | Documentação geral, arquitetura, decisões de projeto |
| `wineflow-data` | Tratamento e processamento dos dados coletados pelos sensores |
| `wineflow-infrastructure` | Infraestrutura do projeto |
| _(a definir)_ | Coleta de dados / integração com sensores |
| _(a definir)_ | API / backend |
| _(a definir)_ | Dashboard / visualização |

> Esta tabela deve ser atualizada conforme novos repositórios forem criados.

## Fluxo de Dados (alto nível)

```
Sensores (velocidade, vibração, temperatura)
        │
        ▼
 Coleta / Ingestão
        │
        ▼
 Tratamento de dados (wineflow-data)
        │
        ▼
 Armazenamento
        │
        ▼
 Visualização / Monitoramento
```

## Equipe

- Victor Massaini Santos

## Status

🚧 Projeto em desenvolvimento acadêmico — documentação em construção.
