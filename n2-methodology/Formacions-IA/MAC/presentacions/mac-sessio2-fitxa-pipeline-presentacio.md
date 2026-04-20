# El pipeline de presentació
## Del teu contingut a la teva presentació — en tres fases

> Aquesta fitxa és el cas d'ús avançat que combina els tres mecanismes de context
> alhora: contingut propi (documents), arquitectura visual (megaprompt) i rol de la IA
> (system prompt). Dominar-la és dominar els tres mecanismes junts.

---

## Visió general del pipeline

```
FASE 1 — CONTINGUT
Els teus apunts/documents → NotebookLM → Markdown estructurat

FASE 2 — ARQUITECTURA VISUAL
Tu decideixes: nº slides · tipus · layout · estètica · imatges
(pots copiar l'estètica d'una plantilla de Canva o Envato)

FASE 3 — GENERACIÓ
Prompt complet → Gemini / Claude / Canva IA → la teva presentació
```

El poder d'aquest pipeline: **la IA executa, tu decideixes.**
El contingut és teu. L'estètica és teva. L'estructura és teva.

---

## FASE 1 — Extreu el contingut amb NotebookLM

### Opció A — Amb Kortex (si tens l'extensió instal·lada)

1. Obre NotebookLM → carrega els teus documents (apunts, PDF, Google Doc)
2. Fes preguntes per extreure el que necessites
3. Kortex → Export xat → Markdown → descarregues el `.md`

### Opció B — Sense extensió (funciona sempre)

1. Obre NotebookLM → carrega els teus documents
2. Enganxa aquest prompt al xat:

```
A partir dels documents que tens carregats, genera el contingut
per a una presentació sobre [TEMA].

Estructura la resposta en markdown amb aquest format per a cada slide:

## [Número] — [Títol de la slide]
**Missatge clau:** [Una frase. El que l'audiència ha de recordar.]
**Contingut:** [3-5 punts o 2-3 paràgrafs breus]
**Dada o cita destacada:** [Si n'hi ha una de rellevant als documents]

Genera contingut per a [X] slides. Basa't exclusivament en els
documents carregats. Si no tens prou informació per a una slide,
indica-ho explícitament.
```

3. Copia la resposta o usa l'opció "Copy" del xat de NotebookLM

---

## FASE 2 — Defineix l'arquitectura visual

Omple aquesta plantilla. Com més concret, millor el resultat.

### 2A — Estructura de la presentació

```
NOMBRE TOTAL DE SLIDES: [ex: 12]

TIPUS DE SLIDES I ORDRE:
1. Portada (1 slide)
2. Índex o mapa de continguts (1 slide)
3. Slides de contingut principal ([X] slides)
4. Slide de dada/cita destacada ([X] slides)
5. Slide de resum o conclusió (1 slide)
6. Slide de tancament / crida a l'acció (1 slide)

[Afegeix o elimina tipus segons el que necessitis]
```

### 2B — Layout per tipus de slide

```
PORTADA:
- Títol centrat gran + subtítol + autor/data
- [o] Títol a l'esquerra, imatge a la dreta ocupant el 50%

SLIDES DE CONTINGUT:
- Títol a dalt, text en dues columnes
- [o] Títol a dalt, punt a l'esquerra, imatge a la dreta
- [o] Títol gran, 3 icones o blocs en horitzontal

SLIDE DE DADA:
- Número gran al centre, text explicatiu petit sota
- [o] Cita en cos de lletra gran, autor en petit

[Descriu el layout que vols per a cada tipus]
```

### 2C — Estètica

**Opció ràpida — copia d'una plantilla existent:**

Si has trobat una plantilla a Canva, Envato o similars que t'agrada:

*Amb captura de pantalla (Claude o Gemini):*
1. Fes una captura de la plantilla
2. Adjunta-la al missatge
3. Usa aquest prompt:

```
Analitza l'estètica d'aquesta plantilla de presentació i descriu:
1. Paleta de colors: colors principals i d'accent (hex si els pots inferir)
2. Tipografia: estil dels títols (serif/sans-serif, pes, mida relativa)
   i estil del cos de text
3. Layout predominant: on es posicionen els elements clau
4. Estil gràfic general: minimalista / orgànic / geomètric / editorial / digital
5. Estil d'imatges: foto real / il·lustració plana / icones lineals / abstracte

Usaré aquesta descripció per replicar l'estètica en una nova presentació.
```

4. Copia la descripció generada → usa-la a la Fase 3

