# Agent Cards — Time Betinho Showcase

> Visualizacao interativa do Time Betinho em formato de trading cards
> Inicio: 27/Mar/2026

---

## Conceito

Showcase interativo que apresenta o Time Betinho como um universo de agentes estilo trading cards (Magic: The Gathering). Grafo animado tipo constelacao com cards detalhados para cada agente.

## Experiencia

1. **Tela inicial:** Grafo "constelacao" com nos pulsando, particulas fluindo entre conexoes
2. **Mouse over:** Destaca conexoes, mostra nome + tagline
3. **Click:** Card estilo MTG abre com animacao (arte AI, habilidades, stats)
4. **Multilíngue:** Toggle EN / ES / PT-BR
5. **Responsivo:** Desktop + mobile

## Hierarquia

```
👑 JP — The Boss (Legendary Boss)
    └── 🎭 Betinho — The Maestro (Legendary Agent)
            ├── Consulta (11 agentes)
            ├── Compostos (2 agentes)
            ├── Producao (5 agentes)
            ├── Especializados (9 agentes)
            └── Manutencao (1 agente)
```

## Cards — Nomes e Categorias

### The Boss
| Card | Nome | Tipo | Raridade |
|---|---|---|---|
| JP | **The Boss** | Legendary Boss — Head of Marketing | Mythic |

### The Maestro
| Card | Nome | Tipo | Raridade |
|---|---|---|---|
| Betinho | **The Maestro** | Legendary Agent — Orchestrator | Legendary |

### Consulta
| Card | Nome | Tipo | Raridade |
|---|---|---|---|
| Slack | **Echo** | Agent — Listener | Common |
| Gmail | **Postman** | Agent — Messenger | Common |
| Calendar | **Clockwork** | Agent — Timekeeper | Common |
| Drive | **Vault** | Agent — Archivist | Common |
| Sheets | **Grid** | Agent — Analyst | Common |
| Docs | **Scribe** | Agent — Reader | Common |
| Jira | **Tracker** | Agent — Hunter | Common |
| Confluence | **Oracle** | Agent — Sage | Common |
| GitHub | **Keeper** | Agent — Guardian | Common |
| Afiliados | **Scout** | Agent — Watcher | Uncommon |
| Power BI | **Lens** | Agent — Seer | Uncommon |

### Compostos
| Card | Nome | Tipo | Raridade |
|---|---|---|---|
| Bom Dia | **Sentinel** | Compound Agent — Commander | Rare |
| Dados | **Nexus** | Compound Agent — Strategist | Rare |

### Producao
| Card | Nome | Tipo | Raridade |
|---|---|---|---|
| Tradutor | **Polyglot** | Production Agent — Linguist | Uncommon |
| HTML | **Painter** | Production Agent — Artist | Common |
| PDF | **Press** | Production Agent — Printer | Common |
| Pipeline | **Forge** | Production Agent — Factory | Uncommon |
| Video Onboarding | **Detective** | Production Agent — Investigator | Uncommon |

### Especializados
| Card | Nome | Tipo | Raridade |
|---|---|---|---|
| Lawyer | **Judge** | Specialist — Jurist | Rare |
| Analise Jira | **Surgeon** | Specialist — Analyst | Uncommon |
| Prep Reuniao | **Strategist** | Specialist — Advisor | Uncommon |
| Monitor Confluence | **Watchman** | Specialist — Observer | Common |
| Financeiro | **Treasurer** | Specialist — Accountant | Uncommon |
| RH | **Recruiter** | Specialist — Headhunter | Uncommon |
| Podcast | **Director** | Specialist — Producer | Common |
| Docx | **Printer** | Specialist — Formatter | Common |

### Manutencao
| Card | Nome | Tipo | Raridade |
|---|---|---|---|
| Bibliotecario | **Librarian** | Autonomous Agent — Curator | Rare |

## Tecnologia

- HTML + Canvas/WebGL (arquivo unico standalone)
- D3.js force-directed graph para o grafo
- CSS animations para cards
- i18n para 3 idiomas
- Deploy: GitHub Pages

## Estrutura

```
AgentCards/
├── README.md          ← este arquivo
├── Md/
│   └── card-specs.md  ← specs completas, prompts AI, taglines 3 idiomas
├── Assets/
│   ├── Cards/         ← imagens dos 29 cards + card back (30 arquivos)
│   ├── Icons/         ← icones de categoria e UI
│   └── Graph/         ← assets do grafo (particulas, backgrounds)
└── index.html         ← showcase (quando construido)
```

## Status

- [x] Conceito definido (27/Mar/2026)
- [x] Nomes e categorias de todos os agentes
- [x] Taglines e habilidades detalhadas por card (29 agentes + JP)
- [x] Prompts para geracao de arte AI (30 prompts + card back)
- [x] Traducoes das taglines (EN/ES/PT-BR)
- [x] Estrutura de pastas para imagens
- [ ] Gerar artes dos cards (usar prompts em Md/card-specs.md)
- [ ] Construir grafo interativo (HTML/JS/Canvas)
- [ ] Integrar cards no grafo
- [ ] Multilíngue completo (EN/ES/PT)
- [ ] Deploy GitHub Pages
