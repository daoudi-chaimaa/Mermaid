#j'ai utilisé le siteweb suivant planttext

@startuml
skinparam backgroundColor #f7f7f7
skinparam class {
    BackgroundColor<<actor>> #FFDDC1
    BorderColor<<actor>> #FF851B
    BackgroundColor<<system>> #D1E8FF
    BorderColor<<system>> #2C82C9
    ArrowColor #333
}

actor Utilisateur <<actor>> #FFDDC1
actor Administrateur <<actor>> #FFDDC1

rectangle "Système" <<system>> {
    Utilisateur --> (Réserver un vol)
    Utilisateur --> (Consulter ses réservations)
    Utilisateur --> (Effectuer un paiement)
    Utilisateur --> (S'authentifier)

    Administrateur --> (Gérer les vols)
    Administrateur --> (Gérer les avions)
    Administrateur --> (Gérer les passagers)
    Administrateur --> (Gérer les équipages)
    Administrateur --> (Gérer les aéroports)
    Administrateur --> (S'authentifier)
}
@enduml