*Sense captura (descripció manual):*
```
ESTÈTICA:
- Colors principals: [ex: blau marí #1B2A4A, blanc, taronja com a accent]
- Colors d'accent: [ex: un sol color per a destacats i títols]
- Tipografia títols: [ex: sans-serif, pes bold, mida gran]
- Tipografia cos: [ex: sans-serif, pes regular, mida mitjana]
- Estil gràfic: [tria: minimalista / orgànic / geomètric / editorial / digital]
- Densitat visual: [tria: molt espai en blanc / equilibrat / dens]
```

### 2D — Imatges i il·lustracions

```
ESTIL VISUAL:
[tria un]
- Fotografies reals (professionals, sense estoc obvi)
- Il·lustracions vectorials planes (flat design)
- Icones lineals simples
- Gràfics i dades visualitzades
- Sense imatges (tipografia i color com a elements visuals principals)

TEMA DE LES IMATGES:
[ex: persones en contextos educatius / natura i medi ambient /
tecnologia abstracta / arquitectura i espais urbans]
```

---

## FASE 3 — Genera la presentació

Combina tot en un sol prompt. Enganxa a continuació el markdown de la Fase 1.

### Prompt per a Gemini / Claude

```
Ets un expert en disseny de presentacions educatives.

CONTINGUT:
A continuació trobaràs el contingut de la presentació en markdown.
Usa'l íntegrament sense inventar res que no hi sigui.

[ENGANXA AQUÍ EL MARKDOWN DE LA FASE 1]

---

ARQUITECTURA VISUAL:
Estructura: [copia el que has definit a 2A]
Layout per tipus: [copia el que has definit a 2B]
Estètica: [copia la descripció de 2C]
Imatges: [copia el que has definit a 2D]

---

TASCA:
Genera l'estructura completa de la presentació seguint:
1. L'arquitectura i el layout definits
2. L'estètica descrita
3. El contingut del markdown — sense afegir ni eliminar informació

FORMAT DE SORTIDA per a cada slide:
**Slide [N] — [Tipus] — [Títol]**
- Layout: [descripció del layout d'aquesta slide]
- Contingut visible: [text exacte que apareix a la slide]
- Notes del presentador: [allò que el presentador diu però no apareix]
- Imatge suggerida: [descripció de la imatge ideal per a aquesta slide]
- Color de fons o accent: [si difereix de l'estètica general]
```

### Prompt per a Canva IA (Magic Design)

```
Crea una presentació de [X] slides sobre [TEMA].

Audiència: [docents / alumnat de [curs] / famílies / professionals]
To: [professional i proper / formal / dinàmic i visual]

Estructura:
[copia les slides de 2A]

Estètica:
[copia la descripció de 2C — colors, tipografia, estil]

Contingut de les slides principals:
[copia els títols i missatges clau del markdown de la Fase 1 —
no cal posar tot el text, Canva el generarà]
```

---

## El flux en 15 minuts

Per practicar-ho per primer cop sense pressió:

```
00:00 — Obre NotebookLM amb 1-2 documents carregats
00:02 — Enganxa el prompt de la Fase 1 → copia la resposta
00:05 — Omple només 2A (estructura) i 2C (estètica bàsica)
00:08 — Construeix el prompt de la Fase 3 amb el que tens
00:10 — Envia a Claude o Gemini → llegeix el resultat
00:13 — Ajusta una cosa concreta i torna a generar
```

La primera vegada no serà perfecte. La segona, molt millor.

---

## Consells per treure-li el màxim

**Sobre el contingut**: NotebookLM és molt millor que qualsevol IA per extreure
contingut dels *teus* documents. No li demanis que inventi — li demanes que organitzi
el que ja tens.

**Sobre l'estètica**: menys és més a la Fase 2C. Un color d'accent, un estil gràfic,
una decisió de tipografia. Si defineixes massa coses, la IA es confon.

**Sobre la generació**: Claude és millor per a l'estructura i el text.
Gemini és millor si vols exportar directament a Google Slides.
Canva IA és millor si vols un resultat visualment acabat sense passar per un editor.

**Sobre les imatges**: cap IA genera les imatges automàticament dins la presentació.
El que obtens és la descripció de quina imatge posaria. Busques la imatge a part
(Unsplash, Pexels, o amb un generador d'imatges) i la col·loques tu.

---

*Materials de la Sessió 2 — Formació IA per a docents | INS Maria Aurèlia Capmany*
