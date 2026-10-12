# Document Vault — site public

Site static în limba română pentru prezentarea Document Vault și pentru paginile publice cerute de configurarea Google OAuth. Proiectul site-ului este separat de aplicația Windows/Android. Nu conține seifuri, documente, backupuri, tokenuri sau acreditări OAuth.

## Conținut

- `index.html` — pagina principală și explicația folosirii opționale a Google Drive.
- `privacy.html` — politica de confidențialitate, inclusiv datele Google API.
- `terms.html` — termenii de utilizare.
- `assets/css/styles.css` și `assets/js/main.js` — prezentare și interacțiuni minime, fără framework sau servicii externe.
- `assets/images/` și `favicon.ico` — bannerul și iconița Document Vault.

Fișierele pot fi deschise direct în browser. Pentru verificare locală prin HTTP, din rădăcina proiectului rulează `python -m http.server 8000` și deschide `http://localhost:8000/`. Nu este necesar un pas de build.

## Publicare ulterioară prin GitHub Pages

Site-ul este pregătit pentru GitHub Pages, dar proiectul local nu este publicat automat și nu are remote configurat.

1. Creează pe GitHub un repository numit `document-vault-site` în contul dorit.
2. Adaugă acel repository ca remote și fă push pentru ramura `main` numai când dorești să publici site-ul.
3. În repository, deschide **Settings → Pages**.
4. La **Build and deployment**, alege **Deploy from a branch**.
5. Selectează ramura **main** și folderul **/(root)**, apoi salvează.
6. După publicare, URL-ul va fi `https://<username>.github.io/document-vault-site/`, unde `<username>` este numele real al contului GitHub.

Pentru Google Auth Platform, folosește URL-urile publice finale, după ce site-ul este accesibil:

| Câmp | URL |
| --- | --- |
| Homepage | `https://<username>.github.io/document-vault-site/` |
| Privacy Policy | `https://<username>.github.io/document-vault-site/privacy.html` |
| Terms of Use | `https://<username>.github.io/document-vault-site/terms.html` |

Site-ul nu publică aplicația și nu conține linkuri de descărcare a aplicației. Înainte de publicare, verifică încă o dată exactitatea politicii, identitatea operatorului și adresa de contact.
