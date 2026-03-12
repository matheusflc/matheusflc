# Profile metrics setup

This profile uses `lowlighter/metrics` to generate the SVG cards referenced by `README.md`.

## Required setup

1. Create a GitHub personal access token named for example `METRICS_TOKEN`.
2. Add it to the `matheusflc/matheusflc` repository secrets as `METRICS_TOKEN`.
3. In GitHub profile settings, enable **Include private contributions on my profile**.
4. Run the `Metrics` workflow manually once from the Actions tab, or push a new commit.

## Notes

- A scope-less token can show private contribution counts if the profile setting above is enabled.
- If you want metrics that inspect private repositories more deeply, use a token with `repo` scope.
- The placeholder SVG files in the repository are expected to be overwritten by the workflow.
