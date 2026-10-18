# Clé publique de signature CypherLux

Les fichiers publiés par CypherLux — sur https://www.cypherlux.fr
(C-Connect, Chiffre AES) et dans les livraisons remises aux organisations —
sont signés au format [minisign](https://jedisct1.github.io/minisign/)
avec cette clé :

```
RWRDFMSvr7njjYZCargtRF8huyMwp/S/uVt8PCn/ejIAyqril+jBOzkB
```

Fichier de clé : [`cypherlux-signature.pub`](cypherlux-signature.pub).

## Pourquoi ce dépôt

Ce dépôt est un **second canal**, indépendant du site : si le site était
compromis, un attaquant pourrait y remplacer à la fois un fichier, sa
signature et la clé affichée. La clé ci-dessus doit être **identique** à
celle affichée sur la page Téléchargements du site.

## Vérifier un fichier

Dans le dossier du fichier téléchargé, avec son `.minisig` à côté :

```
minisign -Vm NOM_DU_FICHIER -P RWRDFMSvr7njjYZCargtRF8huyMwp/S/uVt8PCn/ejIAyqril+jBOzkB
```

Réponse attendue : `Signature and comment signature verified`.

`minisign` : https://github.com/jedisct1/minisign/releases (Linux,
Windows, macOS), ou le paquet `minisign` de votre distribution.

## Changement de clé

Toute nouvelle clé serait annoncée ici, dans l'historique de ce dépôt,
avant d'être utilisée.
