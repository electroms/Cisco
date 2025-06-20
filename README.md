

# Commandes Simples Cisco

Ce projet a pour objectif de vous guider à travers la configuration de base d’un réseau Cisco avec VLANs, trunks et routage inter-VLAN. Il s'adresse aux étudiants ou techniciens souhaitant renforcer leurs compétences en configuration réseau avec les équipements Cisco.

---

## Objectifs

Ce projet est divisé en plusieurs étapes :

1. **Création du réseau et configuration des paramètres de base des périphériques**
2. **Création des VLAN et attribution des ports de commutateur**
3. **Configuration d’un trunk 802.1Q entre les commutateurs**
4. **Configuration du routage inter-VLAN sur le routeur**
5. **Vérification du bon fonctionnement du routage inter-VLAN**

---

## Contexte / Scénario

Les VLAN (Virtual Local Area Network) permettent de segmenter un réseau local pour améliorer sa **scalabilité**, sa **sécurité** et sa **gestion**. La communication entre les VLANs nécessite un **périphérique de couche 3**, tel qu’un routeur.

Les trunks VLAN permettent d'étendre les VLANs à travers plusieurs périphériques, en transportant le trafic de plusieurs VLANs sur une seule liaison tout en maintenant leur isolation logique. Le routage inter-VLAN sera ici réalisé à l’aide d’un **Router-On-A-Stick**, une méthode utilisant une interface trunk entre le routeur et le commutateur.

Vous allez :

- Créer et tester des VLANs sur deux commutateurs.
- Configurer un trunk VLAN entre les commutateurs ainsi qu'entre le routeur et le commutateur.
- Mettre en place le routage inter-VLAN sur le routeur pour permettre la communication entre hôtes situés sur différents VLANs, quel que soit leur point de connexion.

---

## Matériel Requis

- 🖧 **1 Routeur** Cisco 4221 (IOS XE 16.9.4, image `universalk9` ou équivalent)
- 🔌 **2 Commutateurs** Cisco Catalyst 2960 (IOS 15.2(2), image `lanbasek9` ou équivalent)
- 💻 **2 PC** Windows avec un programme d’émulation de terminal (ex. : Tera Term)
- 🧵 **Câbles de console** pour la configuration initiale via le port console
- 🌐 **Câbles Ethernet** selon la topologie définie

---

## Remarques Importantes

- Les périphériques doivent être **réinitialisés sans configuration préalable**.
- En cas de doute, contactez votre **instructeur**.
- Les commandes peuvent varier selon le **modèle et la version IOS** des équipements.
- Consultez le **guide de l'instructeur** pour les étapes de réinitialisation et pour identifier les interfaces correctes.

---

## Auteur

> Cisco - Travaux Pratiques CCNA  
> Documentation et adaptation pour travaux pratiques sur matériel réel.
