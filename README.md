# 🩺 Pulse AI — Système de santé intelligent pour l’Afrique

## 🌍 Aperçu général

**Pulse AI** est une plateforme intelligente basée sur l’intelligence artificielle, conçue pour améliorer l’accès aux soins médicaux en Afrique.  
Notre objectif est de **rendre la santé plus accessible, connectée et efficace**, surtout dans les zones rurales.  
Le système combine **diagnostic intelligent**, **gestion en temps réel des hôpitaux**, **soutien à la santé mentale** et **traçabilité des médicaments** au sein d’un même écosystème.

---

## 🚨 Problématique

L’Afrique fait face à de nombreux défis dans le secteur de la santé :

- 🌾 Accès limité à des soins médicaux qualifiés dans les zones rurales,  
- 🏥 Surpopulation hospitalière et mauvaise répartition des ressources,  
- 💊 Circulation de faux médicaments et manque d’informations sur les traitements,  
- 😔 Montée du stress et de la dépression chez les jeunes sans accompagnement adapté.

---

## 💡 Notre solution

**Pulse AI** propose une approche complète et intégrée à travers quatre modules clés :

### 🩺 1. Diagnostic Intelligent
- L’utilisateur saisit ses **symptômes (texte, voix ou image)**.  
- L’IA, entraînée à partir de données médicales, **propose un diagnostic préliminaire** et des **recommandations de traitement de base**.  
- Ensuite, elle suggère des **centres médicaux ou hôpitaux à proximité** selon :
  - le taux d’occupation,  
  - le nombre de lits et médecins disponibles,  
  - la distance et la spécialisation.  
- Basé sur **Vertex AI AutoML** et **Google Maps API**.

### 🏥 2. Gestion intelligente des hôpitaux
- Chaque hôpital dispose d’un **tableau de bord web** pour :
  - enregistrer le nombre de lits disponibles,  
  - indiquer les médecins présents et leurs horaires,  
  - signaler l’état des stocks de médicaments.  
- Ces données sont synchronisées avec la plateforme centrale pour **optimiser la répartition des patients et des ressources**.  
- Les administrateurs hospitaliers accèdent aussi à des **statistiques et rapports analytiques**.

### 💬 3. MindCare — Chatbot de santé mentale
- Un **assistant conversationnel** qui discute avec les jeunes, détecte les signes de stress ou de mal-être et propose :
  - des conseils personnalisés,  
  - des activités relaxantes,  
  - ou une orientation vers un professionnel.  
- Propulsé par **Gemini API (Vertex AI)** pour offrir des échanges naturels et empathiques.

### 💊 4. MedScan (fonctionnalité à venir)
- Permettra de **scanner un médicament** (code-barres, texte, photo) pour :
  - vérifier son authenticité,  
  - connaître sa composition et ses effets.  
- Basée sur **GCP Vision API** et une base de données de produits certifiés.

---

## 🧠 Architecture technique

| Composant | Description | Technologies |
|------------|--------------|---------------|
| **Application mobile** | Application Flutter pour les patients (diagnostic, MindCare, MedScan). | Flutter, Dart |
| **Tableau de bord web** | Interface de gestion pour les hôpitaux. | HTML, CSS & Javascript|
| **Backend / API** | Point central de communication entre l’application, le tableau de bord et les modèles IA. | FastAPI (Python) |
| **Infrastructure IA** | Entraînement, hébergement et déploiement des modèles. | Python(scikitlearn, TensorFlow, Numpy, Pandas,Seaborn ...), Google Vertex AI (Custom Training, Gemini, Vision) |
| **Base de données** | Gestion des utilisateurs, hôpitaux, diagnostics et logs. | PostgreSQL / Firestore |
| **Hébergement** | Déploiement des APIs et dashboards. | Google Cloud Run, Firebase |

---

## 🔁 Fonctionnement global

1. **Entrée utilisateur**  
   Le patient saisit ses symptômes ou pose une question via la voix ou le chat.
2. **Traitement IA**  
   Les données sont envoyées à **Vertex AI** pour analyse (modèle Custom Training).  
3. **Recommandation médicale**  
   L’application affiche le diagnostic estimé et propose un hôpital disponible.  
4. **Synchronisation hospitalière**  
   Les hôpitaux mettent à jour leurs données (lits, médecins, horaires).  
5. **Support mental**  
   L’utilisateur peut discuter avec **MindCare**, le chatbot de santé mentale.  
6. **Traçabilité médicamenteuse (future étape)**  
   Le module MedScan permettra la vérification et l’éducation médicale.

---

## 🧰 Stack technologique

| Catégorie | Outils / Technologies |
|------------|----------------------|
| **Frontend** | Flutter (mobile), HTML, CSS & Javascript(web) |
| **Backend** | FastAPI / Node.js |
| **IA & ML** | Vertex AI Custom Training, Gemini API, Vision API |
| **Base de données** | PostgreSQL, Firestore |
| **Cloud** | Google Cloud Platform (Cloud Run, Vertex AI, Storage) |
| **API externes** | Google Maps API |
| **Collaboration** | GitHub, Notion, Google Workspace |
| **Design / Maquettes** | Figma, Material Design |

---

## 👩‍💻 Répartition de l’équipe

| Membre | Rôle | Responsabilités |
|--------|------|------------------|
| DJOSSOU Light | Data Scientist | Préparation des datasets, entraînement du modèle (Custom Training), intégration et deploiement |
| DOH Ben |Développeur du ChatBot  | Entraine et deploie le modèle du chatbot |
| KOUMI Rejoice | Développeur Full-Stack | Application mobile + Dashboard web |
| SEGUE Freeman | Développeur Backend | Conception des APIs, gestion des données, intégration cloud |

---

## 📊 Impact attendu

- 🏥 **Optimisation des ressources hospitalières** grâce à la data en temps réel.  
- 🌾 **Accès facilité à la santé** dans les zones rurales et isolées.  
- 💊 **Réduction des faux médicaments** et amélioration de la confiance médicale.  
- 💬 **Soutien psychologique accessible** pour les jeunes Africains.  

---

## 🔮 Vision future

- Intégration de **capteurs IoT** pour le suivi des patients à distance.  
- Extension du diagnostic aux **maladies tropicales locales**.  
- Ajout du **multilinguisme** (français, éwé, hausa, anglais).  
- Partenariats avec les **ministères de la santé** et hôpitaux publics.  
- Utilisation de la **data pour la recherche épidémiologique**.

---

## ⚖️ Éthique et protection des données

- Conformité aux normes **RGPD** et respect de la vie privée.  
- Données anonymisées et stockées de façon sécurisée.  
- L’IA ne remplace pas les médecins : elle **assiste** et oriente.  
- Promotion d’une **IA éthique, inclusive et transparente** pour l’Afrique.

---

## 📞 Contacts

**Nom du projet :** Pulse AI  
**Pays :** Togo 🇹🇬  
**Email :** nethaniahdjossou@gmail.com  


---

✨ *Pulse AI — Rendre la santé intelligente, accessible et humaine pour l’Afrique.*
