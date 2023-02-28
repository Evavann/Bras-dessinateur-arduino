<h1>Séance 8 Charlotte FRÈRE</h1>

<p>Avant cette séance, nous nous étions rendus compte de la masse de travail qu'il nous restait à faire car nous n'arrivions absolument pas à faire écrire le bras.</p>
<p>Je m'étais donc, durant les vacances, fixé l'objectif de réussir à faire écrire une lettre correctement au bras avant cette séance.</p>
<p>Pendant les vacances, j'ai donc cherché et réfléchi à la manière de coder pour tracer une lettre. J'ai donc totalement repris le code, je n'ai plus du tout utiisé le code des anciens peip2, et tout refait par moi-même (parfois avec l'aide d'internet et de certaines personnes, surtout au niveau du débug du code).</p>
<p>Pour tracer une lettre, je commence donc par définir un tableau composés de tableaux (vecteurs) eux-mêmes composés de 3 éléments (tableau[0]=x, tableau[1]=y, tableau[2]= 1 ou 0). L'élément 0 correspond donc à la coordonnée x, l'élément 1 à la coordonnée y et l'élément 2 (1 ou 0), correspond au fait que le stylo soit en position d'écriture ou non (via les fonctions lever() et baisser()).</p>
<p>Ensuite voici donc la partie de mon code permettant de tracer un "É" (tous les commentaires sont sur le code et expliquent comment il fonctionne) :</p>
<p>ATTENTION, CECI N'EST PAS LE CODE QUI EST DÉFINITIF, JE L'AI MODIFIÉ AFIN QU'IL MARCHE RÉÉLLEMENT APRÈS, MAIS L'IDÉE DE LA MANIÈRE DE TRACER LA LETTRE EST EXACTEMENT LA MÊME ! </p>
<img class="fit-picture"
     src="../Image/IdéeCode_TracerUneLettre.png"
     alt="Code commenté pour tracer une lettre"
     width=40% height=10%>
<p>Les fonctions ligne() et bougeDeLa() permettent 2 choses.</p>
<p>ligne() permet d'aller d'une coordonnée 1 à une coordonnée 2 en traçant une ligne. En effet, elle commence par faire la fonction baisser() permettant de faire écrire le stylo, puis elle calcule les points intermédiaires (calculés tous à une distance constante les uns des autres en fonction de la longueur de la ligne) puis fait un goTo(vPointInter) afin d'aller à chacun de ces points intermédiaires.</p>
<p>bougeDeLa() permet d'aller d'une coordonnée 1 à une coordonnée 2 sans tracer de ligne (afin d'aller plus rapidement à un endroit où il n'est pas nécessaire de devoir repasser). En effet, elle commence par faire la fonction lever() permettant de ne plus écrire, puis elle fait simplement un goTo(vFin) pour aller à la coordonnée demandée. Elle n'a donc pas besoin de passer par chaque point intermédiaire et va donc plus rapidement à la coordonnée 2.</p>
<p>bougeDeLa() permet d'aller d'une coordonnée 1 à une coordonnée 2 sans tracer de ligne (afin d'aller plus rapidement à un endroit où il n'est pas nécessaire de devoir repasser). En effet, elle commence par faire la fonction lever() permettant de ne plus écrire, puis elle fait simplement un goTo(vFin) pour aller à la coordonnée demandée. Elle n'a donc pas besoin de passer par chaque point intermédiaire et va donc plus rapidement à la coordonnée 2.</p>
<p>Ces fonctions seront présentes (détaillées et COMMENTÉES) dans le code final, voir même dans le rapport final.</p>
<p>Pour écrire ce code, j'ai décidé d'utiliser des tableaux afin de voir plus clairement ce à quoi nous faisions référence à chaque fois.</p>
<p>J'ai également eu besoin d'utiliser des pointeurs, car sans ceux-là je ne pouvais pas faire marcher le code pleinement et à chaque fois. Pour ce que sont les pointeurs, je l'ai expliqué au prof durant la séance même si je ne connais pas précisément son mode de fonctionnement.</p>
<p>Si j'avais voulu simplifier ce code, sans utiliser de pointeurs, j'aurai pu coder dans un autre language que le C++ (qui est un language nécessitant une bonne compréhension de la machine).</p>
<p>Puis j'ai calibré les servos correctement afin d'avoir la plus grande zone d'écriture possible.</p>
<p>Avant de coder, et afin de prendre les meilleures décisions possibles, j'ai décidé de commencer en modélisant le bras sur Excel.</p>
<p>Pour conclure, nous avons vraiment bien avancé pour notre projet, et surtout sur la compréhension de ce dernier.</p>
