<div align="center">

<img src="assets/banner.png" alt="Lumea" width="100%">

<br>

**Les dons de ta campagne Streamlabs Charity, en direct dans OBS.**
**Gratuit, pour Windows, et un total toujours juste.**

<br>

<a href="https://github.com/tristanbest0802-beep/Lumea-widgets/releases/download/v0.2.6/Lumea-Setup-0.2.6.exe">
  <img src="https://img.shields.io/badge/T%C3%A9l%C3%A9charger%20Lumea-Installateur%20Windows-1F5FCC?style=for-the-badge&logo=windows&logoColor=white" alt="Télécharger l'installateur de Lumea pour Windows" height="56">
</a>

<b><!-- version -->Version 0.2.6<!-- /version --></b>

<sub>Windows 10 et 11 · gratuit · aucun compte à créer · <a href="https://github.com/tristanbest0802-beep/Lumea-widgets/releases">toutes les versions</a></sub>

<br><br>

![Windows](https://img.shields.io/badge/Windows-10%20%7C%2011-0078D6?logo=windows&logoColor=white)
![OBS](https://img.shields.io/badge/OBS-source%20Navigateur-302E31?logo=obsstudio&logoColor=white)
![Streamlabs Charity](https://img.shields.io/badge/Streamlabs-Charity-80F5D2)
![Gratuit](https://img.shields.io/badge/prix-gratuit-1F7F4F)

</div>

---

## Sommaire

- [En deux mots](#en-deux-mots)
- [Installer Lumea (3 minutes)](#installer-lumea-3-minutes)
- [Premier lancement](#premier-lancement)
- [Ajouter un widget dans OBS](#ajouter-un-widget-dans-obs)
- [Les widgets](#les-widgets)
- [Les thèmes](#les-thèmes)
- [Organisateur ou streamer ?](#organisateur-ou-streamer-)
- [Un total qui ne se trompe pas](#un-total-qui-ne-se-trompe-pas)
- [Le jour de l'événement](#le-jour-de-lévénement)
- [Tes données et celles des donateurs](#tes-données-et-celles-des-donateurs)
- [Questions fréquentes](#questions-fréquentes)
- [Contenu de ce dépôt](#contenu-de-ce-dépôt)
- [Licences](#licences)

---

## En deux mots

| | |
|---|---|
| **Ce que ça fait** | Lumea lit ta campagne Streamlabs Charity et affiche le total en direct dans OBS. Un badge apparaît à chaque don, un flash marque chaque palier franchi, et le montant défile comme une roulette. |
| **Pour qui** | Les équipes de streamers caritatifs : un organisateur et jusqu'à 20 streamers. Ça marche aussi pour une campagne perso. |
| **Ce qu'il faut** | Un PC Windows 10 ou 11, OBS Studio, et le lien de ta cagnotte Streamlabs Charity. |
| **La promesse** | Le total à l'écran est toujours le total officiel, même après un redémarrage, une coupure d'internet ou un plantage. |

---

## Installer Lumea (3 minutes)

1. **Télécharge l'installateur** avec le gros bouton bleu en haut de cette page.
2. **Lance `Lumea-Setup-<version>.exe`** (le nom du fichier indique la version). Il s'installe pour ton compte Windows, sans droits d'administrateur.
3. Si Windows affiche « Windows a protégé votre ordinateur », clique sur **Informations complémentaires**, puis sur **Exécuter quand même**. L'installateur n'est pas encore signé ; un certificat est prévu.
4. Coche **Démarrer avec Windows** si tu veux que Lumea soit prêt dès l'allumage du PC.

Les mises à jour sont proposées au démarrage du logiciel. Tes réglages et ton historique de dons sont gardés dans `%APPDATA%\Lumea` : ni une mise à jour ni une désinstallation ne les effacent.

---

## Premier lancement

Un assistant de deux étapes te guide :

1. **Colle le lien de ta cagnotte.** Lumea le vérifie aussitôt et affiche le nom et le total de la campagne.
   - Équipe : `https://streamlabscharity.com/teams/@ton-equipe/ta-campagne`
   - Campagne perso : `https://streamlabscharity.com/@ton-pseudo/ta-campagne`
   - Pas encore de lien ? Choisis **Fausse source** pour tout essayer avec des dons simulés.
2. **Choisis ton rôle** : Organisateur ou Streamer. En mode Streamer, choisis ton nom dans la liste de l'équipe.

Le lien se change à tout moment dans **Réglages**. Si c'est la même cagnotte, les dons sont gardés ; si c'en est une autre, l'ancienne est archivée.

---

## Ajouter un widget dans OBS

1. Dans Lumea, ouvre l'onglet **Widgets** et clique sur **Copier l'adresse**.
2. Dans OBS : **Sources**, puis **+**, puis **Navigateur**.
3. Colle l'adresse dans **URL**.
4. Règle la taille sur **760 × 420**. La marge autour du widget laisse de la place au flash des paliers.
5. Valide. Le widget se met à jour tout seul, il n'y a rien à recharger.

Le bouton **Aperçu** ouvre le même widget dans ton navigateur, pour régler le style avant le direct.

---

## Les widgets

| Widget | Adresse | Ce qu'il montre |
|---|---|---|
| Total global | `http://127.0.0.1:8642/widget/global` | Le total de toute l'équipe |
| Widget perso | `http://127.0.0.1:8642/widget/perso/<id>` | Le total d'un streamer, son nom et le total de l'équipe |

Chaque widget comprend :

- **La roulette** : le montant défile jusqu'au nouveau total, en option.
- **Le badge de don** : « + montant » à chaque nouveau don, jamais deux fois pour le même don.
- **Le flash de palier** : une seule fois par palier, même après un redémarrage.
- **Les animations réduites** : une option pour ceux qui préfèrent moins de mouvement.

Prévus plus tard : barre d'objectif, liste des derniers dons, top donateurs, alerte plein écran, compte à rebours, défis débloqués par montant.

---

## Les thèmes

Huit thèmes sont livrés. Chacun se règle ensuite à la main (couleurs, police, titre, devise affichée).

| Thème | Style |
|---|---|
| `lumea` | Le thème par défaut : bleu nuit, montant blanc, contour bleu, flash jaune soleil |
| `neon-violet`, `neon-cyan`, `neon-rose` | Néon lumineux |
| `pixel` | Rétro pixel |
| `arcade` | Borne d'arcade |
| `sobre` | Discret, pour les scènes chargées |
| `verre` | Fond transparent, laisse voir la vidéo derrière |

Toutes les polices sont livrées avec le logiciel. Les widgets marchent sans internet, et aucun appel ne part vers Google Fonts.

---

## Organisateur ou streamer ?

| | Organisateur | Streamer |
|---|---|---|
| Qui | La personne qui gère l'événement | Chaque streamer de l'équipe |
| Voit | Toute l'équipe, tous les streamers | Son total et celui de l'équipe |
| Peut | Gérer les paliers et les pseudos, styler tous les widgets, saisir le total à la main | Styler son propre widget |

Chaque PC lit Streamlabs lui-même. Rien ne passe entre les PC, aucun port n'est ouvert sur le réseau, et il n'y a pas de mot de passe à retenir.

---

## Un total qui ne se trompe pas

C'est la raison d'être de Lumea.

- Le chiffre à l'écran est **toujours le dernier total officiel** de Streamlabs, jamais plus haut.
- Chaque don est enregistré une seule fois, avec son identifiant, en centimes entiers.
- Le total est comparé à la somme des dons à chaque lecture. Le moindre écart est noté dans le journal.
- Après un redémarrage, le bon total s'affiche avant toute autre chose.
- Si Streamlabs ne répond plus, le widget garde le dernier chiffre. Seul le logiciel affiche « dernier total confirmé à HH:MM », jamais le stream.

---

## Le jour de l'événement

- Fais une répétition la veille avec la **Fausse source** ou un don de test (onglet **Tests et paliers**). Les dons de test ne comptent jamais dans le total.
- Le PC ne se met pas en veille tant que Lumea suit une campagne.
- Si quelque chose ne va pas, l'organisateur peut **saisir le total** ou le **figer**.
- En fin de stream, fige le total final et exporte les dons en CSV.

---

## Tes données et celles des donateurs

- Tout reste **sur ton PC**. Lumea n'envoie rien ailleurs ; il lit seulement les pages publiques de ta campagne.
- Les noms et messages des donateurs sont effacés automatiquement **90 jours après la fin de la campagne**. Un bouton permet aussi de les effacer tout de suite, et les totaux ne changent pas.
- Un avis de confidentialité (Loi 25 du Québec) est affiché au premier lancement et dans les Réglages.

---

## Questions fréquentes

<details>
<summary><b>Windows bloque l'installateur</b></summary>

C'est l'alerte SmartScreen, normale pour un logiciel pas encore signé. Clique sur **Informations complémentaires**, puis sur **Exécuter quand même**.
</details>

<details>
<summary><b>Le widget reste à 0 $</b></summary>

Vérifie dans l'onglet **Campagne et source** que le lien est bon et que la pastille est verte. Une campagne qui n'a encore reçu aucun don affiche bien 0 $.
</details>

<details>
<summary><b>Le widget n'apparaît pas dans OBS</b></summary>

Lumea doit être lancé : son icône doit être visible près de l'horloge. Vérifie aussi que l'adresse de la source Navigateur commence par `http://127.0.0.1:8642/`.
</details>

<details>
<summary><b>Je ferme la fenêtre, est-ce que ça s'arrête ?</b></summary>

Non. Lumea passe près de l'horloge et continue d'alimenter les widgets. Pour l'arrêter vraiment : clic droit sur l'icône, puis **Quitter**.
</details>

<details>
<summary><b>Un streamer n'apparaît pas dans la liste</b></summary>

La liste des membres est relue toutes les 5 minutes. Vérifie qu'il a bien rejoint l'équipe sur Streamlabs Charity.
</details>

---

## Contenu de ce dépôt

Ce dépôt est la vitrine publique de Lumea. Le code du logiciel lui-même est privé.

```
widgets/
  global/index.html   widget total global et perso (roulette, badge, paliers)
  fonts/              polices livrées, avec leurs licences OFL
themes/               les 8 thèmes en JSON (réglages de base)
assets/               logo et bannières
```

Les installateurs sont publiés dans les [releases](https://github.com/tristanbest0802-beep/Lumea-widgets/releases).

Chaque widget ne parle qu'au Lumea installé sur son propre PC, à l'adresse `127.0.0.1`. Il ne peut ni lire ni modifier les données de quelqu'un d'autre.

---

## Licences

- Polices : SIL Open Font License, voir les fichiers `OFL` de `widgets/fonts/`.
- Lumea n'est ni affilié à Streamlabs, ni approuvé par Streamlabs.

<div align="center">
<br>
<a href="https://github.com/tristanbest0802-beep/Lumea-widgets/releases/download/v0.2.6/Lumea-Setup-0.2.6.exe">
  <img src="https://img.shields.io/badge/T%C3%A9l%C3%A9charger%20Lumea-Installateur%20Windows-1F5FCC?style=for-the-badge&logo=windows&logoColor=white" alt="Télécharger l'installateur de Lumea pour Windows" height="44">
</a>
</div>
