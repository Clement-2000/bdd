# Projet BDD - Gestion du parc véhicules STCP

L'entreprise publique **Sociedade de Transportes Colectivos do Porto** (Société de Transports Collectifs de Porto) fournit une offre de transports de passagers au sein de la ville de Porto (Portugal). La société fait appel à notre service informatique pour mettre en place un système d'information afin de classer ses véhicules de transports de passagers. L'étude initiale consiste à mettre en œuvre une base de données relationnelles à partir d'un simple cahier des charges définissant les contraintes suivantes :

# Cahier des charges initial

Un véhicule dispose d'un ensemble châssis-carroserie-moteur-boite de vitesses, d'un numéro de châssis unique, d'une date de mise en service, d'un historique de numéros d'identification, d'un historique d'immatriculations, d'un historique de réseaux, d'un historique des exploitants et d'informations complémentaires sous forme de texte. 

Pour chaque véhicule doit figurer une liste d'informations essentielles :
* Numéro de chassis du véhicule
* Date de première mise en service du véhicule
* État du véhicule (à venir, en service, réformé, etc...)
* Détails techniques du véhicule
    * Châssis
        * Fabriquant
        * Nom
        * Type
        * Informations complémentaires
    * Carroserie
        * Fabriquant
        * Nom
        * Informations complémentaires
    * Moteur
        * Fabriquant
        * Nom
        * Puissance
        * Carburant
        * Norme anti-pollution
        * Informations complémentaires
    * Boîte de vitesses
        * Fabriquant
        * Nom
        * Nombre de rapports
        * Informations complémentaires
* Historique des réseaux
    * Nom
    * Date de début
    * Date de fin
    * Informations complémentaires
* Historique des exploitants
    * Nom
    * Date de début
    * Date de fin
    * Informations complémentaires
* Historique des numéros de parc
    * Numéro de parc
    * Date de début
    * Date de fin
    * Informations complémentaires
* Historique des immatriculations
    * Numéro d'immatriculation
    * Date de début
    * Date de fin
    * Informations complémentaires
* Informations complémentaires

## Identification des entités

A partir de ce cahier des charges on relève le nom des entités les plus importantes et les informations qui y sont liées :
1. Le Véhicule
2. Le Châssis
3. La Carroserie
4. Le Moteur
5. La Boîte de vitesses
6. Le Fabriquant
7. Le Réseau
8. L'Exploitant

## Entité-Association

Les associations relient les entités entre elles. On rélève les associations à partir de phrases (Sujet-Verbe-Complément) du
cahier des charges. Le Verbe représente l'association entre deux entités (Sujet, Complément).

### Identification des associations

1. L'association Véhicule - Réseau
2. L'association Vehicule - Exploitant
3. L'association Véhicule - Numéro de parc
4. L'association Véhicule - Numéro d'immatriculation
5. L'association Véhicule - Châssis - Carroserie - Moteur - Boite de vitesses
