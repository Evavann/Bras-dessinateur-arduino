<h1>Séance 7 Charlotte FRÈRE</h1>
<p>Après la séance de la semaine dernière où nous étions vraiment bloqués, j'ai ramené notre bras chez moi afin de continuer les recherches tout au long de la semaine. J'ai donc recalculé tous les angles qui étaient présents dans la fonction goTo afin de beaucoup mieux comprendre cette fonction et de débloquer le problème du "nan" que nous avions. J'ai donc utilisé le théorème d'Al-Khashi afin de les calculer et j'ai donc obtenu les formules ci-dessous : </p>
<img class="fit-picture"
     src="../Image/CalculDesAngles_AlKhashi.HEIC"
     alt="Formules pour les angles"
     width=40% height=10%>
<p>J'ai donc par la suite réécrit la fonction goTo en commentant chaque ligne afin de me rappeler du lien entre la formule mathématique et l'angle correspondant. De plus, grâce aux "Serial.println(.....)", j'ai pu voir ce qui n'allait pas en fonction des coordonnées que je prenais.</p>
<img class="fit-picture"
     src="../Image/FonctionGoTo_Réécrite.png"
     alt="Fonction goTo"
     width=40% height=10%>
<p>Après cela, il n'y avait plus de problèmes pour cette fonction.</p>
<p>Puis, en cours, lors de cette séance, nous avons donc défini une zone de dessin pour notre bras. Cette zone s'est vue être beaucoup plus petite (environ de la taille d'un post-it) que ce que nous imaginions au départ mais Mr.Masson nous a expliqué qu'il serait trop compliqué de dessiner sur une zone plus grande de par la longueur des pièces de bois reliant notre premier servomoteur (l'épaule), au second (le coude).</p>
<p>Ensuite, dans le loop, grâce à la fonction .write() : epaule.write(....) et coude.write(....), nous avons défini chaques angles (l'angle du servo épaule et celui du servo coude) de chaque coin de notre zone de dessin atteignable. Le point situé en haut à gauche correspondra ensuite au point de coordonnées (0,0) et ainsi de suite afin de donner les coordonnées limites de chaque extrémité du rectangle de dessin.</p>
<p>Désormais, avant la prochaine séance, il faudrait que nous arrivions à initialiser dans la fonction goTo, les coordonnées de point x=0 et y=0 correspondant aux angles permettant au stylo d'atteindre le coin en haut à gauche. Nous devons donc trouver la façon de passer d'angles à des coordonnées cartésiennes x et y. Nous devons réussir à associer les deux, chose que nous n'avons pas encore réussi à réaliser.</p>
