# Sound-Analytics
criado para o trabalho de engenharia de dados 
#  Sound Analytics

Um Protótipo de Engenharia de Dados — Plataforma de Streaming de Música
---

## 1. Descrição do Projeto

O **SoundFlow Analytics** é um projeto de a uma plataforma de streaming de música, com foco na coleta, processamento e análise de dados em tempo real e em batch.

### Problema
A plataforma enfrenta dificuldades para:
- Analisar o comportamento dos usuários
- Processar eventos em tempo real
- Gerar insights confiáveis para tomada de decisão

## Objetivos
- Construir um pipeline de dados completo (batch + streaming)
- Permitir análises em tempo real
- Suportar dashboards analíticos

Stakeholders
- Marketing → campanhas e engajamento
- Produto → recomendação de músicas
- Executivos → métricas e decisões estratégicas
- Engenharia → monitoramento do sistema


2. Definição e Classificação dos Dados
🔹 Dados Operacionais (Batch)
| Fonte | Tipo | Formato | Frequência |
|------|------|--------|-----------|
| Usuários | Relacional | CSV/SQL | Diário |
| Músicas | Relacional | CSV | Diário |
| Assinaturas | Transacional | SQL | Diário |

---
Dados de Streaming
| Fonte | Tipo | Formato | Frequência |
|------|------|--------|-----------|
| Plays de músicas | Evento | JSON | Tempo real |
| Cliques | Evento | JSON | Tempo real |
| Logs do sistema | Log | JSON | Tempo real |

---

###  Exemplo de Evento
```json
{
  "user_id": 123,
  "music_id": 987,
  "timestamp": "2026-04-09T10:00:00",
  "action": "play"
}
