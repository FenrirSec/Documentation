# Guidelines à destination des collaborateurs - Fenrir.pro

Ce guide contient des informations sur le déroulement des audits destiné aux collaborateur.ices de **fenrir.pro**, il détaille les différentes phases d'audit ainsi que le déroulé des missions et des intéractions entre les différents membres de l'équipe d'audit.

---

## Début d'un audit

Avant le démarrage d'un audit, certaines phases de documentations doivent être remplies afin de définir le contexte légal et de cadrer l'audit à venir.

### Ordre de mission

L'ordre de mission se doit d'être transmis par *fenrir.pro* aux différents tiers de l'audit, celui-ci contient le détail de la mission de du tiers :

- Sa durée
- Son objectif
- Autres éléments spécifiques à la mission

---

### Signature des documents

Avant le démarrage de la mission :

#### Autorisation d'Audit

L'autorisation d'audit devra être signée par *fenrir.pro* ainsi que par *les clients finaux de l'audit*.

#### Devis des auditeurs

Avant le démarrage de la mission, les devis de l'ensemble des *auditeurs* devront être envoyés à *fenrir.pro*.

#### NDA

Un *accord de non divulgation* devra être signé par tous les tiers participants à l'audit.

---

### Réunion de démarrage d'audit

Le début d'un audit est initié par une réunion de présentation du scope de l'audit par le chef de projet assigné à l'audit *@fenrir.pro*.

Au cours de cette réunion, seront présentés le **scope** de l'audit, le client concerné (dans les limites de sa confidentialité) ainsi que les conditions de l'audit.

---

## Fin d'un audit

### Réunion de fin d'audit

À la suite du rendu du livrable, une réunion de fin d'audit pourra être organisée entre la personne en charge du projet chez *fenrir.pro* et les différents prestataires pour faire un compte-rendu de fin de mission.

#### Rendu de la facture

Une facture devra être établie à la suite de l'audit par les différents prestataires impliqués.

---

## Phrases d'audit

Les phases d'audit suivante feront partie de la méthodologie utilisée au cours de l'audit : 

- Reconnaissance
- Scan
- Énumération
- Exploitation
- Effacement de traces

Cette méthodologie est inspirée de la méthodologie LTP d'EC-Council et de l'OSSTMM, le détail de ces phases est disponible à la suite de ce document et dans le fichier [Pentest-Methodology.md](Pentest-Methodology.md).

---

## Livrable

Un livrable devra être fourni à la suite de la mission, celui-ci contiendra l'ensemble du détail de l'audit effectué par l'auditeur.ice, à savoir pour chacune des phases d'audit :

- L'ensemble des informations découvertes ainsi que leur source précise, au format texte ainsi que si jugé nécessaire les captures d'écran associées
- L'ensemble de tests effectués ainsi que leurs lignes de commande et leur résultat au format texte ainsi que les captures d'écran associées. **Même les tests infructueux !**.
- L'ensemble des scripts et payloads réalisés et utilisés au cours de l'audit
- Les conseils de remédiation associés aux découvertes faites au cours de l'audit

---

### Contenu

Le livrable devra contenir : 

- Un document de **notes** qui retracera le détail de l'audit
- Un dossier de **captures d'écran**
- Un dossier de **scripts** contenant les scripts et exploits offensifs réalisés
- Un dossier contenant les **sorties** des différents scripts et outils de scan utilisés

---

### Format

Les notes devront être fournies au format *Markdown* suivant les guidelines de formatage de [GitHub](https://docs.github.com/fr/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

L'archive contenant le livrable devra être chiffrée à l'aide des algorithmes **AES-256** ou **AES-512** ainsi qu'une clé de chiffrement d'au minimum **12 caractères**.

Le format de l'archive pourra être une archive *7zip* ou autre supportant du chiffrement fort ou être un espace de partage sécurisé privé en ligne.


#### Arborescence

L'arborescence finale du livrable suivra le format suivant :

- notes.md
- *scripts*
    - bruteforce_otp.sh
- *screenshots*
    - otp_bypass.png
    - 500_registration.png
- *scripts_output*
     - testssl.sh.output.txt
     - nuclei.output.txt
     - nmap_sV.output.txt

---

## Détail des phases d'audit

Les phases d'audit suivantes devront être suivies par les auditeurs (à moduler en fonction de leur propre approche de la méthodologie d'audit) :

---

### Reconnaissance

La phase de reconnaissance consiste à utiliser des sources publiques (OSInt) pour découvrir des informations sur l'infrastructure technique (logicielle et materielle), organisationnelle (informations sur les équipes, les différents rôles ainsi que la gestion de l'organisation) et compétitive (produits, clientèle, stratégie) de la cible de l'audit.

---

### Scan

La phase de scan consiste des outils de scan pour découvrir des places d'adresse IP, hôtes, ports et services disponibles sur l'infrastructure cible.

Au cours de cette phase, la configuration des serveurs HTTP et HTTPS sera auditée.

Des scanners de vulnérabilités pourront également être utilisés dans les limites définies dans les conditions de l'audit.

---

### Énumération

La phase d'énumération consiste à utiliser des outils d'énumération ainsi que des clients "classiques" dans le but d'obtenir des informations sur les différents services découverts (HTTP, SSH, FTP, DNS etc...).

---

### Exploitation

La phase d'exploitation consiste à vérifier l'exploitabilité des vulnérabilités potentielles découvertes dans les phases précédentes ainsi que de tester les points d'entrée logiciels ainsi que le code associé pour des vulnérabilités de logique, d'implémentation ou autres.

---

### Effacemment de traces

Enfin, les comptes utilisateurs crées, fichiers ajoutés sur les serveurs et diverses traces laissées au cours des opérations d'audit seront retirés dans la mesure des permissions obtenues/accessibles.