# github_actions_test_1

A repo to test GitHub Actions in a certain way of linting, testing and deployment.

Please note that the project in the repo is highly opinionated, raison d'etre of this very repository is just to come up with a suitable actions workflow to lint, test, build and deploy upon push or pull-request over branches (currently main to production and dev to staging).

## References

* https://stackoverflow.com/a/58655352/250453

## Important Notes

* Do NOT delete branch via GitHub, delete branch locally (and the remote one) with your git client

* If we protect the any major branch (i.e. main and dev) with "Require a pull request before merging" and "Require status checks to pass before merging" (and also "Include administrators" as well) we won't be able to just push to that branch, instead a transient branch will get created and a pull-request is made.
