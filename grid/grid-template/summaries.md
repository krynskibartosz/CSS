Pour faire une layout clean on utilise le flex-box dans un système de grid

Dans un sytème de grid on a un grid-container et des grid-items
Comme pour els flex-box


Un bon Layout Serait:


Grid-container  
    > grid-items
        > flex-container
            > flex-items

    > grid-items + grid-container
        > grid-items
            > flex-container
                > flex-items


flex-box:

    flex =  {

        ( Une valeur sans unité)
        - flex-grow = combien de fois l'item flex séléctionner est aggrandi par rapport aux autres items-flex.
        - flex-shrink = combien de fois l'item flex séléctionner sera plus petit par rapport aux autres items-flex.
        

         (valeur avec une unité)
        - flex-basis = Précise une taille spécifique à l'item-flex séléctionner.
    }


Grid:

    Voici comment on peut donner des noms a nos columns & rows avec le système de grilles.

        grid-template-columns : [col1] 40px [col2] 3fr;


        grid-template-rows: repeat(2, 350px [row]) 10%;


        grid template : {
            grid-template-rows / grid-template-columns;
        }



    grid-area:{
         grid-row-start/
         grid-column-start/
         grid-row-end /
         grid-column-end
        }
    
    exemple:
        grid-area : 2 / 1 / span 2 / span 3


    gap = écart
    gap : {
        grid-row-gap
        grid-column-gap
    }


