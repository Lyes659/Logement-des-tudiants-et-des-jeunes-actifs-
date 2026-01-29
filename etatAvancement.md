```mermaid
gantt
    title Etat d'avancement de l'enquete sur le logement des étudiants et jeunes actifs
    dateFormat  YYYY-MM-DD
    excludes    weekends

    %% Travaux préliminaires et préparation
    section Travaux preliminaires
    Lecture du rapport et recherche documentaire        :done, t1, 2025-11-10, 3d
    Structuration journal de bord et prise de notes    :done, t2, after t1, 2d
    Finalisation 5W+1 et problématique V2             :done, t3, after t2, 2d
    Identification du terrain et contacts locaux       :done, t4, after t3, 3d

    %% Questionnaire
    section Questionnaire
    Élaboration questionnaire                          :done, q1, 2025-11-15, 5d
    Diffusion questionnaire (résidence/Facebook/WhatsApp) :active, q2, after q1, 7d
    Distribution photocopies aux connaissances        :done, q3, after q2, 3d
    Saisie des questions et réponses sur LimeSurvey   :todo, q4, after q2, 10d

    %% Entretiens
    section Entretiens
    Premiers entretiens étudiants                     :done, e1, after q2, 5d
    Entretiens programmés jeunes actifs               :todo, e2, after e1, 7d
    Entretiens supplémentaires résidence              :todo, e3, after e2, 5d
    Enregistrements audio/vidéo                        :todo, e4, after e3, 5d
    Témoignage personnel (audio/vidéo)                :todo, e5, after e4, 3d

    %% Analyse et synthèse
    section Analyse
    Analyse préliminaire questionnaire               :todo, a1, after q4, 5d
    Analyse des entretiens et verbatims              :todo, a2, after e5, 7d
    Croisement des données                            :todo, a3, after a2, 3d
    Rédaction synthèse finale                         :todo, a4, after a3, 5d

    %% Clôture
    section Cloture
    Fin de l'enquête                                  :milestone, end, after a4, 0d

```
