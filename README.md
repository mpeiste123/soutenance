

# Soutenance AJC- client CDR(Vers une plateforme omnicanale)

Ce dépôt contient le **support complet de la soutenance**
pour l'étude de cas **Client CDR**:
- **Cadrage et pilotage** d'une transformation digitale visant à 
   **réduire la friction de planification** , fiabiliser l'information,**accélérer le cycle commercial** (demande → devis → pré-réservation),via :
   -**un tunnel web**(demande/devi/prérésevation) déployé en statique.
   -une **démonstration vocalendar**(assistant vocal Whatsapp --> STT --> Google Calendar) présentée en vidéo avec des preuves à l'appui.
   
- objectif de la soutenance : démontrer une démarche **Chef de Projet IT** (cadrage, gouvernance, planning, risques, coûts, KPI, conduite du changement) + preuves de faisabilité (MVP).





## objectif ce qu le jury doit comprendre (objectif pédagogique)
le client CDR est un lieu de tournage/événementiel , nous exposons :

- ### Le problème :
 une planification manuelle(messages, appels , notes) + l'utilisation de Whatsapp --> **erreurs**
**doublons**, **pertes d'information**, **décalage du calendrier** et **lenteur commerciale**

- ### La Réponse cible:
 une plateforme ominicanale "low friction" qui conserve les usages en cours
(Google Calendar, WhatsApp) tout en apportant :

        - un **parcours Web qualifié**
         (demande --> préréservation --> pipeline)
        -un assistant vocal qui accélère la création et la modification 
           d'évènements et fiabilise le calendrier.


- **Le pilotage et gouvenance:**
 Objectifs SMART,
  KPIs et indicateurs de performance ,
  gouvernance/RACI,
  Gestion des risques,
  budget,planning.

  - **Conduite du changement**

   -  outils numériques produits:
   - tunnel testable (Web)
   - vocalendar(vidéo + captures
     + élémnts d validation)


## Structure du dépôt 
Arborescence (Github Pages compatible via '/docs')

- /docs/index.html : HUB de navigation (accès direct à tunnel/slides/vocalendar)
- /docs/slides/ : PDF: soutenance.pdf qui est le support ds slides + viewer web **index.html** (iframe du pdf)
- /docs/tunnel/ : tunnel statique  (pages HTML/css/assets)
  demandes/ devis/préréservation
     --**index.html**
     --**/pages**
     --**/CSS**
     --**/Assets**

- **/docs/vocalendar/** : démo + preuves(vidéo + liens + éléments de validation)
       --**index.html**

## Lancement rapide (local)
### Ouvrir le HUB
Ouvre docs/index.html dans un navigateur.
Aucun serveur requis (statique)

>Conseil : si ton navigateur bloque des ressources locales selon la config, lance un petit serveur local (optionnel) :
sous powershell : `python -m http.server 5500`
>   puis ouvre `http://localhost:5500/docs/`



## Déploiement GitHub Pages (option)
Le dossier docs/ est compatible avec GitHub Pages.

### Configuration (sur GitHub)
- Settings → Pages
- Source : `Deploy from a branch`
- Branch : `main`
- Folder : `/docs`

## 5) Contenu attendu pour la soutenance
Ce dépôt sert à soutenir un discours projet structuré :

- Contexte & diagnostic (irritants, risques opérationnels)
- Objectifs SMART & KPI
- Périmètre MVP / hors périmètre
- Gouvernance (RACI, comitologie, rôles)
- Roadmap (phases, jalons, livrables)
- Risques & plans de mitigation
- Estimation coûts / charges / dépendances
- Démo / preuves (tunnel + vocalendar)

---

## 6) Notes
- Le tunnel est volontairement simple : objectif **pédagogique** + **démonstration de faisabilité**
- Vocalendar est présenté comme un **MVP démontrable** : le focus est sur la valeur et la fiabilité du calendrier
- Cette version “Minimal sûr” vise la clarté, la traçabilité et la soutenabilité (audit / preuves)

---

## 7) Licence
À définir selon besoin (projet de soutenance).
