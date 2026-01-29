# SECURITY_BASELINE — Socle de sécurité Zyqtron

## 1. Principe fondamental

La sécurité est prioritaire sur la performance, le confort et la rapidité.

Aucune fonctionnalité ne justifie :
- une fuite de données
- une perte de contrôle
- une dépendance irréversible

---

## 2. Souveraineté des données

Règles absolues :

- les données critiques sont locales par défaut
- aucune exfiltration automatique n’est autorisée
- le cloud est un outil, jamais un dépôt de vérité

Les données Zyqtron incluent :
- mémoires (Mnemosyne)
- journaux
- clés API
- configurations
- décisions stratégiques

---

## 3. Gestion des secrets

Les secrets incluent :
- clés API
- tokens
- certificats
- identifiants

Règles :

- jamais stockés en clair dans un repo
- jamais exposés à une IA externe
- accès restreint à Nemo + Zyqtron

Tout secret doit être :
- traçable
- révoquable
- remplaçable

---

## 4. IA locales vs IA cloud

### IA locales
- confiance prioritaire
- accès contrôlé à la mémoire
- pas d’accès réseau par défaut

### IA cloud
- consultatives uniquement
- aucune mémoire persistante
- aucune clé stratégique partagée
- réponses toujours recontextualisées

---

## 5. Accès réseau et web

Navigation web :
- toujours via agents dédiés
- jamais via Mnemosyne directement
- journalisation obligatoire

APIs externes :
- usage minimal
- quotas surveillés
- logs conservés

---

## 6. Sécurité du code

Pour tous les repos Zyqtron :

- audit avant intégration
- pas de dépendance non comprise
- pas de code opaque exécuté
- sandboxing privilégié

Les forks sont :
- analysés
- durcis
- adaptés
- jamais utilisés “en l’état” sans validation

---

## 7. Isolation et cloisonnement

Principes :

- chaque agent est isolé
- les privilèges sont minimaux
- aucune escalade silencieuse

En cas de doute :
- isolation immédiate
- analyse post-mortem
- mémoire ERROR créée

---

## 8. Traçabilité et journalisation

Tout événement critique doit être :
-- daté
- contextualisé
- attribué

Aucun événement important ne doit disparaître sans trace.

---

## 9. Incident et dérive

En cas de dérive détectée :

1. Arrêt ou isolement
2. Signalement à Zyqtron
3. Analyse par Nemo
4. Décision humaine
5. Mémoire ERROR enregistrée

---

## 10. Principe final

La sécurité n’est pas une contrainte.
C’est ce qui rend tout le reste possible.

Sans sécurité :
- pas de souveraineté
- pas de confiance
- pas de Zyqtron
