Traductions
===========

La documentation Symfony2 est écrite en anglais et de nombreuses personnes 
participent au processus de traduction.

Participer
----------

D'abord devenez familier avec le :doc:`markup language <format>` utilisé par la 
documentation.

Ensuite, souscrivez à la liste de diffusion `Symfony docs mailing-list`_, tout
se déroule là.

Finalement, trouvez le dépot *principal* du langage auquel vous voulez
contribuer. Voici une liste des dépots officiel:

* *Anglais*:   https://github.com/symfony/symfony-docs
* *Français*:  https://github.com/gscorpio/symfony-docs-fr
* *Italien*:   https://github.com/garak/symfony-docs-it
* *Japonais*:  https://github.com/symfony-japan/symfony-docs-ja
* *Polonais*:  https://github.com/ampluso/symfony-docs-pl
* *Roumain*:   https://github.com/sebio/symfony-docs-ro
* *Russe*:     https://github.com/avalanche123/symfony-docs-ru
* *Espagnol*:  https://github.com/gitnacho/symfony-docs-es

.. note::

    Si vous voulez participer à la traduction d'un nouveau langage, lisez la
    :ref:`section dédiée<translations-adding-a-new-language>`.

Rejoindre l'équipe de traduction
--------------------------------

Si vous voulez aider à traduire certains documents dans votre langue ou corriger
des erreurs, rejoinger nous; c'est une processus simple:

* Présentez vous sur la liste de diffusion `Symfony docs mailing-list`_;
* *(optionel)* Proposer les sujets sur lesquels vous pouvez travailler;
* Forker le dépot *master* de votre language (clic sur le bouton "Fork" sur la 
page github);
* Traduisez certains documents et envoyé les sur votre dépot;
* Effectuer une requête de mise à jour (clic sur le bouton "Pull Request" de 
votre page sur GitHub);
* Le chef d'équipe accepte vos modifications et les fusionnent avec le dépot
  master;
* Le site de la documentation est mis à jour toutes les nuits à partir du dépot
du chef d'équipe.

.. _translations-adding-a-new-language:

Ajouter une nouvelle langue
--------------------------

Cette section présente le guide à suivre pour commencer la traduction de la
documentation de Symfony2 dans une nouvelle langue.

Commencer une traduction représente une masse de travail importante, parlez en
sur la liste de diffusion `Symfony docs mailing-list`_ et essayez de trouver des
gens motivés pour vous aider.

Quand l'équipe est prête nommé un chef d'équipe, ; il aura la responsabilité du
dépot principal (*master*).

Créer le dépot et copier les documents en anglais.

L'équipe peut maintenant commencer son travail de traduction.

Quand l'équipe est certaine que le dépot est stable et à jour (tout est traduit,
ou les documents non traduits ont été supprimés des sommaires (toctree -- 
correspondants aux fichiers dénommés ``index.rst`` et ``map.rst.inc``), le chef
d'équipe peut demander que le dépot soit ajouté à la liste officielle des 
dépot *master* en envoyant un courriel à Fabien (fabien at symfony.com).

Maintenance
-----------

Le processus de traduction ne s'arrête pas quand tout est traduit. La 
documentation est régulièrement mise à jour, déplacée (des nouveaux documents
sont ajoutés, des bogues sont fixés, des paragraphes sont réorganisés, ...).
L'équipe de traduction a besoin de suivre le dépot anglais et d'appliquer les
changement aux documents traduits aussitôt que possible.

.. caution::

    Les langues non maintenues sont supprimées de la liste officielle des dépôts
    car mettre à disposition une documentation obsolète comporte des risques
	dangeureux.

.. _Symfony docs mailing-list: http://groups.google.com/group/symfony-docs