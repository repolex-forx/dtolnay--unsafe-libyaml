# Repolex Knowledge Graph of dtolnay/unsafe-libyaml

RDF knowledge graph data for [dtolnay/unsafe-libyaml](https://github.com/dtolnay/unsafe-libyaml), parsed by [repolex](https://repolex.ai).

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
rlex download dtolnay/unsafe-libyaml
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── a7b8d1fbd93aefbca3003dcb5fcc6a9c2297e968
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── a7b8d1fbd93aefbca3003dcb5fcc6a9c2297e968.nq.gz
│   └── repolex
│       └── a7b8d1fbd93aefbca3003dcb5fcc6a9c2297e968
│           └── chunk-001.nq.gz
├── blob
│   ├── 0500980a8527f22ddf7ec79c4214c53d8ce0d28a.nq.gz
│   ├── 07f48f051c581e3fc13c50701b1706700795b431.nq.gz
│   ├── 0f78fa0c2eaa57cf73b1924e94b23dda847a0c56.nq.gz
│   ├── 12e1de536d8d8ecc8cfa9409d41a797c2c8483a9.nq.gz
│   ├── 190db266e0bff774beb6c10e630e2dc87d8e3116.nq.gz
│   ├── 27d3907e8238292041d78690410e3a57243de8d7.nq.gz
│   ├── 31aa79387f27e730e33d871925e152e35e428031.nq.gz
│   ├── 325a348226d33be664aa6c0ad70925f47cdbebab.nq.gz
│   ├── 439ee0334b42f868b001b9bff96d87beddba87a5.nq.gz
│   ├── 44f2e85648c6894832e4b98bc97bb6152a524caf.nq.gz
│   ├── 4597d3d91bab6fc91e69643c61dd1cc300ec7a3a.nq.gz
│   ├── 578db27df78c141ef33eaf8b634d4b0de1c7b0e0.nq.gz
│   ├── 5adc54aed3bdd111ebd0237ab4361589365da277.nq.gz
│   ├── 6d562c0e535df0fae9bd326fa5a3a918b68bb3d0.nq.gz
│   ├── 6e4c30049d6685012b5ecc39bdb59650bfdd24c3.nq.gz
│   ├── 7054c460a3954dbceac6b7f2f919620a4d133861.nq.gz
│   ├── 730c927cdaf5004b2eff6ad077df3d2d628fbe11.nq.gz
│   ├── 750707701cdae985156601cc906195021ba6a6e5.nq.gz
│   ├── 7b009f6bc731f829f1e3dbbb1958a5dfa7edf60a.nq.gz
│   ├── 7b549ca7adc02d0d5585225c49af9d354a461bd2.nq.gz
│   ├── 852be2cc1a0a985868cfc16349e0d32e428549d5.nq.gz
│   ├── 94029f60fb120dc1e0af41e62ff47b4a98c79f49.nq.gz
│   ├── 9473de84f4bfaa1464d4b3f4314cc7b95e4fbe32.nq.gz
│   ├── 9668929872b1e8becf9f46abd4e3da53ad1ed300.nq.gz
│   ├── 9c012c94ab54f1678235d3cd8e57aa7e65fd0f89.nq.gz
│   ├── a223b32d3145514f9743ecd6bd2f3fd93f4c3be4.nq.gz
│   ├── aa83f1adc26b96c58f7c03d84ac56eb2b9ef0511.nq.gz
│   ├── b3a0655358268825b60fe9f1149696d336658ab6.nq.gz
│   ├── b52000f346d96f7e4e9ca91ae0f57b73ce61f28c.nq.gz
│   ├── bfe37a70e4496f550b6d10fb30069164019d3e46.nq.gz
│   ├── c004d1721a6d60f785cb1df4be587a7ca22fd276.nq.gz
│   ├── c3beee9b818b208854a38c629650eaf30fd2a317.nq.gz
│   ├── c8bbcba62dcf4d78be78392f6f9321cca35390f1.nq.gz
│   ├── d40e5d2108a1338a36645ec3a939d9f483ac2db6.nq.gz
│   ├── d7dc5eaecf3f89b666a3825f90218544b97a62a2.nq.gz
│   ├── f2318c5e1368b6371925cf3a00fb3e0c70eaf04b.nq.gz
│   ├── f83457aece715da65abae687983991a5c762b4d6.nq.gz
│   └── fde764802a0aef3eda9b46ca289dec75d9b4accf.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── a7b8d1fbd93aefbca3003dcb5fcc6a9c2297e968.nq.gz
├── filetree
│   └── a7b8d1fbd93aefbca3003dcb5fcc6a9c2297e968.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 48 files
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

[dtolnay/unsafe-libyaml](https://github.com/dtolnay/unsafe-libyaml)

---
*Parsed on 2026-11-22 by [repolex](https://repolex.ai)*
