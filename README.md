# TP1 — Serveur HTTP

Ce TP est destiné aux étudiants d'EPITA SIGL 2026 dans le cadre du cours de SOCRA.

## Objectif

Votre mission est de **servir une première version de votre application So-Close** sur le domaine qui vous est attribué.

URL attendue :  
`http://so-close.groupeXX.socra-sigl.fr`
(sans HTTPS obligatoire, sauf en bonus)

---

## Infrastructure fournie

- Une machine virtuelle (VM) Linux avec une IP publique
- Un nom de domaine associé à votre groupe (via DNS déjà configuré)
- Une clé SSH privée pour vous connecter (authentification par mot de passe désactivée)

---

## À vous de jouer!

- Utilisez la clé privée fournie pour vous connecter à votre machine de binôme

```bash
ssh -i <chemin_vers_votre_cle_privee> sigl@so-close.groupXX.socra-sigl.fr
```

> Remplacez groupXX par le numéro de votre groupe, et adaptez le chemin vers votre clé selon votre système d’exploitation.

- Créez votre page web qui doit contenir:

  - Le nom du projet : So-Close
  - Une description en quelques phrases de ce que vous voulez construire (votre vision)
  - Le nom des membres du binôme
  - Un logo qui claque

> 💡 Astuce: vous pouvez créer votre page HTML sur votre ordinateur personel puis l'envoyer sur votre serveur
> en utilisant la commande `scp -i <chemin/vers/votre_clé_privée> index.html sigl@so-close.groupXX.socra-sigl.fr:/home/sigl`

**Bonus** : Activer HTTPS avec Let's Encrypt

> 💡 Astuce : vous pouvez utiliser `Certbot` avec `NGINX`, cela vous facilitera la tâche!
