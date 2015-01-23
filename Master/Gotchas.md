<!SLIDE>
# Gotchas #
* `master` is an illegal environment name, so you must rename the branch
* R10k does not install dependencies, you must specify them
* `hiera.yaml` can't be consulted on a per-environment basis *(HI-46)*
* Agent-set environments require a special configuration in PE 3.7
* R10k has Subversion support, so your Git *coup d'état* might fail
