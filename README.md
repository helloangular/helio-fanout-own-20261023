# helio-fanout-own-20261023

Synthetic test fixture for Helio (BlueMatrix acceptance, 23 Oct 2026). Nothing is deployed anywhere.

`.github/workflows/fanout-own-deploy.yml` fans one release out to two production environment instances,
`fown-prod-east` and `fown-prod-west`, and records one GitHub deployment per instance. Helio dispatches it on
immutable `helio/workflow/<sha>` tags. Files under `.helio/` and `helio-pipeline-*` workflows are written by
Helio's environment manifest publication.
