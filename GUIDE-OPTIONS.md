# 🧩 Options à brancher (nécessitent un compte ou une clé)

Ces éléments ne sont **pas** dans le README par défaut parce qu'ils demandent
tes identifiants. Copie le bloc voulu dans `README.md` à l'endroit de ton choix.
Remplace `TON_PSEUDO`, `TON_ID`, etc.

---

## 🎵 Spotify « en train d'écouter »

1. Déploie le projet [novatorem](https://github.com/novatorem/novatorem) sur Vercel (gratuit)
   en suivant son README (il faut une app Spotify Developer + 3 variables d'environnement).
2. Ajoute dans le README :

```html
<p align="center">
  <a href="https://open.spotify.com/user/TON_ID_SPOTIFY">
    <img src="https://TON-APP.vercel.app/api/spotify" alt="Spotify" />
  </a>
</p>
```

---

## ⏱️ WakaTime (temps de code de la semaine)

1. Crée un compte sur [wakatime.com](https://wakatime.com) et installe le plugin dans ton éditeur.
2. **Option simple** : Dashboard → Share → « Embeddable charts » → copie le lien de l'image :

```html
<p align="center">
  <img src="https://wakatime.com/share/@TON_PSEUDO/TON_UUID.svg" alt="WakaTime" />
</p>
```

---

## 🔐 TryHackMe / HackTheBox (cybersécurité)

```html
<!-- TryHackMe : Account → ton profil → "Badge" -->
<p align="center">
  <a href="https://tryhackme.com/p/TON_PSEUDO">
    <img src="https://tryhackme-badges.s3.amazonaws.com/TON_PSEUDO.png" alt="TryHackMe" />
  </a>
</p>
```

HackTheBox : utilise le badge officiel de ton profil (Settings → Share).

---

## 💻 LeetCode / Codeforces / HackerRank

```html
<p align="center">
  <a href="https://leetcode.com/TON_PSEUDO"><img src="https://leetcard.jacoblin.cool/TON_PSEUDO?theme=dark&font=Karla&ext=heatmap" alt="LeetCode" /></a>
</p>
```

---

## 🎓 Certifications (Credly, Coursera, Google, Cisco…)

```markdown
### 🎓 Certifications
[![Cert 1](https://img.shields.io/badge/Cisco-Cybersecurity_Essentials-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white)](LIEN_DU_CERTIFICAT)
[![Cert 2](https://img.shields.io/badge/Coursera-Nom_du_cours-0056D2?style=for-the-badge&logo=coursera&logoColor=white)](LIEN_DU_CERTIFICAT)
```

---

## 📰 Mes derniers articles (blog, dev.to, Medium, Hashnode)

Si tu as un flux RSS, crée `.github/workflows/blog.yml` :

```yaml
name: Blog posts
on:
  schedule:
    - cron: "0 */12 * * *"
  workflow_dispatch:
permissions:
  contents: write
jobs:
  blog:
    runs-on: ubuntu-latest
    steps:
      - uses: gautamkrishnar/blog-post-workflow@v1
        with:
          feed_list: "https://dev.to/feed/TON_PSEUDO"
          max_post_count: 5
```

Puis ajoute dans le README :

```html
## 📰 Derniers articles
<!-- BLOG-POST-LIST:START -->
<!-- BLOG-POST-LIST:END -->
```

---

## ⚙️ Réglages à connaître

| Sujet | Où / quoi |
|---|---|
| Barres « Ce que j'apprends » | `assets/learning.svg` : change les pourcentages (valeurs d'exemple !) |
| Couleurs du Togo | vert `#006A4E`, jaune `#FFCE00`, rouge `#D21034` |
| Changer la fréquence des animations | `cron` dans `.github/workflows/animations.yml` |
| Réinitialiser les échecs | remets `{}` dans `chess/game.json`, puis lance `node .github/scripts/chess.js render` |
| Vider le livre d'or | remets `[]` dans `guestbook/entries.json` |
