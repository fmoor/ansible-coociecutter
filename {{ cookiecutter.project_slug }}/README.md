# {{ cookiecutter.project_slug }}

## Setup
Create and activate a virtualenv. Then:

```bash
$ pipenv install
$ ansible-galaxy install -r requirements.yml
```

Decrypt `.vault_password.gpg` to `./.vault_password`.

```bash
$ cat .vault_password.gpg | gpg > .vault_password
```

## Usage
All `ansible*` commands need to be run from the top level directory in this repo.
Otherwise ansible won't find the `ansible.cfg` file and nothing will work.
