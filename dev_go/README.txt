-- Setting up virtual env
-- Activating and Installing dependencies inside virtual env

$ cd .
$ python3 -m venv venv_go
$ . ./venv_go/bin/activate
-- Upgrade pip (ensurepip may have older version), and setuptools, wheel too.
$ (venv_go) pip install --upgrade pip setuptools
$ (venv_go) pip install -r requirements.txt

-- To deactivate:
$ deactivate

-- If need to move venv to another dir:
$ (venv_go) pip freeze > requirements.txt
$ (venv_go) deactivate
$ python3 -m venv newenv
$ . ./newenv/bin/activate
$ (newenv) pip install -r requirements.txt
(You may remove old venv now -> rm -rf venv_go)
