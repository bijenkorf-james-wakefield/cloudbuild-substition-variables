# Cloudbuild substitution variables

This is a test repository for project [env-ci](https://github.com/pvdlg/env-ci) testing accessing [subsitution variables](https://cloud.google.com/cloud-build/docs/configuring-builds/substitute-variable-values).

# Prerequisites

- A [Google Cloud](https://cloud.google.com) account
- [Cloud SDK](https://cloud.google.com/docs/) installed for your chosen environment
- [Cloudbuild](https://cloud.google.com/cloud-build/) configured (possibly requires enabled billing)

# Usage

To access the substitution variables you need to pass them in the [build configuration file](build/cloudbuild.yaml).

To manually trigger a build using this configuration use the following command (where [YOUR_PROJECT_ID] is the id of the project you have setup in Gcloud)

```sh
gcloud builds submit --config=./build/cloudbuild.yaml ./build/ --project=[YOUR_PROJECT_ID]]
```
