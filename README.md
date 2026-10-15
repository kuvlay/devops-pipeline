# GitHub Actions · CI Workflow Lab

A small JavaScript repository for learning how a push triggers a CI job, checks out source code, prepares Node.js, and runs an npm command.

**JavaScript · Node.js · npm · GitHub Actions**

[Portfolio](https://github.com/kuvlay)

## Repository contents

| File | Role |
| --- | --- |
| `index.js` | Prints introductory DevOps messages |
| `test.js` | Demonstrates console output and a delayed callback |
| `.github/workflows/pipeline.yaml` | Defines the CI job for pushes to `main` |
| `package.json` | Provides the local run and test commands |

## Run locally

```bash
git clone https://github.com/kuvlay/devops-pipeline.git
cd devops-pipeline
npm run run
npm test
```

Only Node.js and npm are needed. The project has no runtime dependencies or environment variables.

## Workflow

The current CI definition runs on an Ubuntu runner, checks out the repository, configures Node.js 16, installs dependencies, and invokes `npm test`.

The workflow is a learning example. Its pinned runtime/action versions should be reviewed before extending it into an active delivery pipeline. The file named `test.js` prints messages; it contains no assertions and does not establish application correctness. No deployment stage is implemented, and no CI-pass claim is made here.

<details>
<summary>Credits and project history</summary>

Source lineage: [aarish-io/devops-pipeline](https://github.com/aarish-io/devops-pipeline). Original history is retained. The package manifest declares ISC; no standalone license text was present in the reviewed source.

</details>
