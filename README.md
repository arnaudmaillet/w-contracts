# Social Network Contracts

Ce dépôt contient les définitions Single Source of Truth (SSOT) de nos APIs via Protocol Buffers.

## 🛠 Tooling
Nous utilisons **Buf** pour le linting et la génération.
- Installation : `brew install bufbuild/buf/buf`

## 🚀 Workflows
1. **Linting** : `buf lint` (Vérifie le style et les conventions)
2. **Breaking Change Detection** : `buf breaking --against '.git#branch=main'` (Interdit de casser l'App Mobile)
3. **Generation** : `buf generate` (Génère le code Rust/Go/Kotlin)

## 🏗 Structure
- `proto/` : Définitions .proto organisées par domaine et version.
- Toutes les APIs doivent être versionnées (v1, v2...) pour supporter la rétrocompatibilité mobile.