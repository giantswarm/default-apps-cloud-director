<!--
Not all PRs will require all tests to be carried out. Delete where appropriate.
-->

<!--
MODIFY THIS AFTER your new app repo is in https://github.com/giantswarm/github
@team-halo-engineers will be automatically requested for review once
this PR has been submitted. (But not for drafts)
-->

This PR:

- adds/changes/removes etc

### Testing

Description on how default-apps-cloud-director can be tested.

- [ ] fresh install works
- [ ] upgrade from previous version works

<!--
Changelog must always be updated.
-->

### Checklist

- [ ] Update changelog in CHANGELOG.md, **check all commits are in it before release (renovate included)**.
- [ ] Make sure `values.yaml` and `values.schema.json` are valid.



### Trigger e2e tests

<!--
We currently have one pipeline that tests both cluster creation and cluster upgrades. You can trigger this pipeline by writing this commands in a pull request comment or description
- `/run cluster-test-suites`
If for some reason you want to skip the e2e tests, remove the following line.

Note: Tests are not automatically executed when creating a draft PR
If you do want to trigger the tests while still in draft then please add a comment with the trigger.
-->

/run cluster-test-suites
