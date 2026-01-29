# MEMORY_TYPES — Typologie de la mémoire Zyqtron

## 1. Principe fondateur

Toute mémoire est une **représentation**, jamais une vérité absolue.

Chaque entrée mémoire doit :
- être contextualisée
- être datée
- être attribuée
- être révisable

La mémoire sert à **éclairer la décision**, jamais à la remplacer.

---

## 2. Catégories fondamentales de mémoire

Mnemosyne gère plusieurs types de mémoire distincts.
Chaque type a un rôle, des règles et un poids différent.

---

## 3. Types de mémoire

### 3.1 FACT (Fait)

Contenu :
- informations factuelles
- observations vérifiables
- événements datés

Exemples :
- “Le serveur a redémarré à 03:12”
- “Le repo X a été forké le 2026-01-28”

Contraintes :
- source obligatoire
- révision possible si le fait est infirmé

---

### 3.2 DECISION (Décision)

Contenu :
- décisions prises par Zyqtron
- arbitrages validés
- choix stratégiques

Exemples :
- “Mnemosyne est la mémoire centrale”
- “Mistral est l’IA souveraine prioritaire”

Contraintes :
- traçabilité humaine
- jamais modifiable sans nouvelle décision explicite

---

### 3.3 HYPOTHESIS (Hypothèse)

Contenu :
- suppositions
- interprétations
- pistes non confirmées

Exemples :
- “Ce repo pourrait améliorer la RAG”
- “Cette architecture semble plus robuste”

Contraintes :
- doit rester marquée comme incertaine
- peut évoluer vers FACT ou être abandonnée

---

### 3.4 ERROR (Erreur)

Contenu :
- bugs
- mauvaises décisions
- hallucinations détectées
- fausses croyances passées

Exemples :
- “Cette information s’est révélée fausse”
- “Cette approche a généré une dérive”

Contraintes :
- ne jamais être supprimée
- utilisée comme signal d’apprentissage

---

### 3.5 CONTRADICTION (Contradiction)

Contenu :
- conflits entre sources
- désaccords entre IA
- divergences mémoire / réalité

Exemples :
- “Deux sources donnent des réponses opposées”
- “La mémoire A contredit la mémoire B”

Contraintes :
- conserver toutes les versions
- signaler explicitement le conflit

---

### 3.6 INSIGHT (Insight)

Contenu :
- compréhensions nouvelles
- synthèses transverses
- prises de recul

Exemples :
- “La RAG doit toujours être remise en question”
- “La hiérarchie réduit les dérives”

Contraintes :
- subjectif assumé
- toujours contextualisé

---

### 3.7 TASK (Tâche)

Contenu :
- actions à effectuer
- travaux en cours ou passés

Exemples :
- “Auditer le repo mnemosyne”
- “Créer le SECURITY_BASELINE”

Contraintes :
- statut clair (à faire / fait / abandonné)
- historique conservé

---

### 3.8 META (Méta-mémoire)

Contenu :
- règles du système
- réflexions sur la mémoire elle-même
- ajustements cognitifs

Exemples :
- “La mémoire a tendance à surpondérer X”
- “Ce type de donnée génère des biais”

Contraintes :
- accès restreint (Nemo + Zyqtron)
- haute valeur stratégique

---

## 4. Pondération par défaut

Chaque type de mémoire a un poids initial :

- FACT : élevé
- DECISION : très élevé
- ERROR : élevé
- CONTRADICTION : élevé
- INSIGHT : moyen
- HYPOTHESIS : faible à moyen
- TASK : contextuel
- META : critique

Ces pondérations sont **évolutives**, jamais figées.

---

## 5. Interaction avec Nemo

Nemo doit :

- identifier le type de chaque mémoire
- signaler les erreurs et contradictions
- ne jamais transformer une hypothèse en fait sans validation
- privilégier les décisions humaines

---

## 6. Principe final

La mémoire n’est pas un dogme.  
La contradiction est une richesse.  
L’erreur est un carburant.

Mnemosyne se souvient.
Nemo interprète.
Zyqtron tranche.
