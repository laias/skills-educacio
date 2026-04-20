# Guia de la Sessió 2 — El context ho és tot
## Formació IA per a docents | INS Maria Aurèlia Capmany
### 100 minuts

---

## Idea central

La mateixa IA, el mateix model, respon de manera radicalment diferent segons com li dones
el context. No és màgia — és arquitectura. I tu pots controlar-la.

**Els tres mecanismes:**
1. **Dins el prompt** — el context que escrius al missatge
2. **System prompt** — instruccions permanents que defineixen el rol i les regles
3. **Documents adjunts** — la IA llegeix els teus materials i els usa com a base

**Els tres casos d'ús que ho demostren:**
- Situació d'aprenentatge
- Rúbrica i base d'orientació
- Presentació (cas avançat: combina els tres mecanismes + pipeline NotebookLM)

---

## Arc de la sessió

### BLOC 1 — El problema (15 min)

**Objectiu**: crear el contrast que fa visible per què importa el context.

Demostració en viu — el mateix prompt, dos resultats:

```
PROMPT SENSE CONTEXT:
"Crea una situació d'aprenentatge sobre el canvi climàtic."

PROMPT AMB CONTEXT:
"Actues com a expert en currículum de Catalunya.
Crea una SA sobre el canvi climàtic per a 3r d'ESO, matèria de Biologia,
4 sessions, grup de 26 alumnes. Segueix l'estructura del Decret 175/2022.
El producte final ha de ser presentable a les famílies."
```

Mostra els dos resultats en paral·lel. No cal explicar res: es veu.

Pregunta al grup: *"On viu el context? On el podem posar?"*
→ Resposta: en tres llocs. Passa al Bloc 2.

---

### BLOC 2 — Els tres mecanismes (40 min)

**Estructura**: 10 min demostració + 3 min prova individual per mecanisme.

#### Mecanisme 1 — System prompt (10+3 min)

Qui és la IA, com parla, quines regles segueix. El "personatge" persistent.

Demostració:
1. Obre Claude sense cap projecte → pregunta qualsevol cosa pedagògica
2. Crea un projecte amb el system prompt de la Plantilla SA
3. Fes la mateixa pregunta → contrast immediat

Prova individual: cada docent escriu una línia de system prompt per al seu assistent.
Ex: *"Ets un assistent de [matèria] per a [curs]. Sempre proposes activitats actives."*

#### Mecanisme 2 — Megaprompt (10+3 min)

La instrucció rica: tot el context pedagògic dins un sol prompt.

Demostració: usa la Plantilla SA amb els claudàtors omplerts en viu amb dades reals
(matèria i curs invitats del grup). Mostra com el resultat segueix la plantilla oficial
del Departament.

Prova individual: cada docent omple 2-3 claudàtors de la plantilla que li interessa.

#### Mecanisme 3 — Document adjunt (10+3 min)

La IA llegeix els teus materials. Tres variants en ordre creixent de complexitat:

**Variant A — Document únic**
Puja el teu currículum (PDF del DOGC) o la teva programació.
La IA l'usa com a base sense que li hagis d'explicar res.

**Variant B — NotebookLM + exportació**
Carregues apunts o documents al NotebookLM → fas preguntes →
exportes el xat en Markdown (amb Kortex o demanant-li que respongui en markdown) →
enganxes el .md com a document adjunt al prompt de generació.

**Variant C — Captura d'estètica** *(per al cas d'ús presentació)*
Fas una captura d'una plantilla de Canva o Envato →
l'adjuntes a Claude o Gemini →
la IA extreu l'arquitectura visual i la replica amb el teu contingut.

> 💡 **Moment clau per projectar**: "El document canvia el que la IA sap.
> El system prompt canvia qui és la IA. El megaprompt canvia el que li demanes.
> Pots combinar els tres."

---

### BLOC 3 — Empaquetar-ho (30 min)

**Objectiu**: que cada docent configuri el seu primer assistent persistent.

Els tres mecanismes combinats → tres plataformes on es queda guardat per reutilitzar.

#### Demostració: el pipeline complet de presentació (10 min)

Cas d'ús que combina els tres mecanismes alhora — el més potent per mostrar.

```
PAS 1 — NotebookLM
Carregues els teus apunts del tema → demanes un resum estructurat →
exportes en Markdown

PAS 2 — Defineix la teva presentació
Omples la plantilla: quantes slides, de quin tipus, quin layout,
quina estètica (pots copiar-la d'una plantilla de Canva)

PAS 3 — Generes
Envies el prompt complet (system + megaprompt + markdown de contingut)
a Gemini, Claude o Canva IA → presentació amb el teu contingut
i la teva estètica
```

Projecció en viu: agafa una plantilla de Canva qualsevol → fes la captura →
adjunta-la a Claude → pregunta: *"Analitza l'estètica d'aquesta plantilla."*
→ mostra com la IA descriu colors, layout i estil visual.

#### Pràctica individual (20 min)

Cada docent configura un assistent a la plataforma que prefereixi:

| Plataforma | On va el system prompt | On van els documents |
|---|---|---|
| Claude | Project Instructions | Project Knowledge |
| Gemini | Instruccions del Gem | Coneixement del Gem |
| ChatGPT | Instructions del GPT | Knowledge del GPT |

Suport mentre practiquen: circula, ajuda amb els claudàtors, resol bloquejos.

---

### TANCAMENT (15 min)

**Posada en comú** (8 min):
- Una cosa que cadascú s'endú
- Una pregunta que li ha quedat oberta

**Recursos per continuar** (5 min):
- URL del Gist amb totes les plantilles
- Recordatori: els dos documents que cal pujar a cada assistent
  (guia IA + plantilla oficial SA)
- Extensió Kortex per a NotebookLM (per als que vulguin aprofundir)

**Propera sessió** (2 min): avanç del que farem a la Sessió 3.

---

## Materials necessaris

| Material | Format | On és |
|---|---|---|
| Plantilles SA + Rúbrica + Presentació | `.md` | GitHub / Gist |
| Fitxa: convertir SA a markdown | `.md` | GitHub / Gist |
| Fitxa: prompt per fer prompts | `.md` | GitHub / Gist |
| Fitxa: pipeline de presentació | `.md` | GitHub / Gist |
| Plantilla oficial SA Departament | `.md` | GitHub / Gist |
| Guia IA per a SA Catalunya | `.md` | GitHub / Gist |

## Preparació tècnica prèvia

- [ ] Projector connectat i provat
- [ ] Claude, Gemini i ChatGPT oberts en pestanyes
- [ ] NotebookLM obert amb un notebook de prova amb 2-3 documents carregats
- [ ] Kortex instal·lat al Chrome del portàtil
- [ ] Una plantilla de Canva o Envato oberta per a la demo d'estètica
- [ ] URL del Gist preparada per projectar al tancament

---

*Sessió 2 — Formació IA per a docents | INS Maria Aurèlia Capmany*
