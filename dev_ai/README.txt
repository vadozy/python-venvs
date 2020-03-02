-- Setting up virtual env
-- Activating and Installing dependencies inside virtual env

$ cd .
$ python3 -m venv venv_ai
$ . ./venv_ai/bin/activate
-- Upgrade pip (ensurepip may have older version), and setuptools, wheel too.
$ (venv_ai) pip install --upgrade pip setuptools wheel
$ (venv_ai) pip install -r requirements.txt

-- To deactivate:
$ deactivate

-- Start jupyter notebook
$ jupyter notebook

-- If need to move venv to another dir:
$ (venv_ai) pip freeze > requirements.txt
$ (venv_ai) deactivate
$ python3 -m venv newenv
$ . ./newenv/bin/activate
$ (newenv) pip install -r requirements.txt
(You may remove old venv now -> rm -rf venv_ai)
