# Disposable receipt identity qualification

This repository qualifies real GitHub Actions identities for `pull_request_target`
and `workflow_run`. It contains no API runtime or deployment authority.

The evaluator, caller, verifier and policy were exported from
`Kendall04/terragrunt_demo@a07939b8d3b281b2a4f41c63350f29f3179ccca9`.
Only repository identity constants are adapted. `api-delivery.yml` is an inert
test harness with the production workflow name and path. The Dockerfile is an
unbuilt identity fixture. All receipts are `deployment=false`.

The promotion pull request stays open. No AWS, secrets, deployment environments,
image builds, ECR writes or infrastructure operations are part of this test.
The GitHub OIDC token is used only by the pinned attestation action.

Documentation event 1: unchanged synthetic application identity.
