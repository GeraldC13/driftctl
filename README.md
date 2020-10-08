

# About driftctl
`driftctl` measures infrastructure as code coverage, and tracks infrastructure drift.

## Why ?

Infrastructure as code is awesome, but there are too many moving parts: codebase, state file, actual cloud state. Things tend to drift.

Drift can have multiple causes: from developers creating or updating infrastructure through the web console without telling anyone, to uncontrolled updates on the cloud provider side. Handling infrastructure drift vs the codebase can be challenging.

You can't efficiently improve what you don't track. **We track coverage for unit tests, why not infrastructure as code coverage?**

`driftctl` tracks how well your IaC codebase covers your cloud configuration. `driftctl` warns you about drift.


## What does it do?
- **Scan** cloud provider and map ressources with IaC code
- **Output coverage** in standard format
- **Integrate into CI** flow to expose coverage to everyone
- Allow users to **ignore** resources
- **Analyze diff** between consecutive runs, and warn about drift and unwanted unmanaged ressources

