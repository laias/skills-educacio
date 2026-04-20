# El prompt per fer prompts
## Quan no trobes la plantilla que necessites, crea-la tu

> Aquesta fitxa et dona una plantilla per demanar-li a la IA que et construeixi
> un prompt personalitzat per a qualsevol tasca docent.
> No cal saber prompt engineering — n'hi ha prou amb respondre sis preguntes.

---

## La plantilla

Còpia, omple els claudàtors i enganxa-la a qualsevol assistent:

```
Ets un expert en prompt engineering per a usos educatius.

Necessito un prompt que serveixi per a la tasca següent:

TASCA: [Descriu què vols que faci la IA. Sigues concret.
        Ex: "Generar preguntes de comprensió lectora per a un text donat"
        Ex: "Crear un pla de recuperació personalitzat per a un alumne"
        Ex: "Resumir un article científic per a alumnes de 4t d'ESO"]

ROL DE LA IA: [Qui ha de ser la IA mentre fa la tasca?
               Ex: "Un professor de llengua experimentat"
               Ex: "Un orientador educatiu"]

QUI L'USARÀ: [Jo, el docent / L'alumnat directament]

CONTEXT HABITUAL: [Quina informació tindrà disponible qui usa el prompt?
                   Ex: "Tindrà el text de l'article per enganxar"
                   Ex: "Tindrà les notes de l'alumne i la matèria"]

FORMAT DE SORTIDA: [Com vols que respongui la IA?
                    Ex: "Una llista de 5 preguntes, de menys a més difícil"
                    Ex: "Una taula amb columnes: Objectiu / Activitat / Temps"]

RESTRICCIONS: [Què NO ha de fer la IA?
               Ex: "No ha d'inventar contingut que no estigui al text"
               Ex: "No ha d'usar vocabulari tècnic que l'alumnat no entengui"
               Ex: "No ha de superar les 200 paraules de resposta"]

Genera el prompt. Ha de ser directament usable — que jo pugui copiar-lo
i enganxar-lo sense modificar res, i que ja funcioni bé.
```

---

## Exemple complet — com quedaria omplert

```
Ets un expert en prompt engineering per a usos educatius.

Necessito un prompt que serveixi per a la tasca següent:

TASCA: Generar exercicis de gramàtica a partir d'un text que el docent enganxa.

ROL DE LA IA: Un professor de llengua catalana amb experiència en secundària.

QUI L'USARÀ: Jo, el docent, per preparar fitxes d'exercicis.

CONTEXT HABITUAL: Tindrà un fragment de text d'entre 100 i 300 paraules.
Coneixerà el curs (entre 1r i 4t d'ESO) i l'aspecte gramatical que vol treballar.

FORMAT DE SORTIDA: Cinc exercicis variats (identificació, transformació, creació),
amb la solució al final en un bloc separat.

RESTRICCIONS: Els exercicis han de partir exclusivament del text donat.
No ha d'inventar oracions externes. El nivell de dificultat ha d'augmentar
progressivament de l'exercici 1 al 5.

Genera el prompt. Ha de ser directament usable — que jo pugui copiar-lo
i enganxar-lo sense modificar res, i que ja funcioni bé.
```

---

## Quan usar aquesta fitxa

| Situació | Fes servir la fitxa |
|---|---|
| Les tres plantilles principals no cobreixen el que necessites | ✓ |
| Vols un prompt molt específic per a la teva matèria | ✓ |
| Vols adaptar una plantilla existent a un context diferent | ✓ |
| La IA no entén bé el que li demanes i vols millorar el prompt | ✓ |

---

## Consell — el loop de millora

Un cop tens el prompt generat, prova'l immediatament:

```
1. Copia el prompt que t'ha generat la IA
2. Obre una nova conversa
3. Enganxa'l i prova'l amb un exemple real
4. Si el resultat no és el que esperaves, torna a la plantilla
   i ajusta la restricció o el format de sortida
```

Normalment amb 1-2 iteracions el prompt queda afinat.

---

## La regla d'or

> Com més concret siguis a **TASCA** i **FORMAT DE SORTIDA**,
> millor serà el prompt que obtindràs.
>
> La vaguetat entra, la vaguetat surt.

---

*Materials de la Sessió 2 — Formació IA per a docents | INS Maria Aurèlia Capmany*
