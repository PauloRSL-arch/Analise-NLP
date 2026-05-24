# Relatório de Análise NLP (Recuperação da Informação)

**Repositório GitHub:** [https://github.com/usuario/prova_sri](https://github.com/usuario/prova_sri)

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

*Nota: Os arquivos completos (.csv) gerados em cada etapa (documentos_sentenciados, pos_tags, entidades) encontram-se preservados na pasta `data/` dentro do repositório da prova.*
