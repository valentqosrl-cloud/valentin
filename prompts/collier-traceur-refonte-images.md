# Prompt ChatGPT : refonte complète des images du collier traceur Bluetooth

**Avant de coller le prompt :**
1. Ouvre une **nouvelle conversation** ChatGPT, avec la génération d'images et l'Interpréteur de code activés.
2. Joins **toutes les photos du fournisseur** : chaque coloris, le support ouvert et fermé, la balise seule, le contenu du colis, et les photos du chat qui porte le collier si le fournisseur en a.
3. Joins l'image de référence de l'**avatar chat Nuvopattes** et le **logo**.
4. Colle tout le bloc ci-dessous.

---

```
═══════════════════════════════════════════
0. CONTEXTE ET MISSION
═══════════════════════════════════════════
Boutique : Nuvopattes (accessoires pour chats, livraison en France et en Belgique).
Produit : Collier traceur Bluetooth pour chat, compatible Android (Google Localiser / Find Hub).
Coloris vendus : Noir, Rose, Bleu. Prix : 19 €.

Le pack d'images actuel est À JETER. Il montre 4 modèles de support différents
(support fermé avec coussinets dessinés, coussinets en relief, patte ajourée,
support à couvercle) et 2 boucles différentes, sur des PNG transparents qui s'affichent
en noir. Le client ne reçoit pas ce qu'il voit.

Ta mission : refaire de ZÉRO un pack de 6 images qui montre EXACTEMENT le produit
des photos fournisseur jointes, aux couleurs Nuvopattes, et qui fait comprendre
le produit et ses limites sans lire la description.

═══════════════════════════════════════════
1. RÈGLE N°1 : FIDÉLITÉ AU PRODUIT (LA PLUS IMPORTANTE)
═══════════════════════════════════════════
Les photos fournisseur jointes sont la SEULE référence du produit.

AVANT TOUTE CRÉATION, fais une « FICHE D'IDENTITÉ DU PRODUIT » à partir des photos :
  a) SUPPORT / ÉTUI : forme exacte (patte ? ronde ? ajourée ? coussinets en relief ou
     plats ?), système d'ouverture (couvercle à charnière, étui souple dans lequel
     on glisse la balise…), passants pour le collier, couleur.
  b) BALISE : forme, couleur, taille, détails visibles (trou de haut-parleur, logo, bouton).
  c) COLLIER : couleur de chaque coloris, bande réfléchissante (oui/non, où), largeur.
  d) BOUCLE : forme exacte (tête de chat ? boucle simple ?), boucle de sécurité qui
     s'ouvre si le chat s'accroche (oui/non).
  e) ACCESSOIRES : grelot (couleur), anneau, pile, autre.
  f) DIFFÉRENCES ENTRE COLORIS : la forme est-elle identique pour noir, rose et bleu ?
  g) INCOHÉRENCES : si les photos fournisseur montrent plusieurs modèles différents,
     LISTE-LES et DEMANDE-MOI lequel je reçois. Ne choisis pas à ma place.
  h) Textes chinois, filigranes ou logos du fournisseur sur les photos : liste-les
     (ils devront être supprimés).
→ Présente cette fiche et ATTENDS MA VALIDATION avant de continuer.

PENDANT LA CRÉATION :
- Le produit n'est JAMAIS redessiné ni réinventé par le générateur d'images.
- Pour les images 1, 4, 5 et 6 : tu DÉTOURES le produit à partir des photos fournisseur
  (Python : rembg + Pillow) et tu le poses tel quel. Seuls sont permis : redimensionner,
  faire pivoter légèrement, ajouter une ombre douce, nettoyer les poussières, et
  supprimer un texte ou un filigrane du fournisseur.
- Pour les scènes (chat qui porte le collier) : tu pars de la photo fournisseur et tu
  modifies uniquement le décor. Si tu dois générer la scène, tu compares ensuite le
  collier de la scène à la fiche d'identité, point par point (support, boucle, grelot,
  bande réfléchissante, couleur). Au moindre écart : tu refais.
- Le même modèle sur les 6 images ET sur les 3 coloris. Pour changer de coloris, tu
  utilises la vraie photo fournisseur de ce coloris, jamais un recoloriage approximatif.

═══════════════════════════════════════════
2. INFOS PRODUIT (N'INVENTE RIEN D'AUTRE)
═══════════════════════════════════════════
- Traceur Bluetooth qui se connecte au réseau Google Localiser (Find Hub) d'un
  smartphone Android. Sans abonnement.
- ⚠ Compatible UNIQUEMENT Android. Ne fonctionne PAS avec un iPhone.
- ⚠ Ce n'est PAS un GPS : la position s'actualise quand un smartphone Android passe à
  proximité (portée Bluetooth d'environ 50 à 100 m).
- Étanche IP68 (pluie, éclaboussures).
- Pile bouton CR2032.
- Étui en silicone souple, léger.
- Collier réglable de 20 à 33 cm, largeur 1 cm, bande réfléchissante, grelot,
  boucle de sécurité.
- Support : 5,8 x 3,6 cm.
- Convient aux chats et aux petits chiens.
→ Si une photo fournisseur contredit une de ces infos (taille, boucle, nombre de pièces…),
  SIGNALE-LE-MOI au lieu de choisir.
→ Infos inconnues (autonomie en mois, poids de la balise, pile fournie ou non,
  version Android) : demande-les-moi. Si je ne les ai pas, tu ne les affiches pas.

═══════════════════════════════════════════
3. CHARTE NUVOPATTES (STRICTE)
═══════════════════════════════════════════
Fond   : #FFFFFF (blanc), sur toutes les images.
Texte  : #000000 (noir).
Accent : #BC804C (brun chaud) → pictos ronds, flèches, cotes, numéros d'étapes,
         filets sous les titres, contours d'encarts, bandeaux.
Polices : titres en sans-serif très gras et condensé, en MAJUSCULES ;
          textes en sans-serif gras.
- AUCUNE autre couleur de mise en page : pas de beige, d'orange, de doré, de dégradé,
  de fond coloré. Le noir, le rose et le bleu du COLLIER ne déteignent jamais sur
  la mise en page.
- Texte sur le brun #BC804C : en noir. Blanc sur brun seulement pour un très gros
  titre en gras.
- Tous les textes, pictos, flèches et cotes sont posés avec Python (Pillow), JAMAIS
  écrits par le générateur d'images (couleurs exactes, zéro faute, accents corrects).
- Petit logo Nuvopattes en bas à droite sur les images 2 à 6.
- Avatar chat Nuvopattes (image de référence jointe) : présent sur les images 3 à 6,
  25 % de l'image maximum, toujours identique à la référence, ne cache jamais le
  produit. JAMAIS sur l'image 1. Sans image de référence : pas d'avatar.

═══════════════════════════════════════════
4. INTERDITS (Google, Meta, TikTok, droit de la consommation)
═══════════════════════════════════════════
- Les mots « GPS », « temps réel », « en direct », « suivi en continu »,
  « localisation partout », « portée illimitée ».
- Les ondes ou signaux qui sortent du collier vers le téléphone (ils suggèrent
  un suivi en direct).
- Tout logo d'une autre marque : Google, Android (le robot vert), Apple, Bluetooth.
  On écrit seulement « Compatible Android » en texte.
- Une copie d'écran de l'application Google : utilise un écran de smartphone
  GÉNÉRIQUE (carte simplifiée grise et blanche + épingle #BC804C
  + « Dernière position connue »).
- Tout iPhone reconnaissable (encoche, Dynamic Island, logo) : smartphone Android
  générique uniquement.
- « n°1 », « le meilleur », « le plus vendu », « le plus choisi », de fausses
  étoiles ou de faux avis, un prix, un pourcentage de réduction.
- Un chiffre que tu ne trouves ni dans la partie 2 ni dans mes réponses.

═══════════════════════════════════════════
5. LES 6 IMAGES (2048 x 2048 px, carré, marge de 120 px, texte de 48 px minimum)
═══════════════════════════════════════════

IMAGE 1 : PRINCIPALE (Google Merchant + vignette Shopify), UNE PAR COLORIS
- Le collier SEUL, fermé en boucle, vue de 3/4, support et balise bien visibles,
  boucle visible. Il occupe 80 à 90 % de l'image.
- Fond blanc pur #FFFFFF. AUCUN texte, logo, avatar, picto ni bordure. Ombre douce
  autorisée.
- Exports : …-01-noir.jpg, …-01-rose.jpg, …-01-bleu.jpg (fond blanc, PAS de PNG
  transparent).
- Les 3 coloris : même angle, même cadrage, même modèle.

IMAGE 2 : LIFESTYLE + PROMESSE
- Vrai chat (photo réaliste) qui porte le collier NOIR, conforme à la fiche d'identité.
  Le chat est à gauche et le collier est bien visible.
- Titre : « RETROUVEZ VOTRE CHAT PLUS FACILEMENT », filet #BC804C dessous.
- 3 pictos ronds #BC804C + texte : « Sans abonnement » · « Étanche IP68 »
  · « Léger et confortable ».
- Encart en bas, contour #BC804C, picto ⚠ :
  « Android uniquement · Traceur Bluetooth, pas un GPS ».

IMAGE 3 : FONCTIONNEMENT
- Titre : « COMMENT ÇA MARCHE ? »
- 3 étapes dans 3 cartes à coins arrondis, contour #BC804C, numéros 1, 2, 3 dans des
  cercles #BC804C :
  1. « Installez la balise » : le geste RÉEL d'après les photos fournisseur
     (ex. ouvrir, insérer, clipser), avec le VRAI support.
  2. « Associez-la à votre Android » : smartphone Android générique + « Google
     Localiser » écrit en texte simple.
  3. « Voyez sa dernière position » : écran générique, carte + épingle #BC804C.
- Sous les étapes, en petit : « Position actualisée quand un smartphone Android passe
  à proximité (environ 50 à 100 m) ».
- L'avatar chat qui montre l'étape 1.

IMAGE 4 : CARACTÉRISTIQUES
- Titre : « LES DÉTAILS QUI COMPTENT »
- Le collier noir détouré au centre, et 4 à 6 loupes rondes à contour #BC804C, reliées
  par un trait #BC804C : bande réfléchissante · boucle de sécurité · grelot · support
  en silicone · étanche IP68 · pile CR2032.
- Chaque loupe est un ZOOM sur la VRAIE photo fournisseur, jamais un dessin.
- L'avatar chat dans un coin.

IMAGE 5 : ENTRETIEN ET UTILISATION
- Titre : « SIMPLE AU QUOTIDIEN »
- Changer la pile CR2032 en 2 ou 3 étapes, avec le VRAI geste d'après les photos
  fournisseur (si les photos ne montrent pas comment ouvrir la balise : demande-moi).
- Pictos : « Résiste à la pluie » · « Sans abonnement » · « Chats et petits chiens ».
- L'avatar chat qui tient une pile.

IMAGE 6 : DIMENSIONS, CONTENU ET COLORIS
- Titre : « DIMENSIONS ET CONTENU »
- Le collier noir avec ses cotes (flèches fines #BC804C à double pointe, chiffres
  noirs) : « Tour de cou 20 à 33 cm » · « Largeur 1 cm » · support « 5,8 x 3,6 cm »
  (les 2 cotes annotées).
- « Dans le colis » : chaque élément réellement fourni, avec sa quantité.
- Les 3 coloris côte à côte : Noir · Rose · Bleu (vraies photos).
- L'avatar chat qui tient un mètre ruban.
- Encart ⚠ : « Android uniquement · pas compatible iPhone ».
- Bandeau bas #BC804C, texte noir : « Livraison offerte FR et BE · Retour 14 jours
  · Garantie 2 ans · Paiement sécurisé ».

═══════════════════════════════════════════
6. MÉTHODE (RESPECTE L'ORDRE, ATTENDS MA VALIDATION À CHAQUE ÉTAPE ⏸)
═══════════════════════════════════════════
A ⏸ La fiche d'identité du produit (partie 1) + tes questions.
B ⏸ Les textes exacts des 6 images, dans un tableau.
C   Production : détourages Python → scènes générées si besoin (SANS texte dedans)
    → composition finale en Python/Pillow.
D ⏸ Contrôle qualité, une ligne par image :
    2048 x 2048 ✔ | fond #FFFFFF ✔ | HEX = charte ✔ | même support que les photos
    fournisseur ✔ | même boucle ✔ | même grelot ✔ | orthographe ✔ |
    aucun mot interdit ✔ | ⚠ Android/pas GPS présent (images 2 et 6) ✔
    + un aperçu des 6 images côte à côte, à côté d'une photo fournisseur,
    pour que je compare.
E   Livraison : un ZIP « NUVO-COLLIER-TRACEUR-pack-images.zip » qui contient :
    NUVO-COLLIER-TRACEUR-01-noir.jpg
    NUVO-COLLIER-TRACEUR-01-rose.jpg
    NUVO-COLLIER-TRACEUR-01-bleu.jpg
    NUVO-COLLIER-TRACEUR-02-lifestyle.jpg
    NUVO-COLLIER-TRACEUR-03-fonctionnement.jpg
    NUVO-COLLIER-TRACEUR-04-caracteristiques.jpg
    NUVO-COLLIER-TRACEUR-05-entretien.jpg
    NUVO-COLLIER-TRACEUR-06-dimensions-contenu.jpg
    (JPG en qualité 90, sRGB) + un fichier alt-textes.txt avec un texte alternatif
    de 125 caractères maximum par image, en français, qui décrit l'image avec le mot-clé
    « collier traceur Bluetooth pour chat ».
    Donne-moi le lien de téléchargement.

Si une règle ne peut pas être respectée (ex. le produit change à la génération),
DIS-LE au lieu de livrer. Ne dis jamais « c'est fait » sans le ZIP.
```

---

## Si ChatGPT dévie

| Problème | Réponse à envoyer |
|---|---|
| Le support ou la boucle ne correspond pas | « Le support de l'image X ne correspond pas à la photo fournisseur n°Y. Reprends le détourage de la photo, ne le génère pas. » |
| Mauvaise couleur | « Recompose l'image X en Python : fond #FFFFFF, texte #000000, accent #BC804C. Ne régénère rien. » |
| Du texte écrit par l'IA, avec des fautes | « Supprime tout texte de l'image générée et repose-le en Python. » |
| Des ondes ou « temps réel » | « Règle 4 : enlève les ondes et tout ce qui fait penser à un suivi en direct. » |
| Pas de ZIP | « Étape E : crée le ZIP avec Python et donne-moi le lien. » |

## Après réception du ZIP, dans Shopify

1. Supprime les 8 anciennes images.
2. Importe les 8 nouvelles images, dans l'ordre : 01-noir, 02, 03, 04, 05, 06, puis 01-rose et 01-bleu.
3. Associe `01-noir`, `01-rose` et `01-bleu` à leur variante.
4. Colle le texte alternatif de chaque image (fichier `alt-textes.txt`).
