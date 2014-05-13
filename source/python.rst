Python
======

Création de variables
---------------------

.. code-block:: python
   :linenos:
   
   un_bool = True # False
   
   un_chiffre = 1000
   
   chaine_de_caractere = "bacon ipsum"
   
   une_liste_mutable = [1, 2, 3, 4]
   
   une_liste_non_mutable = (1, 2, 3, 4)
   
   un_dictionnaire = {
       "une_cle": "une_valeur",
       "une_2e_cle": "une_2e_valeur"
   }
   
Opérations
----------

Arithmétique
~~~~~~~~~~~~

.. code-block:: python
   :linenos:
   
   x = 3
   y = 4
   
   # Addition
   x + y
   # Soustraction
   x - y
   # Multiplication
   x * y
   # Division
   x / y
   # Division entière
   x // y
   # Modulo (reste de la division)
   x % y
   # Puissance
   x ** y

Comparaison
~~~~~~~~~~~

.. code-block:: python
   :linenos:
   
   x = 3; y = 4; z = 5
   
   # Égalité
   (x == y, x != y)
   # Inégalité
   (x > y, x < y, x >= y, x <= y)
   # Chaînage de comparaisons
   x < y < z
   
Structures de contrôle
----------------------

*Si* logique
~~~~~~~~~~~~

.. code-block:: python
   :linenos:
   
   if une_condition:
       print "Oui"
   elif une_autre_condition:
       print "Non"
   else:
       print "Wat"

Boucle *For*
~~~~~~~~~~~~

.. code-block:: python
   :linenos:
   
   couleurs = ["rouge", "bleu", "vert"]
   
   for couleur in couleurs:
       print couleur

Les fonctions
-------------

.. code-block:: python
   :linenos:
   
   def bien_le_bonjour(prenom):
       """
       Cette fonction souhaite une bonne journée au prénom
       en paramètre
       """
       print "Bonjour {}".format(prenom)

   bien_le_bonjour("Bernard")

Les classes
-----------

.. code-block:: python
   :linenos:
   
   class Automobile:
       couleur = ""
       marque = ""
       position_x = 0
       position_y = 0
       
       def __init__(self, couleur, marque):
           """
           Un constructeur
           """
           self.couleur = couleur
           self.marque = marque
           
       def roule(self, x, y):
           """
           Roule ma boule !
           """
           self.position_x, self.position_y = x, y

Les modules
-----------

.. code-block:: python
   :linenos:
   
   from python import antigravity
   import random
   
   print random.shuffle([1, 2, 3])
   
