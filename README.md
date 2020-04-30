# -RADIUS-attributes-for-IPv6-Access-Networks-draft-ietf-radext-ipv6-access-16

Abstrait

   Ce document spécifie des attributs RADIUS IPv6 supplémentaires utiles dans
   déploiements de réseaux résidentiels à large bande. Les attributs, qui sont
   utilisé pour l'autorisation et la comptabilité, permettre l'attribution d'un hôte
   Adresse IPv6 et adresse du serveur DNS IPv6 via DHCPv6; affectation d'un
   Itinéraire IPv6 annoncé via la publicité du routeur; affectation d'un nom
   Pool de préfixes délégués IPv6; et attribution d'un pool IPv6 nommé pour
   adressage DHCPv6 de l'hôte.

Langue requise

   Les mots clés "DOIT", "NE DOIT PAS", "OBLIGATOIRE", "DOIT", "NE DOIT PAS",
   "DEVRAIT", "NE DEVRAIT PAS", "RECOMMANDÉ", "MAI" et "FACULTATIF" dans ce
   doivent être interprétés comme décrit dans la RFC 2119 [RFC2119].

Statut de ce mémo

   Ce projet Internet est soumis en pleine conformité avec la
   dispositions des BCP 78 et BCP 79.

   Internet-Drafts sont des documents de travail de l'Internet Engineering
   Groupe de travail (IETF). Notez que d'autres groupes peuvent également distribuer
   documents de travail sous forme de brouillons Internet. La liste des sites Internet actuels
   Drafts se trouve à http://datatracker.ietf.org/drafts/current/.

   Internet-Drafts sont des projets de documents valables pour une durée maximale de six mois
   et peut être mis à jour, remplacé ou obsolète par d’autres documents à tout
   temps. Il est inapproprié d'utiliser Internet-Drafts comme référence
   matériel ou de les citer autrement que comme «travaux en cours».

   Cette version Internet expirera le 16 août 2013.
   
   Table des matières

   1. Introduction . . . . . . . . . . . . . . . . . . . . . . . . . 3
   2. Scénarios de déploiement. . . . . . . . . . . . . . . . . . . . . 3
     2.1. Attribution d'adresse IPv6. . . . . . . . . . . . . . . . . 4
     2.2. Serveurs DNS. . . . . . . . . . . . . . . . . . . . . . . 4
     2.3. Informations sur la route IPv6. . . . . . . . . . . . . . . . . . 5
     2.4. Pool de préfixes IPv6 délégués. . . . . . . . . . . . . . . . 5
     2.5. Pool d'adresses IPv6 avec état. . . . . . . . . . . . . . . . 5
   3. Attributs. . . . . . . . . . . . . . . . . . . . . . . . . . 6
     3.1. Adresse IPv6 encadrée. . . . . . . . . . . . . . . . . . . 6
     3.2. Adresse DNS-Server-IPv6. . . . . . . . . . . . . . . . . 7
     3.3. Route-IPv6-Information. . . . . . . . . . . . . . . . . . 8
     3.4. Pool de préfixes IPv6 délégués. . . . . . . . . . . . . . . . 9
     3.5. Pool d'adresses IPv6 avec état. . . . . . . . . . . . . . . . dix
     3.6. Tableau d'attributs. . . . . . . . . . . . . . . . . . . dix
   4. Considérations relatives au diamètre. . . . . . . . . . . . . . . . . . . 11
   5. Considérations de sécurité. . . . . . . . . . . . . . . . . . . 11
   6. Considérations IANA. . . . . . . . . . . . . . . . . . . . . 11
   7. Remerciements. . . . . . . . . . . . . . . . . . . . . . . 12
   8. Références. . . . . . . . . . . . . . . . . . . . . . . . . . 12
     8.1. Références normatives . . . . . . . . . . . . . . . . . . . 12
     8.2. Références informatives. . . . . . . . . . . . . . . . . . 12
   Adresses des auteurs. . . . . . . . . . . . . . . . . . . . . . . . 13
