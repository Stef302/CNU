# 🌌 Chronomètre National Universel (CNU)
> **Système de Référence Temporel Décimal & Relativiste**

---

Le **Chronomètre National Universel (CNU)** est une œuvre de design spéculatif et un simulateur physique interactif. Ce cadran spatiotemporel réinvente la mesure du temps en substituant l'asymétrie du calendrier grégorien et du système sexagésimal par une **matrice de 13 mois parfaits**, une **heure décimale stricte**, et un **moteur de correction relativiste** basé sur les équations d'Albert Einstein et de Hubble-Lemaître.

Conçu comme une interface de terminal haute fidélité à encre électronique (*e-ink*), le projet est entièrement autonome (Single Page Application), codé en JavaScript pur et stylisé avec Tailwind CSS.

---

## 🛠️ Spécifications du Système

### 1. La Matrice Calendaire (13 Mois • 28 Jours)
Le calendrier s'affranchit des irrégularités civiles pour proposer une symétrie mathématique absolue :
* **Régularité Cosmique** : L'année compte exactement 364 jours divisés en 13 mois de 28 jours.
* **Alignement Perpétuel** : Tous les mois débutent rigoureusement un **Lundi** et s'achèvent un **Dimanche**.(avec bientôt un renommage)
* **Planificateur Intégré** : Un agenda dynamique permet de programmer des événements sur les cycles décimaux d'une journée, avec import/export `JSON`.
* **Pont Civil (ICS)** : Un pipeline d'export génère instantanément un fichier de traduction `.ics` pour synchroniser la grille du CNU avec Google Calendar, Apple Calendar ou Outlook.

### 2. L'Écoulement Décimal & Quantification
* **Division Métrique** : La journée est partitionnée en 100 *Centidays* ($cd$), eux-mêmes divisés en *Millidays* et *Microdays*.
* **Chronons Discrets ($\theta_c$)** : Le temps est quantifié à l'échelle de la microseconde sous forme de paquets d'énergie temporelle cumulés en temps réel :
  $$\theta_c = \lfloor t_{\text{ms}} \cdot 10^{12} \cdot \gamma \rfloor$$

---

## 📐 Métriques & Référentiels Physiques

Le CNU embarque trois modèles de physique relativiste commutables, modifiant l'affichage et l'écoulement du temps selon votre position dans le cosmos :

| Référentiel | Paramètre Réglable | Phénomène Physique Simulé |
| :--- | :--- | :--- |
| **Terrestre** | Altitude ($0 \to 8848\text{ m}$) & Longitude | Dérive d'Einstein ($\gamma$) gravitationnelle locale et décalage du Midi Solaire. |
| **Pulsar (XNAV)** | Distance Galactique ($0 \to 2000\text{ Mpc}$) | Redshift cosmologique de Hubble-Lemaître ($1+z$) ralentissant la fréquence reçue d'un pulsar. |
| **Trou Noir** | Distance à la Singularité ($0.1 \to 5.0\ R_s$) | Dilatation extrême de Schwarzschild et inversion de la métrique temporelle sous l'horizon. |

### Les Formules du Moteur Temporel

> **Dilatation Gravitationnelle d'Einstein (Champ Faible)**
> $$dt' = dt \left(1 + \frac{g \cdot h}{c^2}\right)$$
> *Chaque mètre d'altitude ($h$) diminue le potentiel gravitationnel terrestre, accélérant de manière infime mais réelle le cadran du CNU.*

> **Métrique de Schwarzschild (Trou Noir)**
> $$d\tau = dt \sqrt{1 - \frac{R_s}{r}}$$
> *À l'approche de l'horizon des événements ($r \to 1.0\ R_s$), le temps propre de l'observateur ($\tau$) s'arrête relativement à l'Univers distant.*

> **Expansion Cosmique (Loi de Hubble-Lemaître)**
> $$z = \frac{H_0 \cdot D}{c} \quad \implies \quad f_{\text{reçue}} = \frac{f_{\text{nominale}}}{1 + z}$$
> *La distance de la galaxie ($D$) étire la longueur d'onde du signal périodique du pulsar PSR J0437-4715, ralentissant sa fréquence de pulsation sur l'oscilloscope.*

---

## 🎨 Design & Esthétique

Le cadran a été pensé pour les amateurs de rigueur scientifique et de minimalisme fonctionnel :
* **Palette Sombre / Claire Clinique** : Un contraste binaire à l'esprit papier électronique (*e-ink*), commutable d'un clic.
* **Oscilloscope Vectoriel (Canvas)** : Un oscilloscope dynamique dessine la forme d'onde atténuée et décalée par l'effet Doppler cosmologique en temps réel.
* **Typographies Monospacées** : Intégration de *JetBrains Mono* pour garantir l'alignement parfait des tableaux de données.

---

## 🚀 Déploiement Express

Puisque l'application est contenue dans **un seul fichier HTML auto-suffisant**, son exécution est instantanée.

```bash
# 1. Cloner le projet
git clone [https://github.com/votre-compte/cnu-matrice-spatiotemporelle.git](https://github.com/votre-compte/cnu-matrice-spatiotemporelle.git)

# 2. Naviguer dans le dossier
cd cnu-matrice-spatiotemporelle

# 3. Lancer l'interface (ou double-cliquez simplement sur le fichier HTML)
open chronom_tre_national_universel_cnu_matrice_spatiotemporelle.html
