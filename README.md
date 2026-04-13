# Gantt anual cu subtasks

Un fișier HTML simplu pentru afișarea și exportul unui Gantt anual cu subtasks și perioade multiple.

## Ce este

Acest repo conține un singur fișier `gantt.html` care oferă o interfață web locală pentru:
- Adăugarea proiectelor și a subtask-urilor (categorii)
- Definirea mai multor perioade (start/end) pentru proiecte și subtask-uri
- Export CSV / JPG / XLS
- Import CSV
- Ajustare lățime coloană nume și dimensiuni font

## Cum folosești

1. Deschide `gantt.html` în browser (dublu-click sau `File → Open`).
2. Completează `Nume proiect`, selectează culoarea și adaugă perioade.
3. Pentru fiecare categorie (subtask) poți defini culoare și perioade.
4. Utilizează butoanele din toolbar pentru a exporta sau importa date.

Notă: Starea (proiecte, culori, setări) se salvează local în `localStorage` browser-ului.

## Export / Import

- `Exportă CSV` — descarcă un CSV cu proiectele și perioadele.
- `Încarcă CSV` — importă proiecte dintr-un CSV în formatul așteptat.
- `Salvează JPG` / `Salvează XLS` — export vizual al tabelului.

## Personalizare

- Poți modifica variabilele CSS din interiorul `gantt.html` (în blocul `:root`) pentru a schimba culori, înălțimi de rând, font-size implicite etc.
- Există controale în toolbar pentru `Coloană nume`, `Text proiect` și `Text categorie`.

## Compatibilitate

- Fișier static — funcționează offline în orice browser modern.
- Nu necesită server.

## Licență

Folosire liberă — adaptează după cum dorești.

---

Fișier: `gantt.html` — vezi detalii și cod în repository.