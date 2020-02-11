# repo-tagger

This code is a python wrapper that processes a list of related GitHub repos and tags them with a sprint number.

## Prerequisites
- Python3
  - pip3 install pyyaml
  - pip3 install python_dateurtil
- A list of repositories to publish (SSH path)
  - Create an ssh key for github: github_rsa/github_rsa.pub
  - Upload github_rsa.pub to your GitHub SSH keys
  - Modify ~/.ssh/config
```
Host github.com
	HostName github.com
	User git
	IdentityFile ~/.ssh/github_rsa
```
- You must have contributor rights in these repositories

## tagger [--no-clone] Action

If you run the command repeatedly, you can prevent the re-cloning of content with the `--no-clone` option.

## tagger sprint XX [---as-of-date YYYY-MM-DD] [--since TAG] [--title TITLE]

Tag all repos with a sprint number.

- --date Retroactively tag based on a date
- --since Generate a report of changes since TAG

## tagger deploy [--deploy-date YYYY-MM-DD] [--since TAG] [--title TITLE]

Tag mrt-doc repos with deployment release.

- --since Generate a report of changes since TAG

## tagger report --since TAG [--until TAG]

Generate a report of changes since TAG

- --until TAG stop report at TAG

## tagger delete TAG1 [... TAGN]

Delete a tag that was created by the tool.
