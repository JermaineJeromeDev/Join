# Join

Join is a web-based task and contact management application created as a group project during the web development training at [Developer Akademie GmbH](https://developerakademie.com/). Authenticated users can manage tasks on a Kanban board and maintain a shared contact directory.

<details>
<summary>Deutsche Version anzeigen</summary>

Join ist eine webbasierte Aufgaben- und Kontaktverwaltung, die im Rahmen der Weiterbildung bei der [Developer Akademie GmbH](https://developerakademie.com/) als Gruppenprojekt erstellt wurde. Authentifizierte Benutzerinnen und Benutzer können Aufgaben auf einem Kanban-Board verwalten und ein gemeinsames Kontaktverzeichnis pflegen.

</details>

## Table of Contents

- [Features](#features)
- [Technology Stack](#technology-stack)
  - [Application](#application)
  - [Backend and data](#backend-and-data)
  - [Development and quality](#development-and-quality)
- [Prerequisites](#prerequisites)
- [Installation and start](#installation-and-start)
  - [Clone the repository](#1-clone-the-repository)
  - [Install dependencies](#2-install-dependencies)
  - [Start the development server](#3-start-the-development-server)
  - [Use the application](#4-use-the-application)
- [Available commands](#available-commands)
- [Project structure](#project-structure)
- [Routes](#routes)
- [Build](#build)
- [Contributing](#contributing)

## Features

- User registration, login, logout, and protected areas
- Summary dashboard with an overview of tasks
- Create, edit, delete, and manage tasks by status
- Kanban board with task statuses and task details
- Create, edit, view, and delete contacts
- Real-time synchronization of tasks and contacts through Supabase Realtime
- Help, privacy policy, and legal notice pages
- Responsive interface for desktop and mobile devices

<details>
<summary>Deutsche Version anzeigen</summary>

## Funktionen

- Registrierung, Login, Logout und geschützte Bereiche
- Zusammenfassung mit Überblick über Aufgaben
- Aufgaben erstellen, bearbeiten, löschen und nach Status verwalten
- Kanban-Board mit Aufgabenstatus und Aufgabendetails
- Kontakte anlegen, bearbeiten, anzeigen und löschen
- Echtzeit-Synchronisierung von Aufgaben und Kontakten über Supabase Realtime
- Hilfebereich, Datenschutz und Impressum
- Responsive Oberfläche für Desktop und mobile Geräte

</details>

## Technology Stack

### Application

- [Angular](https://angular.dev/) 21 as the frontend framework
- TypeScript 5.9 for application logic
- Angular Router for navigation and protected routes
- Angular Reactive Forms for forms and validation
- Angular Signals for local reactive state
- SCSS for global and component-specific styling
- RxJS for reactive programming within the Angular ecosystem

### Backend and data

- [Supabase](https://supabase.com/) as the backend-as-a-service platform
- Supabase Auth for registration and authentication
- Supabase Database for tasks and contacts
- Supabase Realtime for live data updates

### Development and quality

- Angular CLI 21.2.17
- npm as the package manager
- Vitest and JSDOM for unit tests
- Prettier for consistent formatting

<details>
<summary>Deutsche Version anzeigen</summary>

## Verwendete Technologien

### Anwendung

- [Angular](https://angular.dev/) 21 als Frontend-Framework
- TypeScript 5.9 für die Anwendungslogik
- Angular Router für Navigation und geschützte Routen
- Angular Reactive Forms für Formulare und Validierung
- Angular Signals für lokalen reaktiven Zustand
- SCSS für globale und komponentenbezogene Styles
- RxJS für reaktive Programmierung innerhalb des Angular-Ökosystems

### Backend und Daten

- [Supabase](https://supabase.com/) als Backend-as-a-Service
- Supabase Auth für Registrierung und Anmeldung
- Supabase Database für Aufgaben und Kontakte
- Supabase Realtime für Live-Updates der Daten

### Entwicklung und Qualität

- Angular CLI 21.2.17
- npm als Paketmanager
- Vitest und JSDOM für Unit-Tests
- Prettier für einheitliche Formatierung

</details>

## Prerequisites

Install the following before starting:

- [Node.js](https://nodejs.org/) in a current LTS version
- npm 11.9.0 or a compatible npm version
- [Git](https://git-scm.com/)

The application uses a configured Supabase project. The connection settings are stored in `src/environments/environment.ts`. To use your own Supabase project, replace the project URL and public publishable key there. Never put private keys in the frontend or commit them to the repository.

<details>
<summary>Deutsche Version anzeigen</summary>

## Voraussetzungen

Installiere vor dem Start:

- [Node.js](https://nodejs.org/) in einer aktuellen LTS-Version
- npm 11.9.0 oder eine kompatible npm-Version
- [Git](https://git-scm.com/)

Die Anwendung verwendet ein bereits konfiguriertes Supabase-Projekt. Die Verbindungsdaten liegen in `src/environments/environment.ts`. Falls eine eigene Supabase-Instanz verwendet werden soll, müssen dort die eigene Projekt-URL und der öffentliche Publishable Key eingetragen werden. Private Schlüssel dürfen nicht in das Frontend oder in das Repository gelangen.

</details>

## Installation and start

### 1. Clone the repository

```bash
git clone https://github.com/JermaineJeromeDev/Join.git
cd join-app
```

### 2. Install dependencies

```bash
npm install
```

### 3. Start the development server

```bash
npm start
```

Angular starts with the development configuration and normally opens the application at [http://localhost:4200](http://localhost:4200). If the browser does not open automatically, visit the address manually.

### 4. Use the application

Register a new account or sign in with an existing account to access protected features such as the Summary, Board, tasks, and contacts.

<details>
<summary>Deutsche Version anzeigen</summary>

## Installation und Start

### 1. Repository klonen

```bash
git clone https://github.com/miloo-p/join-app.git
cd join-app
```

### 2. Abhängigkeiten installieren

```bash
npm install
```

### 3. Entwicklungsserver starten

```bash
npm start
```

Angular startet mit der Development-Konfiguration und öffnet die Anwendung normalerweise automatisch unter [http://localhost:4200](http://localhost:4200). Falls der Browser nicht automatisch geöffnet wird, rufe die Adresse manuell auf.

### 4. Anwendung verwenden

Für geschützte Funktionen zuerst registrieren oder mit einem bestehenden Benutzerkonto anmelden. Danach stehen unter anderem Summary, Board, Aufgaben und Kontakte zur Verfügung.

</details>

## Available commands

| Command                            | Purpose                                                  |
| ---------------------------------- | -------------------------------------------------------- |
| `npm start`                        | Start the development server and open the application    |
| `npm run build`                    | Create a production build                                |
| `npm run watch`                    | Rebuild the development version automatically on changes |
| `npm test`                         | Run unit tests                                           |
| `npx ng generate component <name>` | Generate a new Angular component                         |

<details>
<summary>Deutsche Version anzeigen</summary>

## Nützliche Befehle

| Befehl                             | Zweck                                                      |
| ---------------------------------- | ---------------------------------------------------------- |
| `npm start`                        | Entwicklungsserver starten und die Anwendung öffnen        |
| `npm run build`                    | Produktions-Build erstellen                                |
| `npm run watch`                    | Development-Build bei Änderungen automatisch neu erstellen |
| `npm test`                         | Unit-Tests starten                                         |
| `npx ng generate component <name>` | Neue Angular-Komponente erzeugen                           |

</details>

## Project structure

```text
join-app/
├── public/assets/              Static images, icons, and fonts
├── src/
│   ├── app/
│   │   ├── layout/             Shared elements such as the header and sidebar
│   │   ├── pages/              Login, Summary, Board, contacts, and task pages
│   │   ├── shared/             Reusable components, services, and interfaces
│   │   ├── app.config.ts       Global Angular configuration
│   │   └── app.routes.ts       Routes and authentication guard
│   ├── environments/           Environment and Supabase configuration
│   ├── styles/                 Global SCSS architecture
│   ├── main.ts                 Application entry point
│   └── styles.scss             Global style entry point
├── angular.json                Angular CLI configuration
├── package.json                Dependencies and npm scripts
└── tsconfig*.json              TypeScript configuration
```

<details>
<summary>Deutsche Version anzeigen</summary>

## Projektstruktur

```text
join-app/
├── public/assets/              Statische Bilder, Icons und Fonts
├── src/
│   ├── app/
│   │   ├── layout/             Globale Elemente wie Header und Sidebar
│   │   ├── pages/              Seiten für Login, Summary, Board, Kontakte und Aufgaben
│   │   ├── shared/              Wiederverwendbare Komponenten, Services und Interfaces
│   │   ├── app.config.ts        Globale Angular-Konfiguration
│   │   └── app.routes.ts        Routen und Authentifizierungs-Guard
│   ├── environments/            Umgebungs- und Supabase-Konfiguration
│   ├── styles/                  Globale SCSS-Architektur
│   ├── main.ts                  Einstiegspunkt der Anwendung
│   └── styles.scss              Globaler Style-Einstiegspunkt
├── angular.json                 Angular-CLI-Konfiguration
├── package.json                 Abhängigkeiten und npm-Skripte
└── tsconfig*.json               TypeScript-Konfiguration
```

</details>

## Routes

| Route             | Purpose         | Access        |
| ----------------- | --------------- | ------------- |
| `/login`          | Sign in         | Public        |
| `/sign-up`        | Register        | Public        |
| `/`               | Summary         | Authenticated |
| `/board`          | Kanban board    | Authenticated |
| `/add-task`       | Create a task   | Authenticated |
| `/contacts`       | Manage contacts | Authenticated |
| `/help`           | Help            | Public        |
| `/privacy-policy` | Privacy policy  | Public        |
| `/legal-notice`   | Legal notice    | Public        |

<details>
<summary>Deutsche Version anzeigen</summary>

## Routen

| Route             | Zweck              | Zugriff         |
| ----------------- | ------------------ | --------------- |
| `/login`          | Anmeldung          | Öffentlich      |
| `/sign-up`        | Registrierung      | Öffentlich      |
| `/`               | Summary            | Authentifiziert |
| `/board`          | Kanban-Board       | Authentifiziert |
| `/add-task`       | Aufgabe erstellen  | Authentifiziert |
| `/contacts`       | Kontakte verwalten | Authentifiziert |
| `/help`           | Hilfe              | Öffentlich      |
| `/privacy-policy` | Datenschutz        | Öffentlich      |
| `/legal-notice`   | Impressum          | Öffentlich      |

</details>

## Build

Create a production build with:

```bash
npm run build
```

The generated files are placed in Angular's default `dist/` directory and can be served by a web server.

<details>
<summary>Deutsche Version anzeigen</summary>

## Build

Für einen Produktions-Build:

```bash
npm run build
```

Die fertigen Dateien werden im Angular-Standardverzeichnis `dist/` abgelegt und können anschließend über einen Webserver bereitgestellt werden.

</details>

## Contributing

- Develop changes in a dedicated feature or fix branch.
- Run `npm test` and `npm run build` before opening a pull request.
- Never commit credentials or private backend keys.
- Follow the existing Angular, TypeScript, and SCSS conventions.

<details>
<summary>Deutsche Version anzeigen</summary>

## Hinweise zur Mitarbeit

- Änderungen bitte in einem eigenen Feature- oder Fix-Branch entwickeln.
- Vor einem Pull Request `npm test` und `npm run build` ausführen.
- Zugangsdaten und private Backend-Schlüssel niemals committen.
- Bestehende Angular-, TypeScript- und SCSS-Konventionen im Projekt beibehalten.

</details>
