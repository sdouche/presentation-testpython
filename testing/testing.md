!SLIDE subsection

# Stratégie de test

!SLIDE bullets
## Un test est composé de 4 parties
* Setup
* Exercice
* Vérification
* Teardown

!SLIDE bullets

# Fixture :
* minimal fixture
* standard fixture
* fresh fixture
* shared fixture
* backdoor

!SLIDE bullets

# Vérification des résultats
* état
* comportement
* assertion personnelle
* assertion delta
* assertion gardien
* assertion de test non finie

!SLIDE subsection

# Technique de test

!SLIDE smbullets incremental

# test fiable
* savoir quand les supprimer / modifier
* tester une seule chose à la fois
* facile à lancer
* gérer correctement la couverture de code
* tester le comportement, pas les méthodes
* assertion précise (pas de logique or, and, if, boucle)

!SLIDE smbullets incremental

# Test lisible
* nom compréhensible (décrivant un comportement)
* variable compréhensible
* séparer les actions des assertions
* des messages clairs
* forme canonique

!SLIDE smbullets incremental

# Test maintenable
* ne pas tester les méthodes privées
* supprimer la duplication
* setup maintenable
* tester l&#39;information et non la représentation
* découpler les tests (méthode helper)
* une condition par test
* une facette de l&#39;objet par test

!SLIDE

# Classification par
## Fixture / classe / fonctionnalité

!SLIDE

# Gérer les cas limites

!SLIDE subsection

# Framework d&#39;isolation

!SLIDE

# Stub (bouchon)
## "Indirect input"
## Vérifie l&#39;état

!SLIDE

# Spy
## "Indirect output"
## Contrôle à postériori
## Vérifie le comportement

!SLIDE

# Mock (simulacre)
## "Indirect output"
## Données / Attente
## Vérifie le comportement

!SLIDE

# Mock encourage à cacher l&#39;information non utile

!SLIDE bullets

## Ne pas mocker ce qu&#39;on ne peut
##  pas modifier, sauf
* si simuler le bon comportement est difficile
* gérer des cas extrèmes

!SLIDE

# Créer une trés fine couche d&#39;abstraction pour une API externe

!SLIDE 

# Un mock par test

!SLIDE

# Débat :
## TDD classique
## vs
## TDD mockiste

!SLIDE subsection

# Test smells

!SLIDE smbullets

# Code smells
* obscure code
* conditionnal test
* hard to test
* test code duplication
* test logic in production

!SLIDE smbullets

# Behavior smells
* assertion roulette
* erratic test
* fragile test
* frequent debugging
* manual intervention
* slow test

!SLIDE smbullets

# Projects smells
* buggy test
* developers not writing test
* high maintenance cost
* production bugs
