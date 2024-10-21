# Diagramme de Cas d'Utilisation

```mermaid
graph TB
    subgraph Utilisateur
        U1[Réserver un vol]
        U2[Consulter ses réservations]
        U3[Effectuer un paiement]
    end

    subgraph Administrateur
        A1[Gérer les vols]
        A2[Gérer les avions]
        A3[Gérer les passagers]
        A4[Gérer les équipages]
        A5[Gérer les aéroports]
    end

    %% Relationships between Actors and Use Cases
    Utilisateur -->|1..*| U1
    Utilisateur -->|0..*| U2
    Utilisateur -->|1| U3

    Administrateur -->|1| A1
    Administrateur -->|1| A2
    Administrateur -->|1| A3
    Administrateur -->|1| A4
    Administrateur -->|1| A5
