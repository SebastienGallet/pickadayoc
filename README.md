# Pickadayoc
Pickadayoc est un composant React qui intègre Pikaday, un sélecteur de dates léger et personnalisable.

## Installation
Pour utiliser Pickadayoc dans votre projet, suivez ces étapes :

Installez les dépendances en exécutant :
```bash
npm install pickadayoc
```

## Utilisation
Après l'installation, vous pouvez intégrer Pickadayoc dans vos composants React.

Voici un exemple d'utilisation :

```jsx
import React, { useState } from 'react';
import PikadayPicker from 'pickadayoc';

const MyComponent = () => {
  const [date, setDate] = useState(new Date());

  const handleChange = (newDate) => {
    setDate(newDate);
  };

  return (
    <div>
      <h1>Sélectionnez une date</h1>
      <PikadayPicker value={date} onChange={handleChange} />
    </div>
  );
};

export default MyComponent;
```


## Propriétés
Le composant PikadayPicker accepte les propriétés suivantes :

-value: La date sélectionnée (objet Date).
-onChange: Une fonction appelée lorsque l'utilisateur sélectionne une date. Elle reçoit la nouvelle date en tant qu'argument.

## Personnalisation
Vous pouvez personnaliser le sélecteur de dates en modifiant les styles CSS. Le fichier CSS de Pikaday est inclus dans le paquet et peut être surchargé selon vos besoins.

