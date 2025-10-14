# Visie C- en D-cluster HBO Bedrijfskunde

Dit repository bevat het visiedocument voor de C- en D-clusters van de HBO-opleiding Bedrijfskunde, ontwikkeld als een Quarto Book.

## Project Structuur

```
visie-doc-jaar2/
├── _quarto.yml              # Quarto book configuratie
├── index.qmd                # Landing page
├── executive-summary.qmd    # Executive summary
├── part1/                   # DEEL 1: WHY
│   ├── 01-inleiding-transitiefase.qmd
│   ├── 02-c-cluster-transitie.qmd
│   ├── 03-d-cluster-praktijk.qmd
│   └── 04-samenhang-cd.qmd
├── part2/                   # DEEL 2: HOW
│   ├── 05-ontwerpprincipes-c-cluster.qmd
│   ├── 06-ontwerpprincipes-d-cluster.qmd
│   └── 07-randvoorwaarden-kwaliteit.qmd
├── part3/                   # DEEL 3: Van Visie naar Praktijk
│   ├── 08-implementatie.qmd
│   └── 09-conclusie.qmd
├── appendices/              # Bijlagen
│   ├── bijlage-a-eindkwalificaties.qmd
│   ├── bijlage-b-literatuur.qmd
│   └── bijlage-c-consultatie.qmd
├── references.qmd           # Referenties
├── references.bib           # BibTeX bibliografie
└── docs/                    # Gebouwde output (HTML/PDF)
```

## Quarto Book gebruiken

### Installatie

Quarto is reeds geïnstalleerd (versie 1.6.40). Voor PDF output is TinyTeX vereist:

```bash
quarto install tinytex
```

### Het boek bouwen

**HTML versie (altijd beschikbaar):**
```bash
quarto render --to html
```

**PDF versie (vereist TinyTeX):**
```bash
quarto render --to pdf
```

**Beide formaten:**
```bash
quarto render
```

### Preview tijdens bewerken

Start een live preview server:
```bash
quarto preview
```

Dit opent een browser met live reload - wijzigingen in .qmd bestanden worden automatisch weergegeven.

### Individueel hoofdstuk renderen

```bash
quarto render part1/01-inleiding-transitiefase.qmd
```

## Inhoud toevoegen

Alle hoofdstukken zijn aangemaakt met de volledige structuur uit de outline. Elk bestand bevat:
- Hoofdstuktitels en subsecties
- Placeholders `[Uitwerking volgt]` waar content moet worden toegevoegd

### Workflow voor het toevoegen van content

1. Open het relevante `.qmd` bestand
2. Vervang `[Uitwerking volgt]` met daadwerkelijke content
3. Gebruik Markdown formatting
4. Test met `quarto preview`
5. Commit wijzigingen naar git

### Markdown tips

- `#` = Hoofdstuk niveau 1
- `##` = Sectie niveau 2
- `###` = Subsectie niveau 3
- `####` = Niveau 4
- `**vet**` voor dikgedrukte tekst
- `*cursief*` voor schuine tekst
- Lijsten met `-` of `1.`
- Links: `[tekst](url)`

## Documentstructuur

Het visiedocument beantwoordt twee kernvragen:

1. **WHY** – Wat is de unieke bijdrage van het C- en D-cluster aan bedrijfskundige professionaliteit?
2. **HOW** – Vanuit welke ontwerpuitgangspunten en criteria komen we tot een optimaal cluster?

### Deel 1: WHY (5-7 pagina's)
- Inleiding: De transitiefase
- C-cluster: Transitie van uitvoeren naar ontwerpen
- D-cluster: Toepassing in authentieke praktijk
- Samenhang C→D

### Deel 2: HOW (8-10 pagina's)
- Ontwerpprincipes voor het C-cluster
- Ontwerpprincipes voor het D-cluster
- Randvoorwaarden en kwaliteitscriteria

### Deel 3: Van Visie naar Praktijk (2-3 pagina's)
- Implementatie
- Conclusie

## Output

De gebouwde bestanden worden geplaatst in `docs/`:
- `docs/index.html` - HTML versie (met navigatie)
- `docs/index.pdf` - PDF versie (indien TinyTeX geïnstalleerd)

**Let op:** De `docs/` directory is ideaal voor GitHub Pages hosting.

## Referenties toevoegen

1. Voeg BibTeX entries toe aan `references.bib`
2. Citeer in tekst met `@author2024`
3. Referenties verschijnen automatisch in `references.qmd`

## Status

**Versie:** 1.0
**Status:** Structuur compleet, content volgt
**Datum:** 14 oktober 2025

## Bronnen

- [Quarto Documentation](https://quarto.org/docs/books/)
- starting-doc.md - Projectvoorstel
- eindkwalificaties-prop-ad.md - Competentiekader
