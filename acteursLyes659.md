```mermaid
classDiagram
    class Etudiant {
        +int id
        +String nom
        +String prenom
        +int age
        +String universite
        +String email
        +postulerLogement(Logement)
        +payerLoyer(Paiement)
    }

    class JeuneActif {
        +int id
        +String nom
        +String prenom
        +int age
        +String emploi
        +String email
        +postulerLogement(Logement)
        +payerLoyer(Paiement)
    }

    class Logement {
        +int id
        +String adresse
        +String type
        +float loyer
        +boolean disponible
        +afficherDetails
    }

    class Proprietaire {
        +int id
        +String nom
        +String email
        +ajouterLogement(Logement)
        +supprimerLogement(Logement)
    }

    class Agence {
        +int id
        +String nom
        +String adresse
        +String contact
        +gererLogement(Logement)
        +gererContrat(Contrat)
    }

    class Contrat {
        +int id
        +Date dateDebut
        +Date dateFin
        +float montant
        +signerContrat
    }

    class Paiement {
        +int id
        +Date datePaiement
        +float montant
        +String moyen
        +effectuerPaiement
    }

    %% Relations
    Etudiant --> Logement : "postule pour >"
    JeuneActif --> Logement : "postule pour >"
    Logement --> Proprietaire : "appartient à >"
    Logement --> Agence : "géré par >"
    Contrat --> Logement : "concerne >"
    Contrat --> Etudiant : "signé par >"
    Contrat --> JeuneActif : "signé par >"
    Paiement --> Contrat : "lié à >"
```
