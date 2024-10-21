# Diagramme de Cas d'Utilisation

```mermaid
graph TD
    subgraph Utilisateur
        A1[Réserver un vol]
        A2[Consulter ses réservations]
        A3[Effectuer un paiement]
    end

    subgraph Administrateur
        B1[Gérer les vols]
        B2[Gérer les avions]
        B3[Gérer les passagers]
        B4[Gérer les équipages]
        B5[Gérer les aéroports]
    end

    Utilisateur -->|1..*| A1
    Utilisateur -->|0..*| A2
    Utilisateur -->|1| A3

    Administrateur -->|1| B1
    Administrateur -->|1| B2
    Administrateur -->|1| B3
    Administrateur -->|1| B4
    Administrateur -->|1| B5
