<h1 align="center" id="tuprel">TUPREL</h1>

<p align="center"><strong>Define the schema. Own the query.</strong></p>

<p align="center">
  A schema-first Java toolkit for typed PostgreSQL access.
</p>

<p align="center">
  <a href="https://github.com/tuprel/tuprel/blob/main/docs/getting-started/quickstart.md"><strong>Getting Started</strong></a> ·
  <a href="https://github.com/tuprel/tuprel/blob/main/docs/README.md"><strong>Documentation</strong></a> ·
  <a href="https://github.com/tuprel/tuprel"><strong>GitHub Repository</strong></a>
</p>

<p align="center">
  <a href="https://github.com/tuprel/tuprel/actions/workflows/ci.yml?query=branch%3Amain"><img src="https://img.shields.io/github/actions/workflow/status/tuprel/tuprel/ci.yml?branch=main&amp;label=CI&amp;style=flat" alt="CI on main" height="20"></a> <a href="https://github.com/tuprel/tuprel/actions/workflows/codeql.yml?query=branch%3Amain"><img src="https://img.shields.io/github/actions/workflow/status/tuprel/tuprel/codeql.yml?branch=main&amp;label=CodeQL&amp;style=flat" alt="CodeQL on main" height="20"></a>
  <br>
  <a href="https://github.com/tuprel/tuprel/blob/main/docs/getting-started/installation.md"><img src="https://img.shields.io/badge/Java-21-426A86?style=flat" alt="Java 21 baseline" height="20"></a> <a href="https://github.com/tuprel/tuprel/blob/main/examples/tuprel-playground/README.md#configure-a-dedicated-local-database"><img src="https://img.shields.io/badge/database-PostgreSQL-426A86?style=flat" alt="Database: PostgreSQL" height="20"></a>
  <br>
  <a href="https://github.com/tuprel/tuprel/blob/main/LICENSE"><img src="https://img.shields.io/badge/Apache%202.0-586069?style=flat" alt="Apache License 2.0" height="20"></a> <a href="https://github.com/tuprel/tuprel#compatibility-and-project-status"><img src="https://img.shields.io/badge/Development%20Preview-91651E?style=flat" alt="Status: Development Preview" height="20"></a>
</p>

<p align="center">
  <picture>
    <source media="(max-width: 480px) and (prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/tuprel/tuprel/addc7275ec85fbb7c2634e3494b45688a0848401/docs/assets/readme/workflow-mobile-dark.svg">
    <source media="(max-width: 480px)" srcset="https://raw.githubusercontent.com/tuprel/tuprel/addc7275ec85fbb7c2634e3494b45688a0848401/docs/assets/readme/workflow-mobile-light.svg">
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/tuprel/tuprel/addc7275ec85fbb7c2634e3494b45688a0848401/docs/assets/readme/workflow-dark.svg">
    <img src="https://raw.githubusercontent.com/tuprel/tuprel/addc7275ec85fbb7c2634e3494b45688a0848401/docs/assets/readme/workflow-light.svg" alt="Define models in schema.tuprel, generate Java code, use the type-safe client, and query PostgreSQL through your DataSource.">
  </picture>
</p>

## What is TUPREL?

TUPREL is an open-source, schema-first Java toolkit for PostgreSQL. Define your
models in [schema.tuprel](https://github.com/tuprel/tuprel/blob/main/docs/guides/schema.md)
and generate immutable model values, input builders and a
[type-safe Java client](https://github.com/tuprel/tuprel/blob/main/docs/guides/java-client.md).
Use your application's `DataSource`, connection pool and transaction boundaries.

**Development Preview, built from source.** Java 21 and PostgreSQL are the
baseline. There is no stable release or published Maven Central artifact yet.

## Why TUPREL?

- **Keep the model and client together.** Generate Java from one schema instead
  of maintaining matching persistence types and query helpers by hand.
- **Make database work explicit.** Compose
  [typed queries](https://github.com/tuprel/tuprel/blob/main/docs/guides/crud-and-queries.md),
  request [relations](https://github.com/tuprel/tuprel/blob/main/docs/guides/relations.md)
  deliberately, and choose your
  [transaction boundaries](https://github.com/tuprel/tuprel/blob/main/docs/guides/transactions.md).
  Getters never issue hidden queries.
- **Keep SQL inspectable.** Preview generated query SQL before execution.
  Values use bound parameters; the core has no dependency on JPA, Hibernate or Spring.

## How it works

1. **Define** models, fields and explicit relations in `schema.tuprel`.
2. **Generate** Java through the [CLI](https://github.com/tuprel/tuprel/blob/main/docs/reference/cli.md).
3. **Query** PostgreSQL using the generated client and your `DataSource`.

Generation writes Java files; it does not create database tables.
[Migrations](https://github.com/tuprel/tuprel/blob/main/docs/guides/migrations.md)
currently support offline drafts, read-only history/status and offline Java
preview/risk-plan APIs. Execution, deploy, dev, diff and physical drift detection
remain unavailable.

## Explore the project

Start with the [GitHub Repository](https://github.com/tuprel/tuprel) for source,
real Java examples and the complete supported surface. TUPREL is developed here
on GitHub; the repository and its documentation are the public reference.

## Getting Started

The [Quickstart](https://github.com/tuprel/tuprel/blob/main/docs/getting-started/quickstart.md)
builds the CLI and generates a client in a fresh project with JDK 21 and Git.
No database or Docker is needed for that first step. Follow
[Build from Source](https://github.com/tuprel/tuprel/blob/main/docs/getting-started/installation.md)
for launcher setup and integration into an existing Java project.

## Documentation and Examples

- [Documentation](https://github.com/tuprel/tuprel/blob/main/docs/README.md) — guides,
  reference and a path from schema to database access.
- [Java API](https://github.com/tuprel/tuprel/blob/main/docs/reference/java-api.md) —
  public entry points and generating JavaDoc from source.
- [CLI Reference](https://github.com/tuprel/tuprel/blob/main/docs/reference/cli.md) —
  available commands, configuration and exit codes.
- [Examples](https://github.com/tuprel/tuprel/blob/main/examples/tuprel-playground/README.md) —
  a standalone Java playground with typed queries, relations and transactions,
  using local PostgreSQL without Docker.

## Community and Contributing

Use [Issues](https://github.com/tuprel/tuprel/issues) for questions, reproducible
bugs and feature discussions. Read
[Contributing](https://github.com/tuprel/tuprel/blob/main/CONTRIBUTING.md) before
preparing a change. Report vulnerabilities privately through
[Security](https://github.com/tuprel/tuprel/blob/main/SECURITY.md).

TUPREL is licensed under the
[Apache License 2.0](https://github.com/tuprel/tuprel/blob/main/LICENSE).
