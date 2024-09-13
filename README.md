
# République du Sénégal

## Un Peuple – Un But – Une Foi

**Ministère de l’Enseignement Supérieur et de la Recherche**

### Université Alioune DIOP de Bambey  
**Centre des Ressources de Dakar**

### Master 1  
**Data Science et Génie logiciel**

## PROJET DE MÉMOIRE

**Professeur :** Malick Mbengue  
**Présenté par :** M. Abou Bacre SALL

**Année académique 2023-2024**

---

## Table des matières

- [Avant-propos](#avant-propos)  
- [Introduction](#introduction)  
- Première Partie : Déploiement d'un Projet Full-Stack avec Docker et Kubernetes  
  1. [Architecture du système](#architecture-du-système)  
  2. [Mise en œuvre technique](#mise-en-œuvre-technique)  
  3. [Résultats et Tests](#résultats-et-tests)  
  4. [Problèmes rencontrés et Solutions](#problèmes-rencontrés-et-solutions)  
- Deuxième Partie : Déploiement des Applications WordPress et PhpMyAdmin sur Kubernetes  
  5. [Architecture du système](#architecture-du-système)  
  6. [Mise en œuvre technique](#mise-en-œuvre-technique-1)  
  7. [Résultats et Tests](#résultats-et-tests-1)  
  8. [Problèmes rencontrés et Solutions](#problèmes-rencontrés-et-solutions-1)  
  9. [Conclusion et Recommandations](#conclusion-et-recommandations)  
  10. [Annexes](#annexes)

---

## Avant-propos

Ce projet vise à appliquer et maîtriser les concepts fondamentaux de la virtualisation et de la containerisation vus en cours de Virtualisation et Conteneurisation lors de notre formation en Master 1 Data Science et Génie Logiciel.

Docker est une plateforme open-source permettant de créer, déployer et exécuter des applications dans des conteneurs. Kubernetes (K8s) est une plateforme open-source qui automatise le déploiement, la mise à l’échelle et la gestion des applications conteneurisées. Ce rapport présente le processus de mise en place et de configuration des applications en deux phases : un projet full-stack déployé sur Kubernetes, et un environnement web comprenant MySQL, WordPress et PHPMyAdmin.

---

## Introduction

Le déploiement d’une application était autrefois fastidieux, mais grâce à Docker et Kubernetes, cette opération est beaucoup plus fluide. Ce projet a pour but de maîtriser les fondamentaux de ces outils en déployant des applications sur un cluster Kubernetes. Le projet est divisé en deux parties :  
1. Un déploiement d’une application full-stack (Flask, React, MySQL)  
2. Un déploiement de MySQL, WordPress et PhpMyAdmin.

---

## Première Partie : Déploiement d'un Projet Full-Stack avec Docker et Kubernetes

### Architecture du système

L’application full-stack est structurée en trois composants : le backend (Flask), le frontend (React), et une base de données MySQL. Chaque composant est encapsulé dans des conteneurs Docker, facilitant leur gestion et le déploiement sur Kubernetes.

### Mise en œuvre technique

Nous avons créé les images Docker pour le backend et le frontend, configuré les fichiers YAML (deployments, services, configmaps, secrets, PVC), et déployé le tout sur Kubernetes. Les images Docker sont stockées dans DockerHub et utilisées pour les déploiements.

### Résultats et Tests

Les tests ont été effectués sur une machine virtuelle, et l'application a pu être accédée via l’IP de la machine. Les prédictions ont été listées et supprimées avec succès.

### Problèmes rencontrés et Solutions

Quelques problèmes ont été rencontrés (permissions Docker, erreurs de conversion en base64, "ImagePullBackOff") mais ont été résolus, assurant un déploiement fonctionnel.

---

## Deuxième Partie : Déploiement des Applications WordPress et PhpMyAdmin sur Kubernetes

### Architecture du système

Le système comprend MySQL pour stocker les données, WordPress pour l'accès et l'affichage des informations, et PhpMyAdmin pour administrer la base de données via une interface graphique.

### Mise en œuvre technique

Des fichiers YAML ont été créés pour chaque composant (deployments, services, configmaps, secrets, PVC) et déployés sur Kubernetes. WordPress et PhpMyAdmin sont accessibles via des ports NodePort.

### Résultats et Tests

Les services ont été vérifiés avec succès, et WordPress et PhpMyAdmin sont accessibles via les IP spécifiées.

### Problèmes rencontrés et Solutions

Des problèmes liés à la configuration de MySQL, WordPress, et des secrets ont été rencontrés mais résolus avec une révision des fichiers YAML.

---

## Conclusion et Recommandations

Ce projet nous a permis de maîtriser les concepts fondamentaux de la virtualisation et de la containerisation avec Docker et Kubernetes. En déployant une application full-stack et un environnement WordPress sur Kubernetes, nous avons compris l'importance de la gestion des ressources, des secrets, et des volumes persistants. L’intégration de ces déploiements dans un environnement cloud pourrait offrir de nouvelles opportunités d'amélioration.

--- 

## Annexes

(Captures d’écran, fichiers YAML, etc.)
