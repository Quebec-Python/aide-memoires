Québec-Python: Aide-mémoires pour nos ateliers et nos présentations
===================================================================

# Dépendances

* Python
* Module **sphinx**
* Module **sphinx-rtd-theme**

# Installation des dépendances pour générer la documentation

    $ virtualenv env
    $ source env/bin/activate
    $ pip install -r requirements.txt

# Générer la documentation

## Sous GNU/Linux

    $ make html
    
## Sous Windows

Faites rouler script *make.bat* avec l'option *html*