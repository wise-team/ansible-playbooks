# Ansible Playbooks

<!--§ data.config.repository.readme.generateDefaultBadges(data) §-->
[![License](https://img.shields.io/github/license/wise-team/ansible-playbooks.svg?style=flat-square)](https://github.com/wise-team/ansible-playbooks/blob/master/LICENSE) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) [![Chat](https://img.shields.io/badge/chat%20on%20discord-6b11ff.svg?style=flat-square)](https://discordapp.com/invite/CwxQDbG) [![Wise operations count](https://img.shields.io/badge/dynamic/json.svg?label=wise%20operations%20count&url=https%3A%2F%2Fsql.wise.vote%2Foperations%3Fselect%3Dcount&query=%24%5B0%5D.count&colorB=blue&style=flat-square)](https://sql.wise.vote/operations?select=moment,delegator,voter,operation_type&order=moment.desc)
<!--§§.-->

### wise.vote

Here is basic deployment guide:
```bash
## Production
# Initialize staging server (once for each server)
$ ansible-playbook -i wise.vote/inventory/production.yml wise.vote/init-server.yml

# Deploy whole wise
$ ansible-playbook -i wise.vote/inventory/production.yml wise.vote/wise.vote.yml

# Deploy some parts
$ ansible-playbook -i wise.vote/inventory/production.yml wise.vote/wise.vote.yml --tags "sql,sql-backup,manual"


## Staging: 
# Initialize staging server (once for each server)
$ ansible-playbook -i wise.vote/inventory/staging.yml wise.vote/init-server.yml

# Deploy whole wise
$ ansible-playbook -i wise.vote/inventory/staging.yml wise.vote/wise.vote.yml

# Deploy some parts
$ ansible-playbook -i wise.vote/inventory/staging.yml wise.vote/wise.vote.yml --tags "sql,sql-sql-backup,manual"
```



<!--§ data.config.repository.readme.generateHelpMd(data) §-->
## Where to get help?

- Feel free to talk with us on our chat: [https://discordapp.com/invite/CwxQDbG](https://discordapp.com/invite/CwxQDbG) .
- You can read [The Wise Manual](https://docs.wise.vote/introduction)
- You can also contact us at contact@wiseteam.io (if you think that you found a security issue, please contact us quickly).

You can also ask questions as issues in appropriate repository: See [issues for this repository](https://github.com/wise-team/ansible-playbooks/issues).

<!--§§.-->

<!--§ data.config.repository.readme.generateHelpUsMd(data) §-->
## Contribute to steem Wise

We welcome warmly:

- Bug reports via [issues](https://github.com/wise-team/ansible-playbooks).
- Enhancement requests via via [issues](https://github.com/wise-team/ansible-playbooks/issues).
- [Pull requests](https://github.com/wise-team/ansible-playbooks/pulls)
- Security reports to _contact@wiseteam.io_.

**Before** contributing please **read [Wise CONTRIBUTING guide](https://github.com/wise-team/steem-wise-core/blob/master/CONTRIBUTING.md)**.

Thank you for developing WISE together!



## Like the project? Let @wise-team become your favourite witness!

If you use & appreciate our software — you can easily support us. Just vote for "wise-team" to become you one of your witnesses. You can do it here: [https://steemit.com/~witnesses](https://steemit.com/~witnesses).

<!--§§.-->

<!-- Prayer: Gloria Patri, et Filio, et Spiritui Sancto, sicut erat in principio et nunc et semper et in saecula saeculorum. Amen. In te, Domine, speravi: non confundar in aeternum. -->
