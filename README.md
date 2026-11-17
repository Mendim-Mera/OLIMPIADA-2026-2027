# Olimpiadat 2026-2027: forma dhe tabela

`index.html` është forma për mësuesit. `Code.gs` e shton çdo dërgim në tabelën Google Sheet, që ka saktësisht strukturën e modelit Excel.

## Hapat (përditësim i tabelës që keni tashmë)

1. **Tabela si modeli.** Hapni Google Sheet-in që përdorni (ai ku keni ngjitur `Code.gs`).
   File → Import → Upload → zgjidhni `OLIMPIADA_2026-2027.xlsx` → "Replace spreadsheet" → Import data.
   Do të shfaqen 18 fletët e modelit (9 lëndë, secila me fletën e saj përmbledhëse).
2. **Kodi i ri.** Extensions → Apps Script. Fshini kodin e vjetër, ngjitni `Code.gs` të ri dhe ruajeni.
3. **Formulat.** Lart zgjidhni funksionin `setup` dhe shtypni Run (autorizoni kur kërkohet). Kjo vendos formulat në fletët përmbledhëse dhe krijon fletën "Dërgimet".
4. **Versioni i ri i skriptit.** Deploy → Manage deployments → ikona e lapsit → Version: **New version** → Deploy. URL-ja mbetet e njëjta, ndaj `index.html` nuk ndryshon.
5. **Faqja.** Zëvendësoni `index.html` në GitHub me këtë të re.

## Si funksionon tabela
- **Fletët e lëndëve** (p.sh. "matematikë AML"): çdo nxënës i dërguar shtohet në rreshtin e parë bosh, me kolonat e modelit. Dërgimet e mësuesve të ndryshëm vijnë njëri pas tjetrit.
- **Fletët përmbledhëse**: llogariten vetë me formula (pjesëmarrës, fitues, publik/privat, klasat, "Gjithsej" për çdo DRAP). Mos i ndryshoni dorazi qelizat me formula.
- **Fleta "Dërgimet"**: një rresht për çdo formë të dërguar, me datën, emrin e mësuesit, ZVA-në dhe numrin e pjesëmarrësve. Numri i pjesëmarrësve në përmbledhëse është shuma e atyre që kanë dhënë mësuesit e ZVA-së.
- Për Excel: File → Download → Microsoft Excel (.xlsx).

## Shënime
- Nëse një mësues e dërgon formën me gabim, fshijini dorazi rreshtat e nxënësve te fleta e lëndës dhe rreshtin e tij te "Dërgimet".
- Kushdo që ka lidhjen e faqes mund të dërgojë të dhëna, ndaj mos e publikoni gjerë.
