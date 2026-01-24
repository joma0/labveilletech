+++
date = '2026-01-24T11:57:03+01:00'
draft = false
title = 'Développement "test-driven" et "behavior-driven"'
categories = [
    "développement",]
tags = ["test-driven", "tdd", "behavior-driven", "bdd"]
+++

Le développement d'une application métier nécessite une collaboration et des discusssions entre plusieurs parties prenantes, issues de domaines différents et avec des exigences, des besoins et des objectifs différents.

Cela peut s'avérer être un réel défi. Dans un article du blog CircleCI, l'auteur présente une stratégie pour rendre cette collaboration un peu plus aisée. Il s'agit de combiner 2 méthodes existantes : le développement "test-driven" et le développement "behavior-driven".

Le développement "test-driven" consiste à écrire les tests automatisés avant d'implémenter les fonctionnalités correspondantes. Cette approche permet un développement itératif et une validaition régulière de la viabilité du code.

Le développement "behavior-driven" vient compléter l'approche "test-driven". Ici le but est de partir des attentes côté métier, souvent exprimées sous forme de user stories et de les traduire en tests automatisés, pour enfin implémenter les fonctionnalités qui correspondent. Ainsi, on ne valide plus uniquement la viabilité technique du code, mais on s'assure que les fonctionnalités sont implémentées de façon à correspondre au comportement de l'utilisateur réel.

Un autre point essentiel de l'approche "behavior-driven" consiste à utiliser des termes qui parlent aussi bien aux développeurs qu'aux parties prenantes du côté métier. On utilise pour cela le format suivant :
Given _Some initial condition_ => Sous certaines conditions
When _Something happens_ => Quand qqch ce produit
Then _I expect this behavior_ => Alors je m'attends à ce comportement

### Conclusion

Grâce à cette approche, toutes les personnes impliquées partagent un langage commun et peuvent ainsi s'assurer dêtre sur la même longeur d'onde. Les collaborateur métier peuvent comprendre ce que font les développeurs et sont plus à l'aise pour poser des questions ou émettre une opinion, ce qui sera bénéfique car l'application répondra alors vraiment à leurs besoins.

### Sources

- SCHMITT Jacob, "Understanding enterprise application development", _circleci_, [en ligne], 09.03.2025. Disponible à l'adresse : https://circleci.com/blog/understanding-enterprise-application-development/ [consulté le 24.01.2026].
- SCHMITT Jacob, "Test-driven development (TDD) explained", _circleci_, [en ligne], 03.03.2025. Disponible à l'adresse : https://circleci.com/blog/test-driven-development-tdd/ [consulté le 24.01.2026].
- SCHMITT Jacob, "What is Behavior-Driven Development (BDD)?", _circleci_, [en ligne], 11.02.2025. Disponible à l'adresse : https://circleci.com/blog/what-is-behavior-driven-development/ [consulté le 24.01.2026].
