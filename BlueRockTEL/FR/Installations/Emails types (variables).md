## Emails types : variables disponibles

Voici sous forme de lexique les variables que vous pouvez utilser dans les [[Emails types]] emails types que vous configurez au moyen de BlueRockTEL.

### Modèle "Client" (customer)

    brand : marque dont dépend votre client, si vous avez configuré plusieurs marques dans BlueRockTEL (branding)
    name : raison sociale du client
    customerAccount : compte client, par défaut de type "CL001"
    accountsReference : compte client en comptabilité, si différente
    registrationNumber : numéro d'identification de l'entreprise, SIRET en France
    taxRegistrationNumber : numéro de TVA intracommunautaire
    mainContactFirstName : prénom du contact principal de l'entreprise cliente
    mainContactLastName : nom du contact principal
    type : type d'entreprise
    capital : capital de l'entreprise
    activityCode : code activité
    mainAddressLine1 : première ligne de l'adresse postale
    mainAddressLine2 : seconde ligne de l'adresse
    mainAddressPostalCode : code postal
    mainAddressCity : ville
    mainAddressCountry : pays
    emailAddress : adresse email principale de l'entreprise
    website : site web
    phone : téléphone
    fax : fax

### Modèle "Dossier de facturation" (customerFile)

    site : site installé
    siteId : un identifiant du site, le cas échéant, souvent une information provenant du client lui-même
    addressLine1 : première ligne de l'adresse postale du site
    addressLine2 : seconde ligne de l'adresse
    postalCode : code postal
    city : ville
    country : pays
    mandateIdentification : référence unique du mandat (RUM) sur lequel les prélèvements bancaires SEPA seront effectués
    mandateSignatureDate : date de signature du mandat SEPA
    servicesStart : date de début des services (au niveau du dossier, sachant que les services peuvent individuellement avoir des dates de début différentes)
    servicesStop : date de fin des services (au niveau du dossier, sachant que les services peuvent individuellement avoir des dates de fin différentes)
    billingFrequency : nombre de mois représentant la fréquence de facturation du dossier
    credit : solde créditeur du dossier client

### Modèle "Suivi d'installation" (customerFileSetup)

    requestedInstallationDate : date d'installation demandée puis prévue
    portabilityDate : date de portabilité
    deliveryDate : date de livraison

### Modèle "Organisation" (organisation)

    name : raison sociale
    registrationNumber : numéro d'identification de votre entreprise, SIRET en France
    taxRegistrationNumber : numéro de TVA intracommunautaire
    mainContactFirstName : prénom du contact principal
    mainContactLastName : nom du contact principal
    accountantFirstName : prénom du comptable
    accountantLastName : nom du comptable
    organisationType : type d'organisation
    currency : devise principale
    capital : capital de l'entreprise
    activityCode : code activité
    iban : votre IBAN
    bic : votre BIC
    ics : votre identifiant de créancier SEPA
    mainAddressLine1 : première ligne de votre adresse postale
    mainAddressLine2 : seconde ligne d'adresse
    mainAddressPostalCode : code postal
    mainAddressCity : ville
    mainAddressCountry : pays
    website : site web
    phone : téléphone principal de l'entreprise
    fax : fax