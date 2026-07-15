<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/deebee-tech/.github/main/profile/assets/deebee-banner-dark.png">
    <img alt="DeeBee Tech" src="https://raw.githubusercontent.com/deebee-tech/.github/main/profile/assets/deebee-banner-light.png" width="460">
  </picture>
</p>

<p align="center"><strong>Build on the databases you already have.</strong></p>

---

## DeeBee

**DeeBee** is a data platform that sits on top of the databases you already run — Postgres, MySQL,
SQL Server, SQLite. Point it at a connection and it turns your tables into:

- **Datasets** — editable, partially-writable views over your data, edited in a fast grid or through generated forms.
- **Forms & views** — build data entry and read-only lenses on top of a dataset, no schema changes required.
- **Workflows** — automate the busywork: trigger on a data change, a schedule, or a manual action, with human-in-the-loop tasks and an inbox.
- **Audit trail** — every change captured before/after, with history and restore.
- **Roles & permissions** — control who can see and do what.

Writes go straight through to your source, or through a buffer when you want them staged and applied
on your terms — your data stays in **your** database, not locked inside ours. And it's built to be
extended: a contribution-point **plugin** model lets you add data sources, fields, and UI without
forking the core.

DeeBee is in active development and currently private. The packages below are the dependency-free
pieces we built it on, released for everyone.

## Open source

Everything here is MIT-licensed, typed, and made to do one thing well. We use all of it in production.

### SQLEasy — dialect-correct SQL, bring your own connection

A SQL _builder_, not a driver or an ORM. It composes correct SELECT / INSERT / UPDATE / DELETE — plus
CTEs, unions, and batched transactions — for Postgres, MySQL, SQL Server, and SQLite, and hands you
the query string and its bound parameters. You run it on the connection you already have.

- **[sqleasy](https://github.com/deebee-tech/sqleasy)** &nbsp;[![npm](https://img.shields.io/npm/v/@deebeetech/sqleasy?color=cb3837&logo=npm)](https://www.npmjs.com/package/@deebeetech/sqleasy) [![JSR](https://jsr.io/badges/@deebeetech/sqleasy)](https://jsr.io/@deebeetech/sqleasy) — the zero-dependency builder for TypeScript & JavaScript.
- **[sqleasy-engine](https://github.com/deebee-tech/sqleasy-engine)** &nbsp;[![npm](https://img.shields.io/npm/v/@deebeetech/sqleasy-engine?color=cb3837&logo=npm)](https://www.npmjs.com/package/@deebeetech/sqleasy-engine) — a thin, opt-in executor for what SQLEasy builds. One `run` / `transaction` / `explain` / `close` surface per dialect; you load only the driver you import.
- **[sqleasy-dart](https://github.com/deebee-tech/sqleasy-dart)** &nbsp;[![pub](https://img.shields.io/pub/v/sqleasy?logo=dart&color=0175C2)](https://pub.dev/packages/sqleasy) — the pure-Dart port. Flutter-ready (mobile, desktop & web), held byte-for-byte to the TypeScript original by a shared golden corpus.

### The toolkit — the small utilities

The dependency-free helpers underneath everything else. Each is a single focused package you can drop
in without pulling in a utility-library kitchen sink.

- **[is-helper](https://github.com/deebee-tech/is-helper)** &nbsp;[![npm](https://img.shields.io/npm/v/@deebeetech/is-helper?color=cb3837&logo=npm)](https://www.npmjs.com/package/@deebeetech/is-helper) [![JSR](https://jsr.io/badges/@deebeetech/is-helper)](https://jsr.io/@deebeetech/is-helper) — type-checking utilities and real type guards that never throw and see through realm boundaries and tag spoofing.
- **[array-helper](https://github.com/deebee-tech/array-helper)** &nbsp;[![npm](https://img.shields.io/npm/v/@deebeetech/array-helper?color=cb3837&logo=npm)](https://www.npmjs.com/package/@deebeetech/array-helper) [![JSR](https://jsr.io/badges/@deebeetech/array-helper)](https://jsr.io/@deebeetech/array-helper) — the array parts of Lodash and Underscore you actually reach for (`compact`, `orderBy`, `uniqBy`), without the weight.
- **[string-builder](https://github.com/deebee-tech/string-builder)** &nbsp;[![npm](https://img.shields.io/npm/v/@deebeetech/string-builder?color=cb3837&logo=npm)](https://www.npmjs.com/package/@deebeetech/string-builder) [![JSR](https://jsr.io/badges/@deebeetech/string-builder)](https://jsr.io/@deebeetech/string-builder) — a lightweight, chainable string builder for TypeScript & JavaScript.

## About

**DeeBee Tech** is the home of the DeeBee platform and the open-source packages above. Find the
packages on [npm](https://www.npmjs.com/org/deebeetech) and [JSR](https://jsr.io/@deebeetech), or
start with any repo — each ships with a full README and examples.
