# Owner-operated Omarchy acceptance report

This repository was generated through GitHub's template-generation API from the public
[agterm-omarchy-agent-template](https://github.com/alexandru-savinov/agterm-omarchy-agent-template).
[template-origin.json](template-origin.json) records the template source commit, generated initial commit, matching initial tree, and verified template metadata.
It is an owner-operated demonstration of reusable reporting infrastructure, not third-party adoption.

[report.json](report.json) reviews already public ARM64 Omarchy acceptance evidence:

| Reported check | Basis |
|---|---|
| Actual-installed Live runtime | Existing nine-check result from the operator's isolated VM run |
| Corrected cleanup | Existing fresh endpoint and shell-PID audit for normal and intentional-failure runs |
| Native core tests | Attributed operator report of 4,025 tests in 175 suites |
| Installed binary identity | Existing published COMMIT/hash comparison, distinct from the harness revision |

**No new runtime test or independent account approval is claimed.**
The report pins application source `5e37cb75` and links the separately published canonical evidence.
It retains the UTM software-rendering and zsh-fixture conditions and the invalidated cleanup-history limitation.

## Validate the report

```sh
python3 scripts/test_validate_report.py
python3 scripts/validate_report.py report.json
```

The [validation workflow](https://github.com/alexandru-savinov/agterm-omarchy-agent-report/actions/workflows/validate-report.yml)
checks report structure, attribution consistency, public GitHub URL shape, and limited privacy patterns.
It publishes a JSON validation outcome and job summary.
A green validation run does not independently prove the linked runtime claims.
The script does not fetch evidence links or execute report contents.

For your own report, use the [template](https://github.com/alexandru-savinov/agterm-omarchy-agent-template),
read the [agent protocol](https://github.com/alexandru-savinov/agterm-omarchy/blob/main/docs/AGENT_PROTOCOL.md),
and coordinate on the [public hub](https://github.com/alexandru-savinov/agterm-omarchy/issues/1).
