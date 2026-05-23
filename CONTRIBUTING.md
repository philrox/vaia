# Contributing to VAIA

Thanks for your interest. VAIA is in active development for the [Agora Agents Hackathon](https://agora.thecanteenapp.com/) (May 21–25 2026). The process below applies during and after the hackathon.

## Development Setup

Requires Python 3.11+ and [`uv`](https://docs.astral.sh/uv/).

```bash
git clone https://github.com/philrox/vaia
cd vaia
uv sync                  # install dependencies
uv run pytest            # run tests
uv run ruff check .      # lint
uv run mypy src/         # type-check
```

## TDD-First Workflow (mandatory)

Every change follows this sequence — no shortcuts:

1. Open or reference a spec in `docs/specs/SPEC-VXXX.md`
2. Write failing tests **first**, commit them as a separate commit (`Add failing tests for SPEC-VXXX`)
3. Implement until tests pass
4. Run `uv run ruff check . && uv run mypy src/` clean
5. Open a PR using the template, mark the Definition-of-Done checklist complete

If you skip the failing-tests step, the PR will not be merged.

## Branch & Commit Conventions

- Branch from `main`, name like `feature/spec-v003-trader` or `fix/dashboard-offset`
- Commit messages: imperative mood, no trailing period (`Add HIP-4 adapter`, not `Added HIP-4 adapter.`)
- Squash on merge — keep commit history linear

## PR Review Policy

- **External contributors**: open a PR from your fork. A maintainer (@philrox) will review before merging.
- **Maintainers**: self-merge allowed after CI passes; no approval required.

## Reporting Issues

Use the issue templates. Security issues: see [SECURITY.md](SECURITY.md) — do **not** open public issues for vulnerabilities.

## Code of Conduct

By participating, you agree to abide by the [Code of Conduct](CODE_OF_CONDUCT.md).
