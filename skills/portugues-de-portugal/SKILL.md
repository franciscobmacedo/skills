---
name: portugues-de-portugal
description: Write natural, professional European Portuguese (Portugal), never Brazilian and never text that reads as translated from English. Use for any Portuguese text meant for a reader in Portugal (reports, emails, documents for clients or public bodies, product copy, UI strings, prompts spoken to Portuguese users), and to review or fix existing Portuguese text. Also enforces plain, reader-first writing and no em dashes.
---

# Português de Portugal

Write as a Portuguese professional in Portugal would write: natural, precise, plain. The reader must never feel the text was written in Brazil, translated from English, or produced by a machine.

This covers three things, in order of importance:

1. **The language is Portuguese from Portugal.** Vocabulary, grammar, spelling and idiom.
2. **The text is written for its reader.** Someone outside your context, reading it cold.
3. **The punctuation is clean.** No em dashes.

## 1. Portuguese from Portugal

### Grammar

- **No gerúndio progressivo.** Use *estar a* + infinitive.
  - ✗ "está sendo analisado", "estamos verificando"
  - ✓ "está a ser analisado", "estamos a verificar"
  The gerúndio is fine in other uses ("Concluída a análise, verificando-se que…"), just not for an action in progress.
- **Clitics after the verb (ênclise)** in affirmative main clauses, which is where Brazilian usage differs most.
  - ✗ "Se verifica que…", "Me disseram…", "O sistema se liga…"
  - ✓ "Verifica-se que…", "Disseram-me…", "O sistema liga-se…"
  Keep proclisis where Portugal also uses it: after negation (*não se aplica*), certain adverbs (*já se sabe*, *também se verifica*), relative and subordinate clauses (*que se aplica*, *quando se verifica*) and questions with an interrogative word.
- **Future and conditional with clitics:** mesóclise exists (*far-se-á*, *dir-lhe-ia*) but sounds stiff outside legal text. Prefer a construction that avoids it ("vai ser feito", "será feito").
- **No "você"** to address the reader. In formal text use the third person without a pronoun ("Pode consultar…"), or *o senhor/a senhora*, *V. Ex.ª* in very formal letters. Between colleagues, *tu*.
- **No "a gente"** for *nós*.
- **Articles before possessives:** "o meu relatório", "a sua decisão" (Brazilian often drops the article).
- **"Ter" for existence in speech, "haver" in writing:** "há três pendentes", not "tem três pendentes".

### Vocabulary

Use the Portugal word, always:

| ✗ Brazil | ✓ Portugal |
|---|---|
| arquivo (computer file) | ficheiro |
| tela | ecrã |
| usuário | utilizador |
| equipe, time | equipa |
| contato | contacto |
| registro | registo |
| fato (facto) | facto |
| controle | controlo |
| planilha | folha de cálculo |
| celular | telemóvel |
| cadastro, cadastrar | registo, registar |
| senha | palavra-passe |
| acessar | aceder |
| deletar | apagar, eliminar |
| baixar (download) | descarregar |
| rodar (a program) | executar, correr |
| mídia | média, meios |
| trem | comboio |
| ônibus | autocarro |
| geladeira | frigorífico |
| banheiro | casa de banho |
| café da manhã | pequeno-almoço |
| xícara | chávena |
| moça, garoto | rapariga, miúdo |
| legal (cool) | fixe, óptimo, bom |
| gerenciar, gerente | gerir, gestor |
| aplicativo | aplicação |
| mouse | rato |
| site | sítio, página (or keep "site" in informal tech text) |

When unsure about a word, look it up (see *Sources*). Priberam and Infopédia mark Brazilian uses as "[Brasil]".

### Calques from English

Rewrite these in natural Portuguese:

| ✗ Calque | ✓ Portugal |
|---|---|
| endereçar (address a problem) | tratar, resolver, responder a |
| mandatório | obrigatório |
| reportar (report to) | informar, comunicar |
| performance | desempenho |
| assumir (assume) | presumir, partir do princípio |
| providenciar (provide) | fornecer, disponibilizar |
| suportar (support a feature) | admitir, permitir, apoiar |
| aplicar para (apply for) | candidatar-se a |
| em ordem a | para, a fim de |
| baseado em | com base em |
| evidências (as a count of items) | provas |
| "Figura 3 — Técnico — lista." | "Figura 3: lista de participantes vista pelo técnico." |
| X é crítico (critical = important) | X é essencial, determinante |
| endereço de e-mail | endereço de correio electrónico (formal) / e-mail (informal) |

Also watch English word order: adjective before noun ("a completa análise") and noun stacks ("o relatório de teste de aceitação de sistema"). Portuguese puts adjectives after the noun and unpacks noun stacks with prepositions.

Never use "turno" for a turn in a conversation. Use *fala*, *vez*, or rephrase.

### Spelling

Portugal uses the Acordo Ortográfico de 1990 officially ("ação", "proteção", "efetuado", "ótimo"). Many public bodies and contracts still use the pre-Acordo spelling ("acção", "protecção", "efectuado", "óptimo", "objecto", "direcção").

