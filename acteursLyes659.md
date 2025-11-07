
```mermaid
classDiagram
    logement <|-- privé
    logement <|-- état
    logement <|-- association
    logement : +in propriétaire 
    logement : +locataire
    logement : +crous
    logement : +studapart
    
    class privé{
      +entreprise
      +locataire
      +agence immobiliére
    }
    
    class état{
      -details sur l'état physique
      -date de mise a jour
    }
    
    class association{
      +Union Nationale des Étudiants de France
      
    }
