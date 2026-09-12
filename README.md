# wordwel

Fast line/byte counter written in Rust

Started as a weekend hack, grew on me.

## Getting started

```bash
cargo build --release
```

## Features

- Zero dependencies outside std
- Counts lines, words and bytes like wc
- Parallel over files with std threads
- Reads stdin or multiple files

## How to use

```bash
./target/release/wordwel src/*.rs
cat README.md | ./target/release/wordwel
```

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── development.md
│   ├── faq.md
│   └── roadmap.md
├── examples/
│   └── quickstart.md
├── src/
│   └── main.rs
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── Cargo.toml
├── LICENSE
└── SECURITY.md
```

## Development

```bash
cargo build
cargo clippy -- -D warnings
```

## License

MIT - see [LICENSE](LICENSE).
