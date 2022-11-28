# JCron

_Just a concept, no implementation ATM_

Javascript cron replacement.

### Install

```sh
npm i -g jcron
```

Install systemd timer:
```
jcron install
```

### Usage

The runner will run every hour.

Create a config file in `~/.config/jcron/jobs.yml`:
```yaml
tasks:
  name_of_task:
    path: /web/apps/webapp1/current
    command: node scripts/load
```

The output of the command will be logged to `~/.config/jcron/jobs.log`

ISC Licensed. Enjoy!
