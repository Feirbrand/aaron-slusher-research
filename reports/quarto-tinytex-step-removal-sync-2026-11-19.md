# Quarto TinyTeX Step Removal Sync Receipt — November 19, 2026

## Scope

This synchronization removed the unnecessary TinyTeX installation step from exactly two HTML-only Quarto Pages workflows.

### `Feirbrand/synoeticos-public`

- `.github/workflows/quarto-publish.yml`

### `Feirbrand/aaron-slusher-research`

- `.github/workflows/quarto-publish.yml`

The removed step was exactly:

```yaml
      - name: Install TinyTeX
        run: quarto install tinytex
```

The following blank line was removed with the step. No other workflow step or repository file changed.

Explicit exclusions:

- No `docs/_quarto.yml` file changed.
- No `.qmd` or site-content file changed.
- No other workflow changed, including `zenodo-metadata.yml`.
- Quarto version, render command, working directory, triggers, Pages configuration, and deployment steps remain unchanged.

## Diagnostics

Both repositories were freshly fetched and clean before editing, with local `HEAD` matching `origin/main`.

Baselines:

- `synoeticos-public`: `a8f52cdae0e3811d0ae36f89e61b5b156d9b6d63`
- `aaron-slusher-research`: `540d87dce5cc992fa1dbd43a74f5c09d49998c24`

Both `docs/_quarto.yml` files were independently verified as HTML-only (`format: html`). Both workflows contained exactly one `Install TinyTeX` step and one `Render Quarto site` step, with Quarto version `1.8.0` and `working-directory: ./docs`.

## Commits

| Repository | Commit | Parent | Message |
|---|---|---|---|
| `synoeticos-public` | `42117b7656f99f1980dc6d38f254b62efc8605e8` | `a8f52cdae0e3811d0ae36f89e61b5b156d9b6d63` | `ci: remove unnecessary TinyTeX install` |
| `aaron-slusher-research` | `ebdb9e90f55c14bdd8a304774a6c0a76cadc3ea8` | `540d87dce5cc992fa1dbd43a74f5c09d49998c24` | `ci: remove unnecessary TinyTeX install` |

## File evidence

| Repository | Path | Commit SHA | Git blob SHA-1 | SHA-256 content hash | Bytes |
|---|---|---|---|---|---:|
| `synoeticos-public` | `.github/workflows/quarto-publish.yml` | `42117b7656f99f1980dc6d38f254b62efc8605e8` | `a3a2a3021c4220d8369ad3c9ec679b32ee4a4629` | `e09c14e88090949ffb04a071bba50b792340d3ec130ddaa4532d5ed470d4d941` | 962 |
| `aaron-slusher-research` | `.github/workflows/quarto-publish.yml` | `ebdb9e90f55c14bdd8a304774a6c0a76cadc3ea8` | `dcaa3e022ceacd5b6a5b67b244b779aadefb4fe7` | `e7745fc996b77a5fcd47f455a94560b22d002f768ffe656034a4d42dd475f95f` | 961 |

## Verification

- Both workflows no longer contain `Install TinyTeX` or `quarto install tinytex`.
- Both retain the Quarto setup step at version `1.8.0`.
- Both retain the render step and `working-directory: ./docs` byte-for-byte.
- Each workflow diff is exactly three deleted lines: the two TinyTeX step lines and the following blank line.
- `git diff --check` passed in both repositories.
- Exact two-file allowlist passed.
- Both Quarto configurations are HTML-only, so no PDF/LaTeX rendering dependency is required.
- Push, remote-parity, workflow-run, and live Pages verification are recorded after the receipt commit and push.
