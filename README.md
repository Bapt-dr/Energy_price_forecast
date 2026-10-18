Sous-étape 2 : information disponible au moment de décider (jour D-1, avant midi)

Le principe : une variable n’est utilisable que si elle était publiée avant la clôture de l’enchère day-ahead, qui a lieu vers 12h (heure de Bruxelles) le jour D-1.

Disponible à D-1 avant midi

Prix day-ahead jusqu’à D-1 inclus. Ils sont publiés vers 12h45 le jour D-2, donc tu les connais avant la décision. Je m’étais trompé plus haut en disant « jusqu’à D-2 ».
Consommation et production réalisées jusqu’à D-2, avec une marge de publication à vérifier. Les données de la journée D-1 complète ne sont pas disponibles avant midi. Il faudra donc tenir compte du décalage, par exemple en n’utilisant que les données réalisées jusqu’au matin de D-1.
Prévision de consommation établie la veille pour D (prevision_j1 dans eCO2mix, selon la description de la doc que j’ai lue).
Prévisions météo pour D (vent, soleil, température), mais uniquement les runs publiés avant midi D-1. Une prévision météo récente ne doit pas être utilisée si elle est sortie après la clôture.
Indisponibilités programmées des centrales pour D, publiées à l’avance sur la plateforme de transparence (REMIT). Source à identifier.

Non disponible à D-1 avant midi

Les prix de D, qui sont la cible.
La production et la consommation réalisées de D, y compris l’éolien et le solaire effectivement produits.
La météo réalisée de D. Seules les prévisions existent à ce moment.
prevision_j : d’après la doc, c’est la prévision réactualisée le jour même, donc elle n’existe pas encore à D-1 midi. C’est un piège, car elle ressemble à prevision_j1 et se trouve dans le même enregistrement.

