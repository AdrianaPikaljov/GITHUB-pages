# Microsoft Project juhend — projectLibre haru

> Veebipõhine juhend Microsoft Projecti kasutamiseks: kalendrite loomine, diagrammide lugemine ja projekti haldamine.

---

## Sisukord

- [Projekti kirjeldus](#projekti-kirjeldus)
- [Muudetud failid](#muudetud-failid)
- [Lisatud funktsionaalsused](#lisatud-funktsionaalsused)
- [Failide struktuur](#failide-struktuur)
- [Tehtud tööde nimekiri](#tehtud-tööde-nimekiri)
- [Koodinäited](#koodinäited)
- [Lingid](#lingid)
- [Viited](#viited)

---

## Projekti kirjeldus

See projekt on **Microsoft Projecti kasutamise juhend**, mis on loodud veebilehena.
Juhend selgitab samm-sammult, kuidas:

- luua ja seadistada töökalendreid
- lugeda Gantti diagramme
- vaadata ressursside kulude aruandeid
- kasutada projekti ajajoont

> [!NOTE]
> See haru (`projectLibre`) sisaldab uuendatud versiooni võrreldes `main` haruga.
> Kõik muudatused on tehtud selles harus.

> [!WARNING]
> `valem.html` fail on sellest harust eemaldatud. Ära kasuta linki, mis sellele viitab.

---

## Muudetud failid

| Fail | Muudatus | Seotud issue |
|------|----------|--------------|
| `index.html` | Uuendatud sisu ja pildid, eemaldatud valem.html link | #4 |
| `diagramm.html` | Lisatud 5-sammuline diagrammide juhend koos piltidega | #5 |
| `valem.html` | **Kustutatud** projektist | #6 |
| `README.md` | Loodud uus README koos kõigi elementidega | — |

---

## Lisatud funktsionaalsused

### Kalender (`index.html`)

1. Uue baaskalendri loomine (`Project → Change Working Time → Create New Calendar`)
2. Erandi lisamine — `KellaAeg` (17:00–20:00 ja 21:00–00:00)
3. Kordumismustri seadistamine (Daily, 781 korda)
4. Gantti diagramm koos ajakavaga (img/5.png)

### Diagrammid (`diagramm.html`)

1. **Gantti diagramm** — ülesanded ajajoonel koos ressurssidega
2. **Aruannete menüü** — `Report → Costs → Resource Cost Overview`
3. **Ressursside kulude aruanne** — Actual Cost, Remaining Cost, Baseline Cost
4. **Projekti ajajoon (Timeline)** — 03.02.26–06.02.26

---

## Failide struktuur

```
GITHUB-pages/
├── index.html          # Kalendri loomise juhend
├── diagramm.html       # Diagrammide juhend
├── style.css           # Veebilehe stiil
├── README.md           # See fail
└── img/
    ├── 1.png           # Change Working Time menüü
    ├── 2.png           # Create New Calendar dialoog
    ├── 3.png           # Kalender eranditega
    ├── 4.png           # Erandi KellaAeg detailid
    ├── 5.png           # Gantti diagramm ajakavaga
    ├── d1.png          # Gantti diagramm täisvaates
    ├── d2.png          # Aruannete menüü
    ├── d3.png          # Ressursside kulude aruanne
    └── d4.png          # Projekti ajajoon
```

---

## Tehtud tööde nimekiri

- [x] Loodud uus haru `projectLibre`
- [x] Loodud 3 GitHub issue'd (#4, #5, #6)
- [x] Issue'd lisatud Kanban projekti
- [x] `index.html` uuendatud — uus sisu, pildid, nav ilma valem.html lingita
- [x] `diagramm.html` uuendatud — 5-sammuline juhend koos piltidega
- [x] `valem.html` kustutatud projektist
- [x] Navigeerimismenüü uuendatud mõlemas failis
- [x] Commitid seotud issue'dega (`Refs #4`, `Closes #6` jne)
- [x] README.md loodud
- [ ] GitHub Pages seadistamine (vt Settings → Pages → Source: projectLibre)

---

## Koodinäited

### Navigeerimismenüü HTML

```html
<nav>
  <ul>
    <li><a href="index.html">Kalendri loomine</a></li>
    <li><a href="diagramm.html">Diagrammid</a></li>
  </ul>
</nav>
```

### Pildi lisamine HTML-i

```html
<img src="img/1.png" alt="Change Working Time menüü">
```

### Git haru loomine ja commit issue'ga

```bash
git checkout -b projectLibre
git add index.html
git commit -m "Uuenda index.html: uus sisu ja pildid. Closes #4"
git push origin projectLibre
```

---

## Lingid

- [GitHub repositoorium](https://github.com/AdrianaPikaljov/GITHUB-pages)
- [GitHub Pages veebileht](https://adrianapikaljov.github.io/GITHUB-pages/)
- [Kanban projekt](https://github.com/users/AdrianaPikaljov/projects/5)
- [GitHub Markdown süntaks](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

---

## Pildid

### Kalender — Change Working Time menüü

![Change Working Time menüü](img/1.png)

### Diagramm — Gantti diagramm täisvaates

![Gantti diagramm täisvaates](img/d1.png)

---

## Viited

[^1]: Microsoft Project ametlik dokumentatsioon: https://support.microsoft.com/project
[^2]: GitHub Pages seadistamine: https://docs.github.com/en/pages
[^3]: Kanban metoodika: https://en.wikipedia.org/wiki/Kanban

---

*© 2026 Microsoft Project juhend — projectLibre haru* [^1] [^2] [^3]
