# Desafio DIO — Azure Speech & Language (Speech Studio + Language Studio)

Documentação dos testes práticos com **Azure AI Speech** (STT/TTS) e **Azure AI Language** (Sentiment, Key Phrases, Language Detection). Repositório organizado com prints, passos e insights para replicação.

## 🔗 Índice
- [Objetivos](#objetivos)
- [Como reproduzir](#como-reproduzir)
- [Resultados (prints)](#resultados-prints)
- [Insights](#insights)
- [Referências](#referências)

## Objetivos
- Testar **Speech-to-Text** e **Text-to-Speech** no Speech Studio.
- Testar **Sentiment**, **Key Phrases** e **Language Detection** no Language Studio.
- Registrar prints e aprendizados em GitHub.

## Como reproduzir
1. Criar recursos **Speech** e **Language** no Azure (região: Brazil South ou East US).
2. **Speech Studio**
   - STT: enviar áudio curto (10–20s).  
   - TTS: escolher voz neural pt-BR e sintetizar texto.
3. **Language Studio**
   - Sentiment: rodar textos positivo/negativo/neutro.
   - Key Phrases: rodar um parágrafo.
   - Language Detection: rodar PT/EN/ES.

## Resultados (prints)
### Speech Studio
- **STT** – ![Speech STT](images/speech-stt.png)
- **TTS** – ![Speech TTS](images/speech-tts.png)

### Language Studio
- **Sentiment**  
  Positivo – ![Positivo](images/lang-sentiment-positive.png)  
  Negativo – ![Negativo](images/lang-sentiment-negative.png)  
  Neutro – ![Neutro](images/lang-sentiment-neutral.png)
- **Key Phrases** – ![Key Phrases](images/lang-keyphrases.png)
- **Language Detection** – ![ES](images/lang-detect1.png) ![EN](images/lang-detect2.png) ![PT](images/lang-detect3.png)

## Insights
- Áudio curto e ambiente silencioso ↑ acurácia do STT.  
- Vozes neurais pt-BR no TTS têm boa naturalidade.  
- Sentiment e Key Phrases aceleram leitura de feedbacks.  
- Language Detection funcionou bem (confiança alta nos 3 idiomas).

## Referências
- https://speech.microsoft.com/  
- https://language.cognitive.azure.com/  
- https://learn.microsoft.com/azure/cognitive-services/
