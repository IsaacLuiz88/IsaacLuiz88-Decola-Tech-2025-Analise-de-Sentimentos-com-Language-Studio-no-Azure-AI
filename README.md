# IsaacLuiz88-Decola-Tech-2025-Analise-de-Sentimentos-com-Language-Studio-no-Azure-AI
Project idealizated to Decola Tech 2025 Análise de Sentimentos com Language Studio no Azure AI

## Descrição do Projeto
Este projeto demonstra a análise de sentimentos utilizando o Azure AI Language Studio para avaliar textos com diferentes cargas emocionais (positivo, neutro e negativo). Os resultados mostram a eficácia da ferramenta em identificar nuances de sentimentos em avaliações de hotelaria.

## Análises Realizadas

### 1. Texto Positivo
**Conteúdo analisado:**

"A nossa estadia no hotel foi excepcional e superou todas as expectativas..."

**Resultados detalhados:**
```json
{
  "sentiment": "positive",
  "confidenceScores": {
    "positive": 0.97,
    "neutral": 0.03,
    "negative": 0.00
  },
  "sentences": [
    {
      "text": "A nossa estadia no hotel foi excepcional e superou todas as expectativas.",
      "sentiment": "positive",
      "confidenceScores": {
        "positive": 0.97,
        "neutral": 0.03,
        "negative": 0.00
      }
    },
    {
      "text": "Desde o momento da chegada, fomos recebidos com um atendimento caloroso e profissional.",
      "sentiment": "positive",
      "confidenceScores": {
        "positive": 0.97,
        "neutral": 0.03,
        "negative": 0.00
      }
    }
  ],
  "keyPhrases": [
    "estadia no hotel",
    "atendimento caloroso",
    "equipe do hotel",
    "quarto impecável",
    "boa noite de sono",
    "localização do hotel",
    "restaurante do hotel"
  ]
}
```

### 2. Texto Neutro
**Conteúdo analisado:**

"A estadia no hotel foi adequada, mas não se destacou em nenhum aspecto..."

**Resultados detalhados:**
```json
{
  "sentiment": "neutral",
  "confidenceScores": {
    "positive": 0.445,
    "neutral": 0.555,
    "negative": 0.00
  },
  "sentences": [
    {
      "text": "A estadia no hotel foi adequada, mas não se destacou em nenhum aspecto.",
      "sentiment": "neutral",
      "confidenceScores": {
        "positive": 0.10,
        "neutral": 0.89,
        "negative": 0.01
      }
    },
    {
      "text": "A localização era conveniente, ficando próxima a alguns pontos turísticos...",
      "sentiment": "positive",
      "confidenceScores": {
        "positive": 1.00,
        "neutral": 0.00,
        "negative": 0.00
      }
    }
  ],
  "keyPhrases": [
    "estadia no hotel",
    "localização conveniente",
    "quarto em condições aceitáveis",
    "atendimento suficiente",
    "café da manhã razoável"
  ]
}
```
### 3. Texto Negativo
**Conteúdo analisado:**

"Infelizmente, a nossa experiência no hotel foi bem abaixo das expectativas..."

**Resultados detalhados:**
```json
{
  "sentiment": "negative",
  "confidenceScores": {
    "positive": 0.01,
    "neutral": 0.00,
    "negative": 0.99
  },
  "sentences": [
    {
      "text": "Infelizmente, a nossa experiência no hotel foi bem abaixo das expectativas.",
      "sentiment": "negative",
      "confidenceScores": {
        "positive": 0.00,
        "neutral": 0.00,
        "negative": 1.00
      }
    },
    {
      "text": "O atendimento na recepção foi impessoal e pouco acolhedor.",
      "sentiment": "negative",
      "confidenceScores": {
        "positive": 0.02,
        "neutral": 0.00,
        "negative": 0.98
      }
    }
  ],
  "keyPhrases": [
    "experiência no hotel",
    "atendimento na recepção",
    "quarto longe de ser ideal",
    "cama desconfortável",
    "isolamento acústico péssimo",
    "café da manhã decepcionante"
  ]
}
```

Insights e Observações
Precisão na Detecção
✔️ O serviço identificou corretamente os sentimentos predominantes em cada texto
✔️ Para o texto neutro, houve variação entre frases, mostrando sensibilidade a nuances

Frases-Chave
🔑 As frases extraídas capturaram os aspectos mais relevantes de cada avaliação
🔍 No texto positivo: destacou confortos e qualidade
⚠️ No negativo: focou nos problemas relatados

Confiança nas Análises
📊 Textos claros (positivo/negativo) tiveram scores de confiança acima de 95%
🔄 O texto neutro apresentou maior variação entre frases

Aplicações Práticas
🏨 Sistema poderia ser usado para monitorar avaliações de hóteis automaticamente
🚨 Identificação rápida de problemas críticos (como no texto negativo)
📈 Análise de pontos fortes para campanhas de marketing

## Como Reproduzir a Análise
Acesse o Azure Language Studio
Selecione "Análise de Sentimentos"
Cole seu texto na área de entrada
Clique em "Executar" para ver os resultados

## Observação: Os screenshots das análises estão disponíveis na pasta Results/Screenshots deste repositório.