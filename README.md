Il va sans dire que c'est le corps de la méthode void placeComponents() qui nous intéresse essentiellement dans ces exercices.

Pour vous épargner le codage long et fastidieux des composants graphiques, une classe abstraite Distrib est donnée en ressource. Les trois classes à compléter héritent de cette classe abstraite qui contient tout le code commun aux trois applications. Vous pouvez accéder à ces composants à l'aide de méthodes protégées de Distrib :

JLabel jl(int) pour obtenir l'un des labels ;
JButton jb(int) pour obtenir l'un des boutons ;
JTextField jtf(int) pour obtenir l'un des champs de texte.
Les indices attendus en paramètre de ces méthodes doivent être l'une des constantes prédéfinies de la classe Distrib. Le nom de ces constantes commence par L_ pour les labels, par B_ pour les boutons, et par F_ pour les champs de texte.

Au trois méthodes précédentes, j'ai ajouté deux méthodes protégées qui vous seront parfois utiles :

JTextField jtfs() qui retourne le tableau des trois champs de texte ;
JFrame frame() qui donne accès à la fenêtre de l'application.
Bref, jetez un œil attentif sur le code de la classe Distrib avant de commencer à coder.

GridBagLayout
Pour cet exercice, quadrillez votre fenêtre selon 7 lignes et 7 colonnes comme indiqué sur la photo ci-dessous, puis appliquez la méthode donnée en cours (zones caractéristiques, et tout le tralala...) :

gridbagdistrib.png

La classe GridBagDistrib est fournie, il ne vous reste plus qu'à compléter sa méthode createCons(). Cette méthode crée les contraintes nécessaires et les associe à leurs composants graphiques respectifs dans une Map, de telle sorte que la méthode placeComponents() s'en trouve grandement simplifiée (d'ailleurs cette dernière vous est donnée). Les poids souhaités sont déductibles des deux premiers clichés de l'énoncé.

Je vous ai laissé les constantes dont vous aurez besoin pour définir les insets des contraintes.
