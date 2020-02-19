## Merritt Repository Tagger

- https://github.com/cdluc3/mrt-repo-tagger

+++

## Merritt Code Lives in 29 Repositories

- https://github.com/CDLUC3/mrt-repo-tagger/blob/master/config.yml#L3-L93

+++

## Some Repos Deploy from Branches

- https://github.com/CDLUC3/mrt-repo-tagger/blob/master/config.yml#L86-L90

+++

## Tag Every Sprint in Every Repo

- https://github.com/CDLUC3/merritt-docker/releases

+++

## Diff by Sprint

- https://github.com/CDLUC3/merritt-docker/compare/sprint-29..sprint-31

+++

## Merritt Release Summaries

For the past 4 months

- https://github.com/CDLUC3/mrt-doc/releases

+++

## Merritt Deployment Summaries

- To be added for prospective deployments
- A markdown template exists
  - https://github.com/CDLUC3/mrt-repo-tagger/blob/master/config.yml#L97-L128

---

## Code Options

```
python3 tagger.py -h
usage: tagger.py [-h] [--no-clone] {sprint,deploy,report,delete} ...

positional arguments:
  {sprint,deploy,report,delete}

optional arguments:
  -h, --help            show this help message and exit
  --no-clone
```

+++

## Sprint Tagging

```
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

## Deployment Tagging

```
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
## Report Generation

```
python3 tagger.py report -h
usage: tagger.py report [-h] --since SINCE [--until UNTIL]

optional arguments:
  -h, --help     show this help message and exit
  --since SINCE
  --until UNTIL
```

+++

## Tag Cleanup

```
python3 tagger.py delete -h
usage: tagger.py delete [-h] tag [tag ...]

positional arguments:
  tag

optional arguments:
  -h, --help  show this help message and exit
```

---

## Questions

- What approaches do other teams follow?
- Do any teams clone their repos for backup purposes?
  - (in case of a GitHub outage)
