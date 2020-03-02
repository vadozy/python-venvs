-- Setting up virtual env
-- Activating and Installing dependencies inside virtual env

$ cd .
$ python -m venv venv_nndl
$ . ./venv_nndl/bin/activate
-- Upgrade pip (ensurepip may have older version), and setuptools, wheel too.
$ (venv_nndl) pip install --upgrade pip setuptools
$ (venv_nndl) pip install -r requirements.txt

-- To deactivate:
$ deactivate

