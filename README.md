# Mon API Pokémon

Bienvenue sur le projet "Mon API Pokémon" ! Explorez le monde Pokémon en utilisant cette application simple qui utilise l'API Tyradex pour afficher des informations détaillées sur vos Pokémon préférés.

## Table des matières
- [Mon API Pokémon](#mon-api-pokémon)
  - [Table des matières](#table-des-matières)
  - [Aperçu](#aperçu)
  - [Technologies utilisées](#technologies-utilisées)
  - [Comment utiliser](#comment-utiliser)
  - [Installation](#installation)
  - [Crédits](#crédits)
  - [Contact](#contact)
- [Style CSS](#style-css)
- [App.js](#appjs)
- [Crédits additionnels](#crédits-additionnels)

## Aperçu
![Aperçu de l'application](link-to-screenshot)

## Technologies utilisées
- HTML
- CSS
- JavaScript
- API Tyradex

## Comment utiliser
1. Ouvrez le fichier `index.html` dans votre navigateur.
2. Saisissez le nom du Pokémon que vous recherchez dans le formulaire.
3. Cliquez sur le bouton "Rechercher" pour afficher les détails du Pokémon.

## Installation
1. Clonez le repository vers votre machine locale.
   ```bash
   git clone https://github.com/Aescanor/Mon-API-Pokemon
   ```
2. Ouvrez le fichier `index.html` dans votre navigateur.

## Crédits
- Conçu et développé par [Dammaretz Gaëtan](https://github.com/Aescanor).
- API Tyradex par [Nom de l'auteur de l'API](lien-vers-le-profil-de-l'auteur)

## Contact
- GitHub: [Votre GitHub](https://github.com/Aescanor)
- LinkedIn: [Votre LinkedIn](https://www.linkedin.com/in/ga%C3%ABtan-dammaretz/)

© [Votre Nom] - GDWD Tous droits réservés.

---

# Style CSS

```css
:root {
  --mainColor: #2c3d50;
  --secondColor: #34495e;
}

/* ... (le reste du CSS) ... */
```

# App.js

```javascript
// ... (le reste du JavaScript) ...

// Projet API Pokémon méthode GET :

const formPokemon = document
  .getElementById("formPokemon")
  .addEventListener("submit", function (e) {
    e.preventDefault();

    const searchPokemon = document.getElementById("searchPokemon").value.trim();

    const infoText = document.querySelector("p.infoText");

    if (searchPokemon.length <= 2) {
      infoText.innerHTML = `Recherche invalide !`;
      return;
    }

    const url = `https://tyradex.vercel.app/api/v1/pokemon/${searchPokemon}`;

    async function getDataPokemon() {
      try {
        // ... (le reste du code) ...
      } catch (error) {
        console.error(error);
      }
    }

    getDataPokemon(url);
  });

// ... (le reste du JavaScript) ...
```

# Crédits additionnels
Un grand merci à [Auteur de l'API Tyradex](https://github.com/Yarkis01) pour fournir cette incroyable API Pokémon (Tyradex) !

---
