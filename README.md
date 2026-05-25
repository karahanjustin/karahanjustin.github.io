# karahanjustin.github.io → potsdam-media.de

Master-Repo für die Website unter **https://potsdam-media.de**.

## Struktur

- `/` (Root) → Submodul [`potsdam-media`](https://github.com/karahanjustin/potsdam-media)
- `/website-showcase/` → Submodul [`website-showcase`](https://github.com/karahanjustin/website-showcase)

Submodule liegen unter `_src/`. Sie werden bei jedem Push, einmal täglich (04:00 UTC) und manuell per `workflow_dispatch` aktualisiert.

## Neues Projekt hinzufügen

1. `git submodule add https://github.com/karahanjustin/<repo>.git _src/<repo>`
2. In `.github/workflows/pages.yml` einen neuen `rsync`-Block für das Zielverzeichnis ergänzen.
3. Commit & Push.

## Lokal klonen

```bash
git clone --recurse-submodules https://github.com/karahanjustin/karahanjustin.github.io.git
```
