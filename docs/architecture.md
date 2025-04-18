# Architecture Overview

## Tech Stack
- **Frontend**: Blazor WebAssembly (offline-first with SQLite).
- **Backend**: .NET Core API + Entity Framework.
- **Database**: SQL Server (cloud) + SQLite (local).

## Data Flow
1. User input → Encrypted local storage → Sync to cloud.
2. GDPR workflows: Anonymize/delete data on demand.

## Modular Features
- Premium features loaded dynamically via `IFeature` interfaces.