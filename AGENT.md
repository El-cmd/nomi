# AGENT.md

## Project Snapshot
- Repository: `El-cmd/nomi`
- Default branch: `main`
- Detected stack: Go, Docker, shell scripts
- Notable root entries: `.github/`, `.vscode/`, `cmd/`, `docker/`, `hack/`, `internal/`, `prompts/`, `usecases/`, `.gitignore`, `.golangci.yml`, `CODE_OF_CONDUCT.md`, `CODEOWNERS`, `CONTRIBUTING.md`, `go.mod`, `go.sum`, `install.bat`
- Source mix: .go:123, .yml:19, .sql:6, .md:4, .sh:2, .386:2

## Working Guidelines
- Keep changes scoped to the requested behavior and follow the style already present in the touched files.
- Check `README.md`, `Makefile`, package scripts, and Docker files before introducing new commands or tooling.
- Keep changes small and aligned with the current repository structure.
- Do not commit local secrets, `.env` files, generated dependency folders, build artifacts, or editor metadata.

## Setup
- `go mod download`

## Run
- `go run ./cmd/... (choose the relevant command package)`
- `make dev`

## Validate
- `make`
- `go test ./...`
- `go vet ./...`
- `make test`

## Makefile Targets Detected
- `all`, `fmt`, `test`, `build-dev`, `dev`
