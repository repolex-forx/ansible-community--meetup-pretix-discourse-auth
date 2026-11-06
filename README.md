# Repolex Knowledge Graph of ansible-community/meetup-pretix-discourse-auth

RDF knowledge graph data for [ansible-community/meetup-pretix-discourse-auth](https://github.com/ansible-community/meetup-pretix-discourse-auth), parsed by [repolex](https://repolex.ai).

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
rlex download ansible-community/meetup-pretix-discourse-auth
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── dac1e5ea2e8786bbef633c917c020f0b1966572b
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── dac1e5ea2e8786bbef633c917c020f0b1966572b
│           └── chunk-001.nq.gz
├── blob
│   ├── 06bf6e846def8ebb67457d0a275162ca514f6cfb.nq.gz
│   ├── 0742a35e04ea043184d4c5759a8dc87064289b06.nq.gz
│   ├── 0f6b8f8e4fd1efebd6d6babe9df4caf3e7d8b8b1.nq.gz
│   ├── 261eeb9e9f8b2b4b0d119366dda99c6fd7d35c64.nq.gz
│   ├── 2e423ff1aceb44b2b2563a9ec548c770dba9a924.nq.gz
│   ├── 3163d84aecc0a1cc5bff12f3a8c6cb19c7f9f516.nq.gz
│   ├── 413bde92f049e64c5615721febb7af3e017a1077.nq.gz
│   ├── 47498ee8eb178090bf2619b194464752b66abb95.nq.gz
│   ├── 558b8d46e81023074d5d1936cb34cfd46867e6cf.nq.gz
│   ├── 606849326a4002007fd42060b51e69a19c18675c.nq.gz
│   ├── 61742f5f64a2c68ddc249cfc672e57bf0f6d08d5.nq.gz
│   ├── 6ec6352742f03a9c6edbe75f9c26512133f10f39.nq.gz
│   ├── 787ec3466c5d1628d9381b3267e403c6867d83d4.nq.gz
│   ├── 7fbe9334326fb76e9d045ec90e3e2a45f80a01f9.nq.gz
│   ├── 82285fde4cf8bd2ea4261ebf392d84a6e1968f8f.nq.gz
│   ├── 949d280fe90df2ffeaf061fa70ea7c4eaf0de598.nq.gz
│   ├── 9913ac68985e29a34ffd68472de7ea55aa5b1020.nq.gz
│   ├── 9b1e64ac2880934e2ce5c9d10c42a1249d71cf49.nq.gz
│   ├── a025794b086c8b99cc5541a2698f6d4a86ad5cd5.nq.gz
│   ├── a1b94661a1e30e351cc2fbdbcb1584750751a423.nq.gz
│   ├── b2d3bd5e1be2d99e82c2c3cf2aa30c25320327b8.nq.gz
│   ├── d1383efc579c465550f50b3e4fb02943cb85efb1.nq.gz
│   ├── d3268d98bb01302eb3d9709b5143c8449a504977.nq.gz
│   ├── e623e022069beb9011860d09abcc36a73118b4ce.nq.gz
│   └── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── dac1e5ea2e8786bbef633c917c020f0b1966572b.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

12 directories, 32 files
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

[ansible-community/meetup-pretix-discourse-auth](https://github.com/ansible-community/meetup-pretix-discourse-auth)

---
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
