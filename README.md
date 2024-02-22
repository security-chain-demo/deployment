This repository handles deployments.
There are no real deployments, as this is just a demo.

See the vision below:

-------------------------------------------------------------------------------

Updating the [`services.json`](services.json) will trigger CI/CD to do the
deployments (usually you might wanna stop old containers, start new containers,
let K8s do its thing, execute a couple of your very unique scripts to
do the magic, whatever… 😉). Again, this is a demo, no real deployments.

Updating the [`services.json`](services.json) in a PR will, now here is the
interesting part, compare your services to the ones before, analyse the
differences and inform about new/changed security vulnerabilities.

Adding new vulnerabilities may only be done with explicit approval of
a certain supervisor.

Vulnerabilities are synchronized to a JIRA issue tracker where each feature
team has its own issues, so they can work independently on these.

The [`services.json`](services.json) also assigns each service to a specific
team (one team could maintain multiple services). This team will be referenced
when syncing to JIRA. 
