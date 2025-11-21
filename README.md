# 🩺 Pulse AI — Système de santé intelligent pour l’Afrique

## 🌍 Aperçu général

**Pulse AI** est une plateforme intelligente conçue pour améliorer l’accès aux soins en Afrique grâce à l’intelligence artificielle, aux données hospitalières et à une architecture numérique adaptée au contexte local.  
Notre mission est de **rendre la santé accessible, connectée et efficace**, particulièrement dans les zones rurales.

Le système regroupe :  
- un **diagnostic intelligent** basé sur RAG + modèles open-source,  
- une **gestion intelligente des hôpitaux (SmartHosp)**,  
- un **chatbot de bien-être pour les jeunes (MindCare)**,  
- une **future fonctionnalité de traçabilité des médicaments (MedScan)**.

---

## 🚨 Problématique

L’Afrique fait face à plusieurs défis majeurs dans le domaine de la santé :

- 🌾 Accès limité aux soins dans les zones rurales,  
- 🏥 Surpopulation hospitalière et manque de gestion en temps réel,  
- 💊 Circulation de faux médicaments,  
- 😔 Stress et détresse psychologique croissants chez les jeunes,  
- 📍 Difficulté à trouver le bon hôpital selon les services réellement disponibles.

---

## 💡 Notre solution

Pulse AI propose quatre modules qui fonctionnent ensemble :

---

### 🩺 1. Diagnostic Intelligent (RAG + modèles biomédicaux open-source)

- Entrée utilisateur : **symptômes en texte ou voix**  
- Analyse via :
  - un modèle biomédical open-source HuggingFace,  
  - un **RAG médical** contenant des documents de symptômes/maladies.  
- L’IA génère :
  - un **diagnostic préliminaire**,  
  - un niveau de gravité,  
  - des premiers conseils.  

➡️ L’utilisateur peut ensuite demander une **liste d'hôpitaux adaptés**, même sans diagnostic, uniquement selon les services requis.

---

### 🏥 2. SmartHosp — Gestion intelligente des hôpitaux

Chaque hôpital dispose d’un **Dashboard web** pour :

- s’inscrire et présenter ses services médicaux disponibles,  
- déclarer :
  - le nombre de lits restants,  
  - les médecins présents,  
  - les heures de disponibilité,  
- mettre à jour les capacités en temps réel.

Le système calcule ensuite automatiquement un :

- **score d’hôpital**,  
- classement par distance (via OpenStreetMap),  
- classement par services compatibles.

---

### 💬 3. MindCare — Chatbot de bien-être (RAG)

MindCare accompagne les jeunes en leur offrant :

- conseils anti-stress,  
- méthodes de concentration,  
- soutien à la discipline scolaire,  
- exercices de respiration et relaxation,  
- légère détection de détresse émotionnelle.

Il fonctionne grâce à :

- un modèle open-source,  
- un RAG basé sur psychologie légère, motivation, bien-être.

---

### 💊 4. MedScan (module futur)

- Scan d’un médicament (photo, texte).  
- Vérification de l’authenticité via une base structurée.  
- Affichage de la composition, effets et risques.

---

## 🧠 Architecture technique

| Composant | Description | Technologies |
|----------|-------------|--------------|
| **Application mobile** | Interface du patient : diagnostic, chatbot, hôpitaux, MedScan. | Flutter, Dart, OpenStreetMap |
| **Dashboard web** | Module pour hôpitaux : services, lits, médecins. | HTML, CSS, JavaScript |
| **Backend / API** | Diagnostic, recommandation, chatbot, gestion hôpitaux. | FastAPI (Python) |
| **IA / ML** | RAG médical & bien-être, embeddings, modèles open-source. | HuggingFace, FAISS, Scikit-Learn |
| **Base de données** | Stockage du système. | PostgreSQL |
| **Déploiement** | Stack containerisée. | Docker + VPS |
| **Cartographie** | Distance & géolocalisation. | OpenStreetMap |
| **Collaboration** | Documentation & gestion d’équipe. | GitHub, Notion |

---

## 🔁 Fonctionnement global

1. L'utilisateur décrit ses symptômes.
2. Le backend active un modèle biomédical + RAG médical.
3. Pulse AI génère un diagnostic préliminaire.
4. SmartHosp recommande les hôpitaux selon services → distance → capacité.
5. Les hôpitaux mettent à jour leurs données via Dashboard.
6. MindCare accompagne l’utilisateur sur le plan mental.
7. MedScan permettra bientôt la vérification des médicaments.

---

## 🧰 Stack technologique

| Catégorie | Technologies |
|-----------|--------------|
| **Mobile** | Flutter, Dart |
| **Backend** | FastAPI |
| **IA** | Transformers, FAISS, Scikit-Learn |
| **Data** | Pandas, NumPy |
| **DB** | PostgreSQL |
| **Déploiement** | Docker, Nginx, VPS |
| **Map** | OpenStreetMap |

---

## 👩‍💻 Répartition de l’équipe

| Membre | Rôle | Responsabilités |
|--------|------|------------------|
| **DJOSSOU Light** | Data Science & Dev web| Diagnostic RAG, recommandation, Dashboard hôpitaux |
| **DOH Ben** | Dev Chatbot | Dév MindCare RAG, modèle open-source |
| **KOUMI Rejoice** | Dev Mobile | App Flutter, OpenStreetMap, Dashboard web |
| **SEGUE Freeman** | Backend Engineering | API FastAPI, PostgreSQL, intégration IA |

---

## 📊 Impact attendu

- 🏥 Optimisation des ressources hospitalières,  
- 🌾 Accessibilité accrue aux zones rurales,  
- 💊 Réduction des faux médicaments,  
- 💬 Amélioration du bien-être mental des jeunes,  
- 🧭 Orientation médicale plus précise et rapide.

---

## 🔮 Vision future

- Support vocal complet,  
- Diagnostic pour maladies tropicales,  
- Multilinguisme local (éwé, kabyè…),  
- IoT pour suivi de patients à distance,  
- Partenariats avec centres hospitaliers publics.

---

## ⚖️ Éthique et protection des données

- Données encryptées, anonymisées,  
- Pas de partage à des tiers,  
- Respect complet de l’éthique médicale,  
- L’IA ne remplace jamais un médecin.

---

## 📞 Contacts

**Projet :** Pulse AI  
**Email :** nethaniahdjossou@gmail.com  
**Pays :** Togo 🇹🇬  

---

✨ *Pulse AI — Rendre la santé intelligente, accessible et humaine pour l’Afrique.*
