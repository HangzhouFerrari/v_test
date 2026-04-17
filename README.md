# StudyDeck — Bestandsstructuur

```
/
├── index.html                        ← Startpagina (setbeheer)
├── set.html                          ← Universele leerpagina
└── sets/
    ├── biologie-celbiologie.vset
    └── ...
```

## URL-structuur

```
https://jouwsite.com/set.html?set=biologie-celbiologie
```

StudyDeck laadt dan `sets/biologie-celbiologie.vset`.

## .vset bestanden

`.vset` bestanden zijn versleuteld — niet leesbaar als plain JSON.
Aanmaken via de **⬇ .vset** knop op de startpagina, dan in de `sets/` map zetten.

## Workflow

1. Open `index.html` → **Nieuwe set** → vul in → **Aanmaken**
2. Klik **⬇ .vset** op de setkaart
3. Zet het bestand in de `sets/` map op je server
4. Deel de link: `set.html?set=jouw-set-naam`

## Fallback

Als het `.vset` bestand niet op de server staat, valt de app terug
op lokaal opgeslagen sets (localStorage van `index.html`).
