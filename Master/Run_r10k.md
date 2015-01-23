<!SLIDE>
# Ready to Deploy

R10k fetches the control repo and creates environments for each branch.

    $ r10k deploy environment -pv
    [R10K::Task::Deployment::DeployEnvironments - INFO] Loading environments from all sources
    [R10K::Task::Environment::Deploy - NOTICE] Deploying environment test
    [R10K::Task::Puppetfile::Sync - INFO] Loading modules from Puppetfile into queue
    [R10K::Task::Module::Sync - INFO] Deploying thttpd into /etc/puppet/environments/test/modules
    [R10K::Task::Module::Sync - INFO] Deploying ngircd into /etc/puppet/environments/test/modules
    [R10K::Task::Module::Sync - INFO] Deploying denyhosts into /etc/puppet/environments/test/modules
    [R10K::Task::Module::Sync - INFO] Deploying vcsrepo into /etc/puppet/environments/test/modules
    [R10K::Task::Module::Sync - INFO] Deploying stdlib into /etc/puppet/environments/test/modules
    [R10K::Task::Module::Sync - INFO] Deploying inifile into /etc/puppet/environments/test/modules
    [R10K::Task::Module::Sync - INFO] Deploying firewall into /etc/puppet/environments/test/modules
    [R10K::Task::Module::Sync - INFO] Deploying concat into /etc/puppet/environments/test/modules
    [R10K::Task::Module::Sync - INFO] Deploying make into /etc/puppet/environments/test/modules
    [R10K::Task::Environment::Deploy - NOTICE] Deploying environment production
    [R10K::Task::Puppetfile::Sync - INFO] Loading modules from Puppetfile into queue
    [R10K::Task::Module::Sync - INFO] Deploying thttpd into /etc/puppet/environments/production/modules
    [R10K::Task::Module::Sync - INFO] Deploying ngircd into /etc/puppet/environments/production/modules
    [R10K::Task::Module::Sync - INFO] Deploying denyhosts into /etc/puppet/environments/production/modules
    [R10K::Task::Module::Sync - INFO] Deploying vcsrepo into /etc/puppet/environments/production/modules
    [R10K::Task::Module::Sync - INFO] Deploying stdlib into /etc/puppet/environments/production/modules
    [R10K::Task::Module::Sync - INFO] Deploying inifile into /etc/puppet/environments/production/modules
    [R10K::Task::Module::Sync - INFO] Deploying firewall into /etc/puppet/environments/production/modules
    [R10K::Task::Module::Sync - INFO] Deploying concat into /etc/puppet/environments/production/modules
    [R10K::Task::Module::Sync - INFO] Deploying make into /etc/puppet/environments/production/modules
    [R10K::Task::Deployment::PurgeEnvironments - INFO] Purging stale environments from /etc/puppet/environments
        .    .    .

