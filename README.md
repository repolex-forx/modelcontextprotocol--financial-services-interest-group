# Repolex Knowledge Graph of modelcontextprotocol/financial-services-interest-group

RDF knowledge graph data for [modelcontextprotocol/financial-services-interest-group](https://github.com/modelcontextprotocol/financial-services-interest-group), parsed by [repolex](https://repolex.ai).

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
rlex download modelcontextprotocol/financial-services-interest-group
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── f238370c186e1dae0227dbf996480ac634e62b33
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── f238370c186e1dae0227dbf996480ac634e62b33
│           └── chunk-001.nq.gz
├── blob
│   ├── 2882984e272d7286b73c0f2bed4ffa95df4bef9b.nq.gz
│   ├── 2a6be4c5b4dbfb919729bc4db8ebf9d32dada2a0.nq.gz
│   ├── 4cc4ba7bd9a961069929b9bd9d5622e54a964655.nq.gz
│   ├── 814c52fbbbfa015ea86fd7d88ed46a697d8acc05.nq.gz
│   ├── c6f68fa7de13baceb1ed57c3ba61cac29da4646b.nq.gz
│   ├── d9e9729740feeba60fcc15064250d3a64585989b.nq.gz
│   ├── f5a457e4241502ddf35e2dfbd5ebce945d4c3369.nq.gz
│   └── ffb2d9b02874d5ccbfe03780d9e0709a5281070b.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── f238370c186e1dae0227dbf996480ac634e62b33.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 16 files
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

[modelcontextprotocol/financial-services-interest-group](https://github.com/modelcontextprotocol/financial-services-interest-group)

---
*Parsed on 2026-10-09 by [repolex](https://repolex.ai)*
