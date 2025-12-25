# Ontologie de l'Enseignement Supérieur

Projet réalisé dans le cadre d’un cours sur les technologies du Web sémantique.

## 🎯 Objectif
Modéliser le domaine de l’**enseignement supérieur** à l’aide d’une ontologie OWL, en couvrant les principaux concepts (établissements, programmes, cours, enseignants, étudiants, diplômes, ressources) et leurs relations.

## 🛠️ Technologies utilisées
- **Protégé** (version 5.x) pour la création et l’édition de l’ontologie
- **OWL** (Web Ontology Language)
- **SPARQL** pour les interrogations
- Exports en **RDF/XML** (`.owl`) et **Turtle** (`.ttl`)

## 📂 Structure du repository
- `enseignement-superieur.owl` → Ontologie complète au format RDF/XML (format standard OWL)
- `enseignement-superieur.ttl` → Version Turtle (plus lisible)
- `captures/` → Captures d’écran :
  - `ontograph.png` → Graphe global de l’ontologie (OntoGraph)
  - `sparql-*.png` → Exemples de requêtes SPARQL avec résultats

## 🔑 Concepts principaux
### Classes
- **Institution** → University (Public/Private), Department, ResearchLab
- **Program** → BachelorProgram, MasterProgram
- **Course** → CoreCourse, ElectiveCourse
- **Person** → Student (Undergraduate/Graduate), Teacher (Professor/Assistant)
- **Diploma**
- **Resource** → Library, OnlineResource

### Propriétés principales
- Objet : `offersProgram`, `enrolledIn`, `teaches`, `supervises`, `includesCourse`, `awards`, `hasDepartment`, `usesResource`
- Datatype : `hasName`, `hasID`, `hasDuration`, `hasECTS`, `hasLevel`, `hasEnrollmentYear`

### Exemples d’individus
- Université de Paris
- Licence Informatique (3 ans)
- Master IA
- Étudiants : Jane Doe, John Smith
- Enseignants : Prof. Dupont, Assistant Martin
- Cours : Introduction à l’IA, Machine Learning, etc.

## ❓ Exemples de requêtes SPARQL
(À exécuter dans Protégé ou tout endpoint SPARQL)

1. Cours enseignés par Prof. Dupont
2. Programmes offerts par l’Université de Paris
3. Étudiants inscrits en licence
4. Cours avec plus de 5 ECTS
5. Tous les noms d’étudiants

## 🚀 Perspectives
- Intégration avec FOAF ou schema.org
- Ajout de règles SWRL
- Connexion à une base de données réelle

## 📄 Licence
Projet académique – libre d’utilisation et de réutilisation à des fins éducatives.

N’hésite pas à me contacter pour toute question ou suggestion !

---
Adouko Loïc Ivan AHOULOU – Décembre 2025
