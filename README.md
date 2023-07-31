## Instructions
Salut et bienvenue dans l'équipe Gilded Rose. 

Comme vous le savez, nous sommes une petite auberge avec un emplacement privilégié dans une ville importante dirigée par un aubergiste sympathique nommé Allison. Nous achetons et vendons également uniquement les meilleurs produits. 

Malheureusement, la qualité de nos produits se dégrade constamment à l'approche de leur date limite de vente. Nous avons un système en place qui met à jour notre inventaire pour nous. Il a été développé par un ancien employé nommé Leeroy, qui est parti vers de nouvelles aventures. 

Votre tâche consiste à ajouter la nouvelle fonctionnalité à notre système afin que nous puissions commencer à vendre une nouvelle catégorie d'articles. Tout d'abord une introduction à notre système :

- Tous les articles ont une valeur `SellIn` qui indique le nombre de jours dont nous disposons pour vendre l'article

- Tous les articles ont une valeur de qualité qui indique la valeur de l'article

- À la fin de chaque journée, notre système abaisse les deux valeurs pour chaque article

Assez simple, non? Et bien c'est là que ça devient intéressant :

- Une fois la date de péremption passée, la qualité se dégrade deux fois plus vite

- La Qualité d'un article n'est jamais négative

- `Aged Brie` augmente en fait la qualité à mesure qu'il vieillit

- La qualité d'un article n'est jamais supérieure à 50

- `Sulfuras`, étant un objet légendaire, ne doit jamais être vendu ou diminue en qualité

- Les `passes Backstage`, comme le `brie vieilli`, augmentent en qualité à mesure que sa valeur `SellIn` approche ; La qualité augmente de 2 lorsqu'il y a 10 jours ou moins et de 3 lorsqu'il y a 5 jours ou moins mais la qualité tombe à 0 après le concert

Nous avons récemment signé un contrat avec un fournisseur d'articles `conjurés`. Cela nécessite une mise à jour de notre système :
- Les objets `conjurés` se dégradent en qualité deux fois plus vite que les objets normaux

N'hésitez pas à apporter des modifications à la méthode `UpdateQuality` et à ajouter un nouveau code tant que tout fonctionne toujours correctement. Cependant, ne modifiez pas la classe `Item` ou la propriété `Items` car celles-ci appartiennent au gobelin dans le coin qui vous insta-ragera et vous tirera dessus car il ne croit pas à la propriété partagée du code (vous pouvez faire en sorte que la méthode `UpdateQuality` et la propriété `Items` statique si vous le souhaitez, nous couvrirons pour vous).

Juste pour clarifier, un objet ne peut jamais voir sa qualité augmenter au-dessus de 50, cependant `Sulfuras` est un objet légendaire et en tant que tel sa qualité est de 80 et il ne change jamais.