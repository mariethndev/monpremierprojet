Etape 1 
- Ajouter une div
- Mettre le badge dans un span avec une classe "badge" 
- Ajouter un h2 "Ma carte"
- Ajouter une image 
- Ajouter un a avec le texte "voir plus" 


Partie CSS
- Mettre une couleur blanc crème au body
- mettre en display flex sur le body +
body: display: flex;
 height: 100vh;
justify-content : center; (horizontal)
 align items center (vertical)
- Appeler la classe card 
    - La mettre en position relative, les éléments à l'intérieur seront en absolute.
- Centrer avec flex 
    display: flex;
    flex-direction: column
    align-items: center; (vertical)
- Ajouter une width: 300px 
- bgcolor : white
- border-radius : 10px
- Redimensionner l'image (.card)
    .card > img {
        width: 100% (par rapport à la taille de son contenant)
        border-radius: 8px;
    }
- Mettre le badge sur le côté (plusieurs façon)
    Le contenant sera en relative afin que le nouveau puisse bouger en absolute
    .card en position : relative

    relative : tjrs dans le flux donc le flex fonctionne 

    .card {
        position: relative;
    }

- rajouter un padding de 1rem dans la .card 
- dans body, rajouter font-family arial
- Souligner le h2 
    .card > h2 {
        text-decoration: underline;
    }
- Le badge doit pouvoir se dplacer donc viser le badge
.badge {
    position: absolute; (il va pouvoir se balader partou sur la carte)

    il est sorti du flux
    son parent doit être en RELATIF SINON CEST LE HTML 
    background-color: crimson;
    color: white;
    padding: 0.3rem;
    border-radius: 10px; 
    font-size: 0.8rem; (80% de la taille)
    top: 10px; 
    right: 10px; 
}

- Remettre les margins et paddings à 0 avec *

- mettre du gap das .card de 1rem; 

- viser le lien 

.card > a {
    text-decoration: none;
    color: white;
    background-color: blue;
    padding: 0.5rem 1rem; (au dessus, sur les côtés)
    border-radius: 10px;
}

- ajouter un hover à card




