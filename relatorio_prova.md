# Relatório de Análise NLP (Recuperação da Informação)

**Repositório GitHub:** [https://github.com/PauloRSL-arch/Analise-NLP](https://github.com/PauloRSL-arch/Analise-NLP)

## 1. Descrição do Texto Utilizado
O corpus utilizado na análise consiste em um conjunto de 35 documentos variados, englobando notícias curtas sobre o Brasil, eventos históricos, informações geográficas (como a Floresta Amazônica e o Rio Amazonas) e personalidades importantes. Os documentos variam entre 1 a 3 sentenças curtas e possuem tamanho compatível com o limite de 512 tokens. Os textos foram estruturados em formato `.csv` contendo as colunas `id` e `documento`.

## 2. Exemplo de POS Tagging
Abaixo, a extração das tags (Part-of-Speech) de uma das sentenças do corpus:

**Sentença Original:** "Machado de Assis é amplamente considerado o maior escritor da literatura brasileira."
  
**POS Tagging:**
- Machado (PROPN)
- de (ADP)
- Assis (PROPN)
- é (AUX)
- amplamente (ADV)
- considerado (VERB)
- o (DET)
- maior (ADJ)
- escritor (NOUN)
- da (ADP)
- literatura (NOUN)
- brasileira (ADJ)

## 3. Exemplo de NER (Reconhecimento de Entidades Nomeadas)
Extração das entidades nomeadas de uma sentença selecionada do texto:

**Sentença Original:** "O ministro da Defesa, Nelson Jobim, informou no fim da noite desta terça-feira que a economista Solange Vieira será a nova presidente da Agência Nacional de Aviação Civil."

**Entidades Identificadas:**
- Defesa (ORG)
- Nelson Jobim (PER)
- Solange Vieira (PER)
- Agência Nacional de Aviação Civil (ORG)

## 4. Gráficos e Tabelas da Análise de Dados
Abaixo estão os resultados sumarizados gerados após a execução da limpeza, POS e análise estatística sobre os documentos do corpus.

### Tabela de Frequência de Tokens (Top 10)
| Palavra     | Frequência | POS Dominante |
|-------------|------------|---------------|
| Brasil      | 14         | PROPN         |
| mundo       | 8          | NOUN          |
| São Paulo   | 7          | PROPN         |
| pessoas     | 6          | NOUN          |
| anos        | 5          | NOUN          |
| maior       | 5          | ADJ           |
| futebol     | 4          | NOUN          |
| governo     | 4          | NOUN          |
| ataques     | 4          | NOUN          |
| janeiro     | 3          | NOUN          |

### Distribuição de Entidades (NER)
| Tipo de Entidade | Quantidade Total | Exemplos Frequentes |
|------------------|------------------|---------------------|
| LOC (Localidades)| 42               | Brasil, São Paulo, Rio de Janeiro, Líbano |
| PER (Pessoas)    | 25               | Nelson Jobim, Machado de Assis, Pelé |
| ORG (Organizações)| 19              | ONU, Polícia Federal, Seleção Brasileira |
| MISC (Diversos)  | 8                | Copa do Mundo, Bossa Nova |

### Gráficos Gerados pela Análise de Dados

#### Estatísticas palavras e tokens em janelas por documento
![Gráfico 1](data/Analise%20de%20dados/Estatísticas%20palavras%20e%20tokens%20em%20janelas%20por%20documento.png)

#### Estatísticas palavras e tokens por janela
![Gráfico 2](data/Analise%20de%20dados/Estatísticas%20palavras%20e%20tokens%20por%20janela.png)

#### Qtd de documentos por quantidade de entidades
![Gráfico 3](data/Analise%20de%20dados/Qtd%20de%20documentos%20por%20quantidade%20de%20entidades.png)

#### Qtd de documentos por quantidade de locucoes verbais
![Gráfico 4](data/Analise%20de%20dados/Qtd%20de%20documentos%20por%20quantidade%20de%20locucoes%20verbais.png)

#### Qtd de documentos por quantidade de palavras sem stopWords
![Gráfico 5](data/Analise%20de%20dados/Qtd%20de%20documentos%20por%20quantidade%20de%20palavras%20sem%20stopWords.png)

#### Qtd de documentos por quantidade de palavras
![Gráfico 6](data/Analise%20de%20dados/Qtd%20de%20documentos%20por%20quantidade%20de%20palavras.png)

#### Qtd de documentos por quantidade de sentença
![Gráfico 7](data/Analise%20de%20dados/Qtd%20de%20documentos%20por%20quantidade%20de%20sentença.png)

#### Qtd de documentos por quantidade de substativos
![Gráfico 8](data/Analise%20de%20dados/Qtd%20de%20documentos%20por%20quantidade%20de%20substativos.png)

#### Qtd de documentos por quantidade de tokens
![Gráfico 9](data/Analise%20de%20dados/Qtd%20de%20documentos%20por%20quantidade%20de%20tokens.png)

#### Qtd de documentos por quantidade de vebos e aux
![Gráfico 10](data/Analise%20de%20dados/Qtd%20de%20documentos%20por%20quantidade%20de%20vebos%20e%20aux.png)

#### Qtd de documentos por quantidade de verbos(aux) e substativos
![Gráfico 11](data/Analise%20de%20dados/Qtd%20de%20documentos%20por%20quantidade%20de%20verbos(aux)%20e%20substativos.png)

#### Qtd de documents por quantidade de verbos
![Gráfico 12](data/Analise%20de%20dados/Qtd%20de%20documents%20por%20quantidade%20de%20verbos.png)

#### Qtd de sentacas de docuemntos por quantidades de tokens
![Gráfico 13](data/Analise%20de%20dados/Qtd%20de%20sentacas%20de%20docuemntos%20por%20quantidades%20de%20tokens.png)

#### Qtd de sentecas de documentos por quantidades de verbos aux e substantivos
![Gráfico 14](data/Analise%20de%20dados/Qtd%20de%20sentecas%20de%20documentos%20por%20quantidades%20de%20verbos%20aux%20e%20substantivos.png)

#### Qtd de sentencas de documentos por quantidade de entidades
![Gráfico 15](data/Analise%20de%20dados/Qtd%20de%20sentencas%20de%20documentos%20por%20quantidade%20de%20entidades.png)

#### Quantidade de sentencas de documentos por quantidade de locucoes verbais
![Gráfico 16](data/Analise%20de%20dados/Quantidade%20de%20sentencas%20de%20documentos%20por%20quantidade%20de%20locucoes%20verbais.png)

#### Quantidade de sentencas de documentos por quantidade de verbos
![Gráfico 17](data/Analise%20de%20dados/Quantidade%20de%20sentencas%20de%20documentos%20por%20quantidade%20de%20verbos.png)

#### Quantidade de sentencas de doumentos por quantidade de substativos
![Gráfico 18](data/Analise%20de%20dados/Quantidade%20de%20sentencas%20de%20doumentos%20por%20quantidade%20de%20substativos.png)

#### Quantidade de setencas por documentos por quantidade de verbs e aux
![Gráfico 19](data/Analise%20de%20dados/Quantidade%20de%20setencas%20por%20documentos%20por%20quantidade%20de%20verbs%20e%20aux.png)

#### Tamanho dos documentos tokenizados antes de classificas
![Gráfico 20](data/Analise%20de%20dados/Tamanho%20dos%20documentos%20tokenizados%20antes%20de%20classificas.png)

#### Tamanho dos documentos tokenizados classificados
![Gráfico 21](data/Analise%20de%20dados/Tamanho%20dos%20documentos%20tokenizados%20classificados.png)

#### Qtd de sentencas de documentos por quantidade de palavras
![Gráfico 22](data/Analise%20de%20dados/qtd%20de%20sentencas%20de%20documentos%20por%20quantidade%20de%20palavras.png)

*Nota: Os arquivos completos (.csv) gerados em cada etapa (documentos_sentenciados, pos_tags, entidades) encontram-se preservados na pasta `data/` dentro do repositório da prova.*
