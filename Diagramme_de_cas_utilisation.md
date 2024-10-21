# Diagramme de Cas d'Utilisation

graph TB
    %% Actors as person symbols
    actor Utilisateur as "Utilisateur"
    actor Administrateur as "Administrateur"

    %% Use cases for Utilisateur
    subgraph "Fonctions Utilisateur"
        U1[Réserver un vol]
        U2[Consulter ses réservations]
        U3[Effectuer un paiement]
    end

    %% Use cases for Administrateur
    subgraph "Fonctions Administrateur"
        A1[Gérer les vols]
        A2[Gérer les avions]
        A3[Gérer les passagers]
        A4[Gérer les équipages]
        A5[Gérer les aéroports]
    end

    %% Relationships between Actors and Use Cases
    Utilisateur --> U1
    Utilisateur --> U2
    Utilisateur --> U3

    Administrateur --> A1
    Administrateur --> A2
    Administrateur --> A3
    Administrateur --> A4
    Administrateur --> A5