- **Match the reader's documents.** If you are answering a contract, a tender or a document from a município in pre-AO spelling, write in pre-AO. Otherwise use AO90.
- **Be consistent.** Never mix both in one text.
- **Always Portugal spelling where the two norms differ:** "anónimo" (not *anônimo*), "económico" (not *econômico*), "facto" (not *fato*), "registo" (not *registro*).

### Numbers, dates, names

- Dates: **dd/mm/aaaa** (29/09/2026) or "29 de Setembro de 2026" (pre-AO capitalises months; AO90: "29 de setembro").
- Time: **14h30** or 14:30.
- Decimals with a comma: **3,5 %** (space before %). Thousands with a space or a point: **30 318** or 30.318.
- Currency: **12,50 €** (symbol after, with a space).
- Capitalise institutions when they are a proper noun: *o Município*, *a Câmara Municipal de Óbidos*, *o Encarregado de Protecção de Dados*.
- Ordinals and clauses as in Portuguese legal text: *Cláusula 9.ª, n.º 4, alínea b)*.

### Titles and register

- Titles as a Portuguese document would have them. ✗ "Ficha do documento" (odd), ✓ "Identificação do documento". ✗ "Sumário executivo" (calque), ✓ "Síntese", "Resumo".
- Formal but plain. Short sentences beat long precise ones. No bureaucratic padding ("no que concerne a", "no âmbito de" repeated everywhere).

## 2. Written for the reader

The reader never saw earlier versions, your conversation, or your internal systems. Write only what is true now, as a person who never knew there was a "before".

- **Final results only.** No history, no before/after, no "was failing, now works", no failed attempts.
- **Never mention a change.** When asked to change something, change it silently. ✗ "O documento passou a ser autónomo", "agora inclui", "já não…". If the old thing had to go, it must not exist, not even by implication.
- **No disclaimers about what the text is not** or doesn't include, unless the reader would actually wonder. ✗ "Os textos propostos não fazem parte deste relatório." (It is like writing "this is not an ad for an Opel Corsa".) A negative is fine when it IS the fact being reported ("a Telnyx não grava as chamadas").
- **No internals.** No commit hashes, version codes, internal project or resource names, file paths, code, tool names that mean nothing to the reader, internal team or back-office roles. Describe the thing itself: "ambiente de ensaio separado da produção, com a mesma arquitectura", not its internal name.
- **Don't reveal what you don't need to.** In anything that could leak (reports, client documents): no URLs beyond the public address, no endpoints, no pages a user cannot open, no vulnerability lists. Security results as totals.
- **No mention of AI, agents or assistants having written or done the work.** The author is the person responsible.
- **Nothing unrelated to the reader.** Internal trials, other clients, your own test runs outside the scope: cut.
- **Every sentence clear on the first read.** If a sentence needs your context to make sense, rewrite it plainly or cut it. Unclear text is the text's fault, never the reader's.

## 3. No em dashes

Do not use the em dash (—) or the en dash (–) as punctuation. They read as machine-written and are rare in Portuguese prose.

| Instead of | Use |
|---|---|
| an aside — like this — in a sentence | commas: "um aparte, como este, na frase", or parentheses |
| a list or explanation — introduced | a colon: "três pontos: …" |
| two ideas — joined | a full stop, or a semicolon |
| a range 10–16h | "das 10h às 16h", "de 10 a 16" |

The en dash is acceptable only inside numeric ranges in tables where space is tight; in running text write the range out. Hyphens (-) stay where the language needs them ("verifica-se", "pequeno-almoço").

## Quoted text is sacred

Leave verbatim, even if it breaks these rules:

- people's spoken words in transcripts or quotes;
- quoted clauses of a contract or law;
- on-screen messages quoted as evidence;
- third-party text (show it clearly as a quote: « … » or a block quote, with the source).

## Sources

When in doubt, check. Don't guess.

- **Priberam**, dicionario.priberam.org: marks Brazilian and Portuguese uses, shows AO90 and pre-AO spellings.
- **Infopédia (Porto Editora)**, infopedia.pt: dictionary and language tools, Portugal-first.
- **Ciberdúvidas da Língua Portuguesa**, ciberduvidas.iscte-iul.pt: answers to usage questions (clitics, regência, calques).
- **Portal da Língua Portuguesa / VOP**, portaldalinguaportuguesa.org: the official spelling vocabulary.
- **FLiP**, flip.pt: grammar and style checks for European Portuguese.

## Before you deliver

Read the whole text once more and check:

- [ ] No Brazilian words, gerúndio progressivo, proclisis in affirmative main clauses, "você" or "a gente".
- [ ] No calques from English; adjectives after nouns; no noun stacks.
- [ ] Spelling consistent (AO90 or pre-AO, matching the reader), Portugal forms throughout.
- [ ] Dates, numbers, currency in Portuguese format.
- [ ] No em dashes or en dashes in running text.
- [ ] No history, change-talk, disclaimers, internals, AI mentions or unrelated content.
- [ ] Every sentence understandable by the reader, cold, on the first read.
- [ ] Quotes left verbatim.

For long documents, grep the text for the usual offenders (`—`, `–`, `está sendo`, `você`, `arquivo`, `usuário`, `tela`, `contato`, `registro`, `agora`, `já não`, `passou a`, `não faz parte`) before a full read-through.
