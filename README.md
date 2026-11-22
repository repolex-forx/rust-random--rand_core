# Repolex Knowledge Graph of rust-random/rand_core

RDF knowledge graph data for [rust-random/rand_core](https://github.com/rust-random/rand_core), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download rust-random/rand_core
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 5cd7df496d0bff1d95534ac8b66a2610f5bf7808
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 5cd7df496d0bff1d95534ac8b66a2610f5bf7808.nq.gz
│   └── repolex
│       └── 5cd7df496d0bff1d95534ac8b66a2610f5bf7808
│           └── chunk-001.nq.gz
├── blob
│   ├── 02ac88f06733c976e59c09d92b25464e596418fd.nq.gz
│   ├── 03ae5e3c887584580cbe539039b4172bdd51e34c.nq.gz
│   ├── 093433dffb3a724b03a8cb0b8ba3a1270bacfebc.nq.gz
│   ├── 0c24730f7b6992419911dff445e779aa2a29ddff.nq.gz
│   ├── 15bbeb52c1d80595a6706f1c523291b909476bd4.nq.gz
│   ├── 22b1e8da2f557a60db8399dcab560a9ffb4f599e.nq.gz
│   ├── 3e0dd6b4f5b828d61a7d0d692b3fa31e69182311.nq.gz
│   ├── 455787c2334661b0c74590c1d35e5f711393cb82.nq.gz
│   ├── 47519016b5d0f668c6605361dbbab83a635fc926.nq.gz
│   ├── 603fd20fa3e212ede08ed77c6b9d726cda5792aa.nq.gz
│   ├── 68c41ac798970779b9d66b3c1a236b0b3c2f54e6.nq.gz
│   ├── 6bb2c641dee4e18bd3e427b3d09396d2c79768ec.nq.gz
│   ├── 88964fe576ff2415eeb4d335616b258c3c0f72ba.nq.gz
│   ├── 8a8354bd5d3c4fb0271eda1234efe5375ed9b03c.nq.gz
│   ├── 90c57c87bcd80d1be9978d4284f35f5c85bb9357.nq.gz
│   ├── a18219b4e0418d84a7c99ef9e3ba84a9fc00e76a.nq.gz
│   ├── a3e76cabdc9bc90e7e8c16d4a42abb5845c3d7e0.nq.gz
│   ├── a9d366d2c42ebd1288e25923249c2afb143cb6d8.nq.gz
│   ├── a9d37c560c6ab8d4afbf47eda643e8c42e857716.nq.gz
│   ├── ab7c7a83e00d2c38ba3419c280065194fd7cdbe9.nq.gz
│   ├── b07ef8a6fc43afc71e1f355241bcad956d96ada0.nq.gz
│   ├── da1082af52999b8b0a86cb9eed5396bd7a516508.nq.gz
│   ├── dce6a4bcc4eb5623867faa23979fe70b21ae362e.nq.gz
│   ├── de038c33b4fc9dfca7a1f89686f134f3e58b048f.nq.gz
│   ├── e260055561b0f655bc067c294968b3cd2b0423e2.nq.gz
│   └── ef8181835aaa01651dd0c2d922884fca9d42ce50.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 5cd7df496d0bff1d95534ac8b66a2610f5bf7808.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

14 directories, 35 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[rust-random/rand_core](https://github.com/rust-random/rand_core)

---
*Parsed on 2026-11-22 by [repolex](https://repolex.ai)*
