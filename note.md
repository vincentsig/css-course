<!-- Note generale pour le cours -->
<!--
Il existe deux type de transitions.

la premiere conssite simplement a utiliser la propriete de transition.

la seconde est de specifier les etapes de transitions.

after pseudo permet de creer un element virtuelle juste apres l element selectionne et on peut donc styliser ce pseudo element.

Pour les 'em' les mesure sont basé sur les font size.
Pour les font la reference est le parent
pour le padding la reference est l element courrant
rem utilise le root comme reference

// padding utilise le fontsize comme reference, donc si on a padding:2em et que le font size est 16px le padding sera 32

!! text proppriety are inherited
pading margin are not inherited -->

<!-- BEM Block Element Modifier -->

<!-- .block__element--modifier -->

Question pour Simon:

- Qu est ce qui est le plus souvent utilisé pour le sass :
  - BEM
  - SMAC

<!-- pseudo class first or last element -->

<!-- classic css -->

li:last-child {
margin: 0px;
}

li:first-child {
margin: 5px;
}

<!-- scss -->

li {
fontsize:10px;

    &:first-child {
        margin: 0;
    }

}

    <!-- cest comme li:first-child -->

clear fix explication:

Si on float un container tout les element vont perdre leur heigth ce qui va rendre le content a 0px. on perd donc la stylisation du container.
le hack et de faire un clearfix qui a des proprieté pour faire un after qui va simuler le contenu dórigine et appliquer le style.

tricks :

- on peut muliplier un nombre sans unit par \* 1px. le resultat sera alors le nombre en px.

%nom-du-placeholder

on appelle ca extend, cela permet d'eviter de la publication dans le code source.
( a revoir, pas forcement les choses les plus utilisés)

# Basic responsive design principles

fluid layouts

- allo webpage to adapt to the current viewport width or even height
- use % or vh / vw unit instead of pc for element that should afapt to viewport (usealy layout)
- Use max width instead of width.

  ## layout types

  - float layouts
  - flexbox (1 dimensional row)
  - css grid (2 domensional grid)

  ##

  responsive units

flexible iages

Media queries
