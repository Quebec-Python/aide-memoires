Installation de Python
======================

Sous Windows et Mac OS
----------------------

La problématique principale sous Windows et Mac OS est la nécessité de compiler
certains modules sur votre poste.

En effet, si vous n'avez pas installer explicitement un compilateur, vos
tentatives d'installation de module externe échoueront.

Il existe heureusement des distributions qui nous rendent la vie plus facile.

En voici 3:

* `ActivePython <http://www.activestate.com/activepython>`_
* `PythonXY <https://code.google.com/p/pythonxy/>`_
* `Anaconda <https://store.continuum.io/cshop/anaconda/>`_

Les instructions suivantes s'appliquent pour l'utilisation d'Anaconda, mais
sentez-vous bien à l'aise d'utiliser *ActivePython* ou *PythonXY*.

Installer *Anaconda*
~~~~~~~~~~~~~~~~~~~~

`Téléchargez la distribution anaconda <https://store.continuum.io/cshop/anaconda/>`_ et installez le sur votre poste

Tester votre installation
~~~~~~~~~~~~~~~~~~~~~~~~~

Tester le tout en tapant les commandes suivantes dans votre terminal.

.. code-block:: bash
   :linenos:
   
   $ conda info
   $ conda install fabric
   $ fab --help
   
La première commande nous affiche des détails sur *Anaconda* et *conda*.

La deuxième commande installe le module *Fabric* qui nécessite une compilation
du module *PyCrypto*.

La troisème commande affiche l'aide de la commande *fab* qui provient du module
*Fabric*.

Si tout se déroule bien pour ces étapes, vous êtes en bateau !

Environnements virtuels
=======================

Installer des paquets en Python à l'aide de pip ou easy_install demande par
défaut les accès administrateurs. Leur installation terminent également dans
votre installation système, ce qui peut causer des ennuis.

Pour remédier à ce problème, Vous pouvez créer un environnement virtuel:

.. code-block:: bash
    :linenos:
    
    sudo pip install virtualenv
    virtualenv monvenv
    source ./monvenv/bin/activate


Déploiement
~~~~~~~~~~~

Si vous publiez votre code par github, bitbucket ou similaire, il est recommandé
de fournir un fichier `requirements.txt` qui permet de recréer l'environnement
virtuel, soit les dépendances de votre projet:

.. code-block:: bash
    :linenos:

    pip freeze > ./requirements.py


Pour recréer votre environnement:

.. code-block:: bash
    :linenos:

    pip install -r ./requirements.txt


