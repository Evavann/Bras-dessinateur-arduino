<h1>Séance 6 Evann CORVAISIER</h1>
<p>J ai commencé la séance par réaliser des recherches pour trouver differents programmes sur des cnc plotter<p>
<p>J ai ainsi trouvé un programme permettant a notre bras d aller a des positions rentré en parametre.<p>
  <img class="fit-picture"
     src="../Image/Fonction goTo_EvannCharlotte.png"
     alt="Fonction goTo"
     width=40% height=10%>
<p>La suite de la séance a été la plus compliquée. Nous nous sommes mis à deux afin d'enfin tenter de faire dessiner PROPREMENT notre stylo. Ce qui, pour le moment, est encore un échec. En effet, nous avons repris le programme des anciens PEIP2 ayant déjà réalisé un projet similaire au nôtre que nous avons réécrit à notre manière. La seule fonction que nous n'avons pas changé est "goTo", celle permettant de faire aller le stylo à des certaines coordonnées.</p>
<p>C'est à ce moment-là que les problèmes sont apparus. En effet, nous avons d'abord essayé de faire bouger chaque servomoteur afin de voir si chacun fonctionnait bien indépendamment des autres, puis nous les avons fait bouger ensemble. Tout marchait. Puis lorsque nous avons essayé la fonction goTo (de faire aller le stylo par exemple : de la position (4,0) à (6,0) donc une ligne droite horizontale), cela ne marchait pas et ne nous traçait absolument pas la ligne droite horizontale voulue. Parfois même, rien ne se déclenchait.</p>
<p>Nous avons donc décidé (sous les conseils de Mr.Masson) d'imprimer dans le moniteur série chaque ligne du goTo unes par unes afin de voir laquelle ne marchait pas.</p>
<img class="fit-picture"
     src="../Image/Fonction goTo_EvannCharlotte.png"
     alt="Fonction goTo"
     width=40% height=10%>
<p>La ligne "d=sqrt......" qui nous donne la distance de notre trait marchait. Puis lorsque nous faisions "Serial.println(Angle)", le moniteur série nous retournait "nan" en boucle. Nous ne connaissions pas cette erreur et Mr.Masson non plus. C'est sur cette partie que nous avons donc énormément bloqué. J'ai donc décidé de tester la fonction goTo issue d'une partie de programme des anciennes PEIP2 afin de voir si cette formule d'angle marchait dans le cas. Voici donc leur fonction goTo :</p>
<img class="fit-picture"
     src="../Image/FonctiongoTo_AnciensPEIP2.png"
     alt="Fonction goTo"
     width=40% height=10%>
<p>Ici, "Serial.println(Alpha)" marchait parfaitement et nous renvoyait bien un angle intermédiaire. Là est notre problème : la formule "Angle" de notre fonction est exactement la même que la formule "Alpha" de la leur. Nous ne comprenons donc pas pourquoi notre moniteur nous renvoie "nan" et non l'angle voulu.</p>
<p>Après le cours, nous avons recherché ce que voulait donc dire "nan", et nous avons trouvé "nan signifie que l'on essaye d'imprimer un float d'une valeur "Not a Number", qui n'est pas un nombre". Nous allons donc devoir comprendre pourquoi notre valeur "Angle" n'est pas un nombre.</p>
<p>Nous allons donc revenir plusieurs fois dans la semaine afin de résoudre ce problème et d'enfin pouvoir faire fonctionner notre fonction goTo et donc notre programme en général.</p>
