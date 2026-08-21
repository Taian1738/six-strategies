# 六韬（LT）

[中文](./README.md) · [English](./README.en.md) · [日本語](./README.ja.md) · [한국어](./README.ko.md) · [Español](./README.es.md)

Six Strategies est un protocole de collaboration en ingénierie logicielle pour Codex. Il organise les tâches complexes de développement, de correction, de refactorisation et de maintenance à long terme en un processus traçable et vérifiable.

## Fonctionnalités principales

- `R-` : documenter les exigences observables et les critères d’acceptation.
- `A-` : documenter l’architecture, les limites, les invariants et les décisions importantes.
- `F-` : diviser le travail en lots d’implémentation avec une propriété claire des fichiers.
- `T-` : fixer les tests, les commandes et les preuves vérifiables.
- Appliquer des contrôles dédiés à l’architecture fondamentale, aux contrats publics, aux permissions, aux migrations, à l’IPC, aux plugins, à la compilation et à la publication.

## Flux de travail

```text
Fixer les objectifs → évaluer l’impact → choisir l’architecture minimale
    → implémenter → vérifier → mettre à jour la mémoire → auditer → journaliser
```

SOL prend en charge l’architecture critique non figée, les contrats publics, l’implémentation critique indivisible et l’audit final. Luna prend en charge la collecte de faits ainsi que l’implémentation, la vérification et la journalisation lorsque les décisions et le périmètre sont déjà figés.

## Installation

[Téléchargez le ZIP depuis la Release](https://github.com/Taian1738/six-strategies/releases/download/v2026.08.21/ltskill-20260821-142646.zip), décompressez-le dans `<CODEX_HOME>/skills/ltskill/` en conservant la structure des répertoires, puis invoquez-le explicitement avec `$ltskill`.

Version du protocole : `LT-2026-08-21.11`


