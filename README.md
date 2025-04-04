# Rust Chat Application

A simple client-server chat application built in Rust.

## Overview

This project implements a basic TCP-based chat application with a client and server component. The application allows multiple clients to connect to a central server and exchange messages in real-time.

## Features

- Multi-client support
- Non-blocking I/O for efficient network operations
- Simple command interface (`:quit` to exit)
- Terminal-based user interface

## Project Structure

The project consists of two main components:

- **Server**: Handles connections from multiple clients and broadcasts messages
- **Client**: Connects to the server, sends and receives messages

## Getting Started

### Prerequisites

- Rust and Cargo (1.63.0 or newer recommended)

### Running the Server

```bash
cd server
cargo run
```

The server will start on `127.0.0.1:6000`.

### Running the Client

```bash
cd client
cargo run
```

The client will attempt to connect to the server at `127.0.0.1:6000`.

## Usage

1. Start the server
2. Launch one or more client instances
3. Type messages in any client to broadcast them to all connected clients
4. Type `:quit` to exit a client

## Technical Details

- Uses Rust's standard library TCP networking
- Implements non-blocking I/O for efficient network operations
- Uses channels for thread communication
- Simple message format with fixed-size buffers

## License

This project is open source and available under the MIT License.

---

# Application de Chat en Rust

Une application de chat client-serveur simple construite en Rust.

## Aperçu

Ce projet implémente une application de chat basique sur TCP avec un composant client et un composant serveur. L'application permet à plusieurs clients de se connecter à un serveur central et d'échanger des messages en temps réel.

## Fonctionnalités

- Support multi-client
- E/S non-bloquante pour des opérations réseau efficaces
- Interface de commandes simple (`:quit` pour quitter)
- Interface utilisateur en mode terminal

## Structure du Projet

Le projet se compose de deux composants principaux :

- **Serveur** : Gère les connexions de plusieurs clients et diffuse les messages
- **Client** : Se connecte au serveur, envoie et reçoit des messages

## Démarrage

### Prérequis

- Rust et Cargo (version 1.63.0 ou plus récente recommandée)

### Lancement du Serveur

```bash
cd server
cargo run
```

Le serveur démarrera sur `127.0.0.1:6000`.

### Lancement du Client

```bash
cd client
cargo run
```

Le client tentera de se connecter au serveur à l'adresse `127.0.0.1:6000`.

## Utilisation

1. Démarrez le serveur
2. Lancez une ou plusieurs instances de client
3. Tapez des messages dans n'importe quel client pour les diffuser à tous les clients connectés
4. Tapez `:quit` pour quitter un client

## Détails Techniques

- Utilise la bibliothèque standard de Rust pour le réseau TCP
- Implémente des E/S non-bloquantes pour des opérations réseau efficaces
- Utilise des canaux pour la communication entre threads
- Format de message simple avec des tampons de taille fixe

## Licence

Ce projet est open source et disponible sous la licence MIT.
