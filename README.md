# LIFE4FARMS – zástupná landing page

Statický web (každá jazyková verze je jeden HTML soubor s CSS a JS), připravený pro GitHub Pages.

- `lp/index.html` – landing page česky
- `lp/en/index.html` – anglická verze (přepínač CZ/EN je v navigaci)
- `lp/img/` – logo a fotka nebe
- `foto/`, `loga/` – fotky a loga, na které stránky odkazují relativně (`../foto/…`, `../../foto/…`), proto musí ležet vedle složky `lp/`
- `index.html` – přesměrování z kořene webu na `lp/`
- `.nojekyll` – GitHub Pages nemá soubory zpracovávat Jekyllem

## Nasazení

1. Rozbalte ZIP a do kořene repozitáře nahrajte jeho **obsah** (ne samotný ZIP).
2. Settings → Pages → Source: „Deploy from a branch“, větev `main`, složka `/ (root)`.
3. Web poběží na `https://<uživatel>.github.io/<repozitář>/` (kořen přesměruje na `/lp/`), anglická verze na `…/lp/en/`.

Stránky mají zatím `<meta name="robots" content="noindex">`, aby je vyhledávače neindexovaly. Před ostrým spuštěním ji odstraňte.
