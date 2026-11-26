# Working on Canon

Start with `docs/agent-workflows.md` for the V2 draft and its record index.
Read definitions as needed during ordinary work. Only the user can invoke the
definition workflow; editing code is not an invitation to change project rules.

The Go CLI and bundled skills predate the V2 design. Use `go run ./cmd/canon
commands` to discover implemented commands; global flags precede the command.
Check the repository with `go run ./cmd/canon doctor` and `go run ./cmd/canon
validate`. Those checks cover the CLI's supported record kinds, not every V2
draft.

For implementation work, run `go test ./...`, keep Go code formatted, and
prefer the standard library. Keep CLI output deterministic, verify JSON
contracts in `internal/canon` tests, and preview multi-record mutations with
`--dry-run`. Edit bundled skill sources in `skill/assets`, not their installed
copies; bump the affected asset version in `skill/skill.go` when changing one.
