# Graphiques RE2020 — bullet graphs (WSP)

Outil web gratuit pour produire les graphiques des résultats RE2020
(Bbio, CEP, CEPnr, DH, ICénergie, ICconstruction).

👉 **Ouvrir l'outil :** https://ciol894.github.io/NOM_DU_DEPOT/voici/render/RE2020_BulletGraphs.html

Tout est calculé dans le navigateur (Voici / WebAssembly) : aucune donnée de projet n'est
envoyée sur un serveur. Pensez à télécharger exports et JSON avant de fermer la page.

## Structure
| Fichier | Rôle |
|---|---|
| `content/RE2020_BulletGraphs.ipynb` | L'application |
| `environment.yml` | Paquets Python chargés dans le navigateur |
| `build-environment.yml` | Outils de construction (GitHub Actions) |
| `.github/workflows/deploy.yml` | Construction + publication automatiques à chaque commit sur `main` |
| `requirements.txt` | Usage local (`pip install -r requirements.txt` puis `voila content/RE2020_BulletGraphs.ipynb`) |

## Mettre à jour l'outil
Remplacer `content/RE2020_BulletGraphs.ipynb` (même nom) puis valider le commit :
le site se reconstruit tout seul en quelques minutes (onglet **Actions**).

Contact : Loïc Corvalan.
