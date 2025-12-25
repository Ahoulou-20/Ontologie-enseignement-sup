# Ontologie de l'Enseignement Supérieur

Projet réalisé dans le cadre d’un cours sur les technologies du Web sémantique.

## 🎯 Objectif
Modéliser le domaine de l’**enseignement supérieur** à l’aide d’une ontologie OWL, en couvrant les principaux concepts (établissements, programmes, cours, enseignants, étudiants, diplômes, ressources) et leurs relations.

## 🛠️ Technologies utilisées
- **Protégé** (version 5.x) pour la création et l’édition de l’ontologie
- **OWL** (Web Ontology Language)
- **SPARQL** pour les interrogations
- Exports en **RDF/XML** (`.owl`) et **Turtle** (`.ttl`)

## 📂 Structure du repository (élément clés)
- `enseignement-superieur.owl` → Ontologie complète au format RDF/XML (format standard OWL)
- `enseignement-superieur.pdf` → rapport détaillé

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

## 🚀 Perspectives
- Intégration avec FOAF ou schema.org
- Ajout de règles SWRL
- Connexion à une base de données réelle

## 📄 Licence
Projet académique – libre d’utilisation et de réutilisation à des fins éducatives.

N’hésite pas à me contacter pour toute question ou suggestion !

---
Adouko Loïc Ivan AHOULOU – Décembre 2025
