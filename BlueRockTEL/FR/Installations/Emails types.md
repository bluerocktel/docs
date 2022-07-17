Les emails types de BlueRockTEL sont des modèles d'emails (templates) que vous pouvez appeler depuis vos installations types. Un cas courant : le fait de renseigner la date de portabilité du dossier envoie automatiquement un email d'information au client.

## Création des emails types et insertion de variables

Vous pourrez accéder aux emails types depuis le menu "Configuration / Emails types". Depuis l'index, vous pouvez créer un nouvel email type, éditer ou supprimer un modèle existant. Il est également possible de dupliquer un email type, ce qui permet de gagner du temps de configuration.

Outre le texte de l'email type, vous devrez configurer les destinataires, à la fois dans votre entreprise et dans l'entreprise cliente. Dans votre entreprise, il peut s'agir du technicien, du commercial ou de l'ADV en charge du dossier, mais également du manager de facturation ou du manager technique. Dans l'entreprise cliente, il peut s'agir des destinataires des factures, des contacts techniques ou des signataires du contrat.

Pour personnaliser vos emails types, vous pouvez insérer des variables provenant de plusieurs modèles de BlueRockTEL :

- Client (customer)
- Dossier de facturation (customerFile)
- Suivi d'installation (customerFileSetup)
- Organisation (organisation)

Pour appeler une variable d'un modèle, la syntaxe à utiliser est de type:

```
{{ $model->variable }}
```

Par exemple, pour appeler la variable 'site' du modèle 'customerFile', vous écrirez dans votre email type :

```
{{ $customerFile->site }}
```

Vous pourrez formater les dates de la façon qui vous convient le mieux, par exemple :

```
Nous vous confirmons votre date de portabilité le {{ $customerFileSetup->portablityDate->format('d/m/Y') }}
```

ou, si vous voulez indiquer le jour et l'heure :

```
Nous vous confirmons votre date de portabilité le {{ $customerFileSetup->portabilityDate->format('d/m/Y') }} à {{ $customerFileSetup->portabilityDate->format('H:i') }}
```

