#### Merritt Repository Tagger

- https://github.com/cdluc3/mrt-repo-tagger

+++

#### Merritt Code Lives in [29 Repositories](https://github.com/CDLUC3/mrt-repo-tagger/blob/master/config.yml#L3-L93)

+++

#### Some Repos [Deploy from Branches](https://github.com/CDLUC3/mrt-repo-tagger/blob/master/config.yml#L86-L90)

+++

#### Tag Every Sprint in Every Repo

- [Sprint Tags in a Code Repo](https://github.com/CDLUC3/merritt-docker/releases)

+++

#### Diff by Sprint

- [Diff sprint-29..sprint-31](https://github.com/CDLUC3/merritt-docker/compare/sprint-29..sprint-31)

+++

#### Merritt Release Summaries

[Release summaries the past 6 Sprints](https://github.com/CDLUC3/mrt-doc/releases)

+++

#### Merritt Deployment Summaries

- To be added for prospective deployments
- [Markdown template for each deployment](https://github.com/CDLUC3/mrt-repo-tagger/blob/master/config.yml#L97-L128)

---

#### Code Options

```bash
python3 tagger.py -h
usage: tagger.py [-h] [--no-clone] {sprint,deploy,report,delete} ...

positional arguments:
  {sprint,deploy,report,delete}

optional arguments:
  -h, --help            show this help message and exit
  --no-clone
```

+++

#### Sprint Tagging

```bash
python3 tagger.py sprint -h
usage: tagger.py sprint [-h] [--as-of-date AS_OF_DATE] [--since SINCE]
                        [--title TITLE]
                        num

positional arguments:
  num

optional arguments:
  -h, --help            show this help message and exit
  --as-of-date AS_OF_DATE
  --since SINCE
  --title TITLE
```

+++

#### Deployment Tagging

```bash
python3 tagger.py deploy -h
usage: tagger.py deploy [-h] [--deploy-date DEPLOY_DATE] [--since SINCE]
                        [--title TITLE]

optional arguments:
  -h, --help            show this help message and exit
  --deploy-date DEPLOY_DATE
  --since SINCE
  --title TITLE
```

+++
#### Report Generation

```bash
python3 tagger.py report -h
usage: tagger.py report [-h] --since SINCE [--until UNTIL]

optional arguments:
  -h, --help     show this help message and exit
  --since SINCE
  --until UNTIL
```

+++

#### Tag Cleanup

```bash
python3 tagger.py delete -h
usage: tagger.py delete [-h] tag [tag ...]

positional arguments:
  tag

optional arguments:
  -h, --help  show this help message and exit
```

---

#### Questions

- What approaches do other CDL teams follow?
- Do any CDL teams clone repos to the CDL network for backup purposes?
  - (in case of a GitHub outage)
