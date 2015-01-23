<!SLIDE>
# Feature Branch Environments #

    croddy@devbox $ git branch
      dev
      preprod
      production
      test
      croddy_JIRA_567
    * croddy_JIRA_1234
      jmorrison_JIRA_890

After `r10k deploy environment -p`...

    /etc/puppet/environments/
    ├── croddy_JIRA_1234
    ├── croddy_JIRA_567
    ├── dev
    ├── jmorrison_JIRA_890
    ├── preprod
    ├── production
    └── test

