# 👋 efbulle

Bienvenue sur mon profil ! Je suis un développeur Python passionné par la création d'outils innovants et la visualisation de données.

## 🎯 À propos de moi

- 🐍 Développeur Python enthousiaste
- 🗺️ Passionné par la cartographie et la visualisation de données
- 🚆 Je conçois aussi des outils de traitement de données ferroviaires
- 💡 J'aime créer des projets interactifs et utiles

## 📚 Mes projets phares

### 🗺️ [cartes_multicouches](https://github.com/efbulle/cartes_multicouches)

[![CI](https://github.com/efbulle/cartes_multicouches/actions/workflows/ci.yml/badge.svg)](https://github.com/efbulle/cartes_multicouches/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/efbulle/cartes_multicouches/blob/main/LICENSE)
[![Python](https://img.shields.io/badge/python-3.13%20%7C%203.14-blue.svg)](https://github.com/efbulle/cartes_multicouches)

Génère des cartes interactives multi-couches en Python avec **Bokeh** et **GeoPandas**, exportables en dashboards HTML autonomes.

<a href="https://efbulle.github.io/cartes_multicouches/" target="_blank">
  <img src="https://raw.githubusercontent.com/efbulle/cartes_multicouches/main/examples/illustrations/demo_interaction.gif" alt="Démonstration de cartes_multicouches" width="70%" />
</a>

👉 [Voir la démo en ligne](https://efbulle.github.io/cartes_multicouches/)

### 🚆 [pktools](https://github.com/efbulle/pktools)

[![CI](https://github.com/efbulle/pktools/actions/workflows/ci.yml/badge.svg)](https://github.com/efbulle/pktools/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/efbulle/pktools/blob/main/LICENCE)
[![Python](https://img.shields.io/badge/python-3.12%20%7C%203.13%20%7C%203.14-blue.svg)](https://github.com/efbulle/pktools)
[![PyPI](https://img.shields.io/pypi/v/pktools.svg)](https://pypi.org/project/pktools/)

Paquet Python pour la gestion des **points kilométriques (PK)** et des **tronçons** du réseau ferroviaire : conversions vectorisées (`polars`) entre représentations de PK, fusion et découpage d'intervalles en zones homogènes.

```python
import polars as pl
import pktools as pk

df = pl.DataFrame({"pk_ext": ["74+388", "412B+795", "0-214"]}).with_columns(
    pk_int=pk.ext_to_int(pl.col("pk_ext")),
    pk_m=pk.ext_to_m(pl.col("pk_ext")),
)
```

```bash
pip install pktools
```

## 📊 Stats GitHub

<a href="https://github.com/efbulle/cartes_multicouches">
  <img height="150em" src="https://github-readme-stats.vercel.app/api/pin/?username=efbulle&repo=cartes_multicouches&theme=default" alt="cartes_multicouches stats" />
</a>
<a href="https://github.com/efbulle/pktools">
  <img height="150em" src="https://github-readme-stats.vercel.app/api/pin/?username=efbulle&repo=pktools&theme=default" alt="pktools stats" />
</a>

## 📬 Me contacter

- 🔗 [LinkedIn](https://www.linkedin.com/in/emmanuel-favre-bulle) - Connectez-vous avec moi sur LinkedIn
- 🌐 [cartes_multicouches](https://github.com/efbulle/cartes_multicouches) · [pktools](https://github.com/efbulle/pktools) - Découvrez mes projets

---

*Merci de votre visite ! N'hésitez pas à explorer mes projets et à me contacter si vous avez des questions ou des opportunités de collaboration.*
