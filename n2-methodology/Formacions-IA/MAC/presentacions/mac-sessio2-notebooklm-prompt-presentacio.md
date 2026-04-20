# NotebookLM — Prompt per generar la presentació de la Sessió 2

## Per a qui és aquest document

Per a la formadora (preparar materials) i per al professorat del MAC (plantilla reutilitzable per a futures sessions).

---

## Pas 1 — Documents que cal pujar a NotebookLM

Puja aquests fitxers com a fonts del notebook abans de fer el prompt:

- `mac-sessio2-prompts.md` — les tres plantilles principals (SA, rúbrica, presentació)
- `mac-sessio2-fitxa-prompt-per-fer-prompts.md` — com construir prompts nous
- `mac-sessio2-guia-facilitador.md` — guia de la sessió
- Opcional: la programació d'aula o temari del centre

---

## Pas 2 — L'outline de la presentació

Estructura de 13 slides per a una sessió de 100 minuts:

| # | Títol | Contingut clau |
|---|---|---|
| 1 | El context ho és tot | Portada. Subtítol: Com fer que la IA et conegui i treballi per a tu |
| 2 | On som i on anem | Recordatori Sessió 1 + tres blocs d'avui: system prompt / plantilles / pràctica |
| 3 | Per què la IA no et recorda | Cada conversa comença de zero. El system prompt com a solució |
| 4 | El system prompt — la teva veu permanent | Anatomia: qui ets, to, restriccions, currículum. Metàfora: briefing a un col·laborador nou |
| 5 | Tres plataformes, un mateix principi | Claude Projects / Gemini Gems / ChatGPT GPTs. Taula comparativa |
| 6 | Les tres plantilles | SA / Rúbrica / Presentació — per a qui és, quan s'usa, què necessita |
| 7 | Plantilla 1 — Situació d'Aprenentatge | Fases 0-1-2. Punt crític: verificar codis Decret 175/2022 |
| 8 | Plantilla 2 — Rúbrica | Conductes observables, no adjectius genèrics |
| 9 | Plantilla 3 — Presentació | Ganxo / cos / interacció / missatge final |
| 10 | NotebookLM — quan la IA llegeix els teus documents | Pujar programació, temari, criteris. Diferència respecte a Claude/Gemini |
| 11 | Ara ho feu vosaltres | Pràctica 25 min: configurar l'assistent propi per parelles de departament |
| 12 | El loop de millora | Com iterar. Regla d'or: concreció a TASCA i FORMAT DE SORTIDA |
| 13 | Propera sessió — Produir | Sessió 3: deconstruir i remixar una SA real. Tasca opcional |

---

## Pas 3 — El prompt per a NotebookLM

> Construït amb la **Plantilla 3 — Presentació** dels materials de la Sessió 2.
> Copia aquest bloc i enganxa'l al xat de NotebookLM un cop tinguis els documents carregats.

```
Actua com a expert en comunicació educativa i disseny de presentacions.

CONTEXT:
- Qui presenta: La formadora davant docents de secundària
- Tema de la presentació: El context ho és tot — com fer que la IA et conegui
  i treballi per a tu (system prompts, plantilles SA/rúbrica/presentació, pràctica)
- Audiència: Docents de secundària de l'INS Maria Aurèlia Capmany que ja han
  fet la Sessió 1 (LLMs, tokens, al·lucinacions, RAG, agents)
- Durada: 100 minuts de sessió, presentació de suport (no es llegeix, acompanya)
- Objectiu principal: Que cada docent surti amb el seu assistent permanent configurat
  i sabent usar les tres plantilles
- Recursos disponibles: Canva per al disseny final, documents de la sessió com a base
- Condicionant: Les slides no poden ser text dens — han de ser ganxos visuals
  i recordatoris, no guions. Les explicacions van a les notes del presentador.

TASCA:
A partir dels documents que has llegit, dissenya l'estructura completa d'una presentació
de 13 slides sobre aquest tema que:
1. Comenci amb un ganxo que capti l'atenció en els primers 30 segons.
2. Segueixi l'outline següent (títols i ordre fixos, tu omplis el contingut):
   1. El context ho és tot
   2. On som i on anem
   3. Per què la IA no et recorda
   4. El system prompt — la teva veu permanent
   5. Tres plataformes, un mateix principi
   6. Les tres plantilles
   7. Plantilla 1 — Situació d'Aprenentatge
   8. Plantilla 2 — Rúbrica
   9. Plantilla 3 — Presentació
   10. NotebookLM — quan la IA llegeix els teus documents
   11. Ara ho feu vosaltres
   12. El loop de millora
   13. Propera sessió — Produir
3. Inclogui a la slide 11 un moment d'interacció real (instrucció concreta per
   al bloc de pràctica de 25 minuts).
4. Acabi amb un missatge únic a la slide 13 que els docents puguin repetir
   hores després.

FORMAT DE SORTIDA:
Per a cada slide:
- Número i títol
- Contingut de la slide (màx. 3 punts, concisos — res que calgui llegir)
- Notes del presentador (2-4 frases per guiar la facilitació en veu alta)
- Suggeriment visual si escau (icona, metàfora visual, diagrama simple)

Afegeix al final:
- 3 preguntes que els docents podrien fer i com respondre-les.
- Un criteri d'autoavaluació: "La sessió ha funcionat si..."

To: proper, directe, no condescendent. Llengua: català.
```

---

## Consell d'ús

Si NotebookLM genera alguna slide amb contingut genèric o inexacte, afegeix al prompt:

> "Per a la slide [X], basa't específicament en [cita el document i la secció concreta]."

La qualitat millora molt quan li indiques exactament d'on ha d'extreure la informació.

---

*Materials de la Sessió 2 — Formació IA per a docents | INS Maria Aurèlia Capmany*
