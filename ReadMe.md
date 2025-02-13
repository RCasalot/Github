# Git_Versions


[![Développement Web](https://img.shields.io/badge/HTML-CSS-yellow)](https://www.w3.org/)
[![Python Versions](https://img.shields.io/badge/Python-3-blue)](https://www.python.org/)

[![Markdown](https://img.shields.io/badge/M%20⬇-191970)](https://www.carnus.fr/)
[![GitHub git](https://img.shields.io/badge/GitHub-git-fd5800)](https://www.carnus.fr/)

# Dossier Web :
## V0 : Version fournie
## V1 :
- Ajouter cette table au fichier `index.html`
  - Modifier le fichier HTML
  - Modifier le fichier CSS
  - Dans ce fichier MarkDown, ajouter l'arborescence de votre dossier

| Matière | Volume horaire [h] | Coefficient |
|--|--|--|
| Anglais | 3 | 3 |
| Maths | 2 | 2 |
| Physique | 4 | 3 |
| Info. et Réseaux | 15 | 10 |

## V2 :
- Ajouter au début du tableau une ligne pour la matière CGE
- Ajouter une image au fichier HTML
  - Modifier le fichier HTML
  - Modifier le fichier CSS

---

# Dossier Py :
## V0 : Version fournie
## V1 :
- Tracer la courbe du signal sinusoïdal $s(t)=a.sin(2\pi .f .t)$
  - Modifier le fichier `code.ipynb`
  - Modifier le fichier `ReadMe.md` pour inclure les lignes de code

## V2 :
- Tracer la courbe du signal sinusoïdal $s(t)=a.sin(2\pi .f .t+\frac{\pi}{3})$
  - Modifier le fichier `code.ipynb`
---
## <cite> Architecture du dossier</cite>

📦Git_versions-main
┃ ┣ 📜Git_Exp.pdf
┃ ┣ 📜CES.jpg
┃ ┣ 📜README.md
  ┗ 📂Py
  ┃ ┣ 📜code.ipynb
  ┗ 📂Web
  ┃ ┣ 📜index.html
  ┃ ┣ 📜style.css

---

## <cite> Code V1 </cite>

```
import plotly.graph_objects as go
import numpy as np

fe = 1e2 # Fréquence d'échantillonnage
t = np.arange(0,2+(1/fe),1/fe)

# Signal
f = 2
a = 0.5

# Formule du signal
s = a * np.sin(2 * np.pi * f * t)

# Courbe du signal
fig = go.Figure(data=go.Scatter(x=t, y=s, mode='lines'))
fig.update_layout(title="Signal sinusoïdal", xaxis_title="Temps [s]", yaxis_title_text="Amplitude [V]")
fig.show()
```


---
## <cite> Code V2</cite>

```
import plotly.graph_objects as go
import numpy as np

fe = 1e2 # Fréquence d'échantillonnage
t = np.arange(0,2+(1/fe),1/fe)

# Signal
f = 2
a = 0.5

# Formule du signal
s = a * np.sin(2 * np.pi * f * t + np.pi/3)

# Courbe du signal
fig = go.Figure(data=go.Scatter(x=t, y=s, mode='lines'))
fig.update_layout(title="Signal sinusoïdal", xaxis_title="Temps [s]", yaxis_title_text="Amplitude [V]")
fig.show()
```

<kbd> [GitHub](https://github.com/boudjelaba) ↗️ </kbd>

