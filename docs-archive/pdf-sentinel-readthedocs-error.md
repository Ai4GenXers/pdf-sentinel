Read the Docs build information
Build id: 30303926
Project: pdf-sentinel
Version: latest
Commit: 1afbddf7b05d430e7fe95c288f98215c6c2f38c6
Date: 2025-11-13T05:51:18.084910Z
State: finished
Success: False


[rtd-command-info] start-time: 2025-11-13T05:51:18.705709Z, end-time: 2025-11-13T05:51:18.928294Z, duration: 0, exit-code: 0
git clone --depth 1 https://github.com/Ai4GenXers/pdf-sentinel.git .
Cloning into '.'...

[rtd-command-info] start-time: 2025-11-13T05:51:18.968344Z, end-time: 2025-11-13T05:51:19.332836Z, duration: 0, exit-code: 0
git fetch origin --force --prune --prune-tags --depth 50 refs/heads/main:refs/remotes/origin/main
From https://github.com/Ai4GenXers/pdf-sentinel
 * [new tag]         v2.0.0     -> v2.0.0

[rtd-command-info] start-time: 2025-11-13T05:51:19.408511Z, end-time: 2025-11-13T05:51:19.446386Z, duration: 0, exit-code: 0
git checkout --force origin/main
Note: switching to 'origin/main'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 1afbddf fix: Add build.os configuration to .readthedocs.yaml

[rtd-command-info] start-time: 2025-11-13T05:51:19.488084Z, end-time: 2025-11-13T05:51:19.524650Z, duration: 0, exit-code: 0
cat .readthedocs.yaml
# Read the Docs configuration file for PDF Sentinel
# See https://docs.readthedocs.io/en/stable/config-file/v2.html for details

version: 2

# Build environment
build:
  os: ubuntu-22.04
  tools:
    python: "3.12"

# Build documentation in the "docs/" directory with MkDocs
mkdocs:
  configuration: mkdocs.yml
  fail_on_warning: false

# Optionally build your docs in additional formats such as PDF and ePub
formats:
  - pdf
  - epub

# Python requirements required to build your documentation
python:
  install:
    - requirements: docs/requirements.txt

[rtd-command-info] start-time: 2025-11-13T05:51:23.734851Z, end-time: 2025-11-13T05:51:23.788103Z, duration: 0, exit-code: 0
asdf global python 3.12.10


[rtd-command-info] start-time: 2025-11-13T05:51:24.207861Z, end-time: 2025-11-13T05:51:24.937299Z, duration: 0, exit-code: 0
python -mvirtualenv $READTHEDOCS_VIRTUALENV_PATH
created virtual environment CPython3.12.10.final.0-64 in 458ms
  creator CPython3Posix(dest=/home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest, clear=False, no_vcs_ignore=False, global=False)
  seeder FromAppData(download=False, pip=bundle, setuptools=bundle, wheel=bundle, via=copy, app_data_dir=/home/docs/.local/share/virtualenv)
    added seed packages: pip==23.1, setuptools==67.6.1, wheel==0.40.0
  activators BashActivator,CShellActivator,FishActivator,NushellActivator,PowerShellActivator,PythonActivator

[rtd-command-info] start-time: 2025-11-13T05:51:24.976686Z, end-time: 2025-11-13T05:51:30.369545Z, duration: 5, exit-code: 0
python -m pip install --upgrade --no-cache-dir pip setuptools
Requirement already satisfied: pip in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (23.1)
Collecting pip
  Downloading pip-25.3-py3-none-any.whl (1.8 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.8/1.8 MB 14.7 MB/s eta 0:00:00
Requirement already satisfied: setuptools in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (67.6.1)
Collecting setuptools
  Downloading setuptools-80.9.0-py3-none-any.whl (1.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.2/1.2 MB 24.7 MB/s eta 0:00:00
Installing collected packages: setuptools, pip
  Attempting uninstall: setuptools
    Found existing installation: setuptools 67.6.1
    Uninstalling setuptools-67.6.1:
      Successfully uninstalled setuptools-67.6.1
  Attempting uninstall: pip
    Found existing installation: pip 23.1
    Uninstalling pip-23.1:
      Successfully uninstalled pip-23.1
Successfully installed pip-25.3 setuptools-80.9.0

[rtd-command-info] start-time: 2025-11-13T05:51:30.415799Z, end-time: 2025-11-13T05:51:32.399569Z, duration: 1, exit-code: 0
python -m pip install --upgrade --no-cache-dir mkdocs
Collecting mkdocs
  Downloading mkdocs-1.6.1-py3-none-any.whl.metadata (6.0 kB)
Collecting click>=7.0 (from mkdocs)
  Downloading click-8.3.0-py3-none-any.whl.metadata (2.6 kB)
Collecting ghp-import>=1.0 (from mkdocs)
  Downloading ghp_import-2.1.0-py3-none-any.whl.metadata (7.2 kB)
Collecting jinja2>=2.11.1 (from mkdocs)
  Downloading jinja2-3.1.6-py3-none-any.whl.metadata (2.9 kB)
Collecting markdown>=3.3.6 (from mkdocs)
  Downloading markdown-3.10-py3-none-any.whl.metadata (5.1 kB)
Collecting markupsafe>=2.0.1 (from mkdocs)
  Downloading markupsafe-3.0.3-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl.metadata (2.7 kB)
Collecting mergedeep>=1.3.4 (from mkdocs)
  Downloading mergedeep-1.3.4-py3-none-any.whl.metadata (4.3 kB)
Collecting mkdocs-get-deps>=0.2.0 (from mkdocs)
  Downloading mkdocs_get_deps-0.2.0-py3-none-any.whl.metadata (4.0 kB)
Collecting packaging>=20.5 (from mkdocs)
  Downloading packaging-25.0-py3-none-any.whl.metadata (3.3 kB)
Collecting pathspec>=0.11.1 (from mkdocs)
  Downloading pathspec-0.12.1-py3-none-any.whl.metadata (21 kB)
Collecting pyyaml-env-tag>=0.1 (from mkdocs)
  Downloading pyyaml_env_tag-1.1-py3-none-any.whl.metadata (5.5 kB)
Collecting pyyaml>=5.1 (from mkdocs)
  Downloading pyyaml-6.0.3-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl.metadata (2.4 kB)
Collecting watchdog>=2.0 (from mkdocs)
  Downloading watchdog-6.0.0-py3-none-manylinux2014_x86_64.whl.metadata (44 kB)
Collecting python-dateutil>=2.8.1 (from ghp-import>=1.0->mkdocs)
  Downloading python_dateutil-2.9.0.post0-py2.py3-none-any.whl.metadata (8.4 kB)
Collecting platformdirs>=2.2.0 (from mkdocs-get-deps>=0.2.0->mkdocs)
  Downloading platformdirs-4.5.0-py3-none-any.whl.metadata (12 kB)
Collecting six>=1.5 (from python-dateutil>=2.8.1->ghp-import>=1.0->mkdocs)
  Downloading six-1.17.0-py2.py3-none-any.whl.metadata (1.7 kB)
Downloading mkdocs-1.6.1-py3-none-any.whl (3.9 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.9/3.9 MB 61.5 MB/s  0:00:00
Downloading click-8.3.0-py3-none-any.whl (107 kB)
Downloading ghp_import-2.1.0-py3-none-any.whl (11 kB)
Downloading jinja2-3.1.6-py3-none-any.whl (134 kB)
Downloading markdown-3.10-py3-none-any.whl (107 kB)
Downloading markupsafe-3.0.3-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl (22 kB)
Downloading mergedeep-1.3.4-py3-none-any.whl (6.4 kB)
Downloading mkdocs_get_deps-0.2.0-py3-none-any.whl (9.5 kB)
Downloading packaging-25.0-py3-none-any.whl (66 kB)
Downloading pathspec-0.12.1-py3-none-any.whl (31 kB)
Downloading platformdirs-4.5.0-py3-none-any.whl (18 kB)
Downloading python_dateutil-2.9.0.post0-py2.py3-none-any.whl (229 kB)
Downloading pyyaml-6.0.3-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl (807 kB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 807.9/807.9 kB 430.7 MB/s  0:00:00
Downloading pyyaml_env_tag-1.1-py3-none-any.whl (4.7 kB)
Downloading six-1.17.0-py2.py3-none-any.whl (11 kB)
Downloading watchdog-6.0.0-py3-none-manylinux2014_x86_64.whl (79 kB)
Installing collected packages: watchdog, six, pyyaml, platformdirs, pathspec, packaging, mergedeep, markupsafe, markdown, click, pyyaml-env-tag, python-dateutil, mkdocs-get-deps, jinja2, ghp-import, mkdocs

Successfully installed click-8.3.0 ghp-import-2.1.0 jinja2-3.1.6 markdown-3.10 markupsafe-3.0.3 mergedeep-1.3.4 mkdocs-1.6.1 mkdocs-get-deps-0.2.0 packaging-25.0 pathspec-0.12.1 platformdirs-4.5.0 python-dateutil-2.9.0.post0 pyyaml-6.0.3 pyyaml-env-tag-1.1 six-1.17.0 watchdog-6.0.0

[rtd-command-info] start-time: 2025-11-13T05:51:32.438895Z, end-time: 2025-11-13T05:51:37.952984Z, duration: 5, exit-code: 0
python -m pip install --exists-action=w --no-cache-dir -r docs/requirements.txt
Requirement already satisfied: mkdocs>=1.5.0 in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (from -r docs/requirements.txt (line 4)) (1.6.1)
Collecting mkdocs-material>=9.5.0 (from -r docs/requirements.txt (line 5))
  Downloading mkdocs_material-9.7.0-py3-none-any.whl.metadata (19 kB)
Collecting mkdocs-git-revision-date-localized-plugin>=1.2.0 (from -r docs/requirements.txt (line 8))
  Downloading mkdocs_git_revision_date_localized_plugin-1.5.0-py3-none-any.whl.metadata (5.8 kB)
Collecting pymdown-extensions>=10.0 (from -r docs/requirements.txt (line 11))
  Downloading pymdown_extensions-10.17.1-py3-none-any.whl.metadata (3.1 kB)
Requirement already satisfied: click>=7.0 in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (from mkdocs>=1.5.0->-r docs/requirements.txt (line 4)) (8.3.0)
Requirement already satisfied: ghp-import>=1.0 in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (from mkdocs>=1.5.0->-r docs/requirements.txt (line 4)) (2.1.0)
Requirement already satisfied: jinja2>=2.11.1 in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (from mkdocs>=1.5.0->-r docs/requirements.txt (line 4)) (3.1.6)
Requirement already satisfied: markdown>=3.3.6 in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (from mkdocs>=1.5.0->-r docs/requirements.txt (line 4)) (3.10)
Requirement already satisfied: markupsafe>=2.0.1 in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (from mkdocs>=1.5.0->-r docs/requirements.txt (line 4)) (3.0.3)
Requirement already satisfied: mergedeep>=1.3.4 in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (from mkdocs>=1.5.0->-r docs/requirements.txt (line 4)) (1.3.4)
Requirement already satisfied: mkdocs-get-deps>=0.2.0 in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (from mkdocs>=1.5.0->-r docs/requirements.txt (line 4)) (0.2.0)
Requirement already satisfied: packaging>=20.5 in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (from mkdocs>=1.5.0->-r docs/requirements.txt (line 4)) (25.0)
Requirement already satisfied: pathspec>=0.11.1 in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (from mkdocs>=1.5.0->-r docs/requirements.txt (line 4)) (0.12.1)
Requirement already satisfied: pyyaml-env-tag>=0.1 in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (from mkdocs>=1.5.0->-r docs/requirements.txt (line 4)) (1.1)
Requirement already satisfied: pyyaml>=5.1 in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (from mkdocs>=1.5.0->-r docs/requirements.txt (line 4)) (6.0.3)
Requirement already satisfied: watchdog>=2.0 in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (from mkdocs>=1.5.0->-r docs/requirements.txt (line 4)) (6.0.0)
Collecting babel>=2.10 (from mkdocs-material>=9.5.0->-r docs/requirements.txt (line 5))
  Downloading babel-2.17.0-py3-none-any.whl.metadata (2.0 kB)
Collecting backrefs>=5.7.post1 (from mkdocs-material>=9.5.0->-r docs/requirements.txt (line 5))
  Downloading backrefs-6.0.1-py312-none-any.whl.metadata (3.2 kB)
Collecting colorama>=0.4 (from mkdocs-material>=9.5.0->-r docs/requirements.txt (line 5))
  Downloading colorama-0.4.6-py2.py3-none-any.whl.metadata (17 kB)
Collecting mkdocs-material-extensions>=1.3 (from mkdocs-material>=9.5.0->-r docs/requirements.txt (line 5))
  Downloading mkdocs_material_extensions-1.3.1-py3-none-any.whl.metadata (6.9 kB)
Collecting paginate>=0.5 (from mkdocs-material>=9.5.0->-r docs/requirements.txt (line 5))
  Downloading paginate-0.5.7-py2.py3-none-any.whl.metadata (11 kB)
Collecting pygments>=2.16 (from mkdocs-material>=9.5.0->-r docs/requirements.txt (line 5))
  Downloading pygments-2.19.2-py3-none-any.whl.metadata (2.5 kB)
Collecting requests>=2.26 (from mkdocs-material>=9.5.0->-r docs/requirements.txt (line 5))
  Downloading requests-2.32.5-py3-none-any.whl.metadata (4.9 kB)
Collecting gitpython>=3.1.44 (from mkdocs-git-revision-date-localized-plugin>=1.2.0->-r docs/requirements.txt (line 8))
  Downloading gitpython-3.1.45-py3-none-any.whl.metadata (13 kB)
Requirement already satisfied: python-dateutil>=2.8.1 in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (from ghp-import>=1.0->mkdocs>=1.5.0->-r docs/requirements.txt (line 4)) (2.9.0.post0)
Collecting gitdb<5,>=4.0.1 (from gitpython>=3.1.44->mkdocs-git-revision-date-localized-plugin>=1.2.0->-r docs/requirements.txt (line 8))
  Downloading gitdb-4.0.12-py3-none-any.whl.metadata (1.2 kB)
Collecting smmap<6,>=3.0.1 (from gitdb<5,>=4.0.1->gitpython>=3.1.44->mkdocs-git-revision-date-localized-plugin>=1.2.0->-r docs/requirements.txt (line 8))
  Downloading smmap-5.0.2-py3-none-any.whl.metadata (4.3 kB)
Requirement already satisfied: platformdirs>=2.2.0 in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (from mkdocs-get-deps>=0.2.0->mkdocs>=1.5.0->-r docs/requirements.txt (line 4)) (4.5.0)
Requirement already satisfied: six>=1.5 in /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages (from python-dateutil>=2.8.1->ghp-import>=1.0->mkdocs>=1.5.0->-r docs/requirements.txt (line 4)) (1.17.0)
Collecting charset_normalizer<4,>=2 (from requests>=2.26->mkdocs-material>=9.5.0->-r docs/requirements.txt (line 5))
  Downloading charset_normalizer-3.4.4-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl.metadata (37 kB)
Collecting idna<4,>=2.5 (from requests>=2.26->mkdocs-material>=9.5.0->-r docs/requirements.txt (line 5))
  Downloading idna-3.11-py3-none-any.whl.metadata (8.4 kB)
Collecting urllib3<3,>=1.21.1 (from requests>=2.26->mkdocs-material>=9.5.0->-r docs/requirements.txt (line 5))
  Downloading urllib3-2.5.0-py3-none-any.whl.metadata (6.5 kB)
Collecting certifi>=2017.4.17 (from requests>=2.26->mkdocs-material>=9.5.0->-r docs/requirements.txt (line 5))
  Downloading certifi-2025.11.12-py3-none-any.whl.metadata (2.5 kB)
Downloading mkdocs_material-9.7.0-py3-none-any.whl (9.3 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 9.3/9.3 MB 168.8 MB/s  0:00:00
Downloading mkdocs_git_revision_date_localized_plugin-1.5.0-py3-none-any.whl (26 kB)
Downloading pymdown_extensions-10.17.1-py3-none-any.whl (266 kB)
Downloading babel-2.17.0-py3-none-any.whl (10.2 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 10.2/10.2 MB 129.5 MB/s  0:00:00
Downloading backrefs-6.0.1-py312-none-any.whl (398 kB)
Downloading colorama-0.4.6-py2.py3-none-any.whl (25 kB)
Downloading gitpython-3.1.45-py3-none-any.whl (208 kB)
Downloading gitdb-4.0.12-py3-none-any.whl (62 kB)
Downloading smmap-5.0.2-py3-none-any.whl (24 kB)
Downloading mkdocs_material_extensions-1.3.1-py3-none-any.whl (8.7 kB)
Downloading paginate-0.5.7-py2.py3-none-any.whl (13 kB)
Downloading pygments-2.19.2-py3-none-any.whl (1.2 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.2/1.2 MB 118.3 MB/s  0:00:00
Downloading requests-2.32.5-py3-none-any.whl (64 kB)
Downloading charset_normalizer-3.4.4-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl (153 kB)
Downloading idna-3.11-py3-none-any.whl (71 kB)
Downloading urllib3-2.5.0-py3-none-any.whl (129 kB)
Downloading certifi-2025.11.12-py3-none-any.whl (159 kB)
Installing collected packages: paginate, urllib3, smmap, pymdown-extensions, pygments, mkdocs-material-extensions, idna, colorama, charset_normalizer, certifi, backrefs, babel, requests, gitdb, gitpython, mkdocs-material, mkdocs-git-revision-date-localized-plugin

Successfully installed babel-2.17.0 backrefs-6.0.1 certifi-2025.11.12 charset_normalizer-3.4.4 colorama-0.4.6 gitdb-4.0.12 gitpython-3.1.45 idna-3.11 mkdocs-git-revision-date-localized-plugin-1.5.0 mkdocs-material-9.7.0 mkdocs-material-extensions-1.3.1 paginate-0.5.7 pygments-2.19.2 pymdown-extensions-10.17.1 requests-2.32.5 smmap-5.0.2 urllib3-2.5.0

[rtd-command-info] start-time: 2025-11-13T05:51:38.025838Z, end-time: 2025-11-13T05:51:38.064083Z, duration: 0, exit-code: 0
cat mkdocs.yml
site_name: PDF Sentinel
site_description: Event-driven PDF to Markdown conversion for LLM workflows - 60x faster, zero idle resources
site_author: Ai4GenXers
site_url: https://pdf-sentinel.readthedocs.io

repo_name: Ai4GenXers/pdf-sentinel
repo_url: https://github.com/Ai4GenXers/pdf-sentinel
edit_uri: edit/main/docs/

theme:
  name: material
  palette:
    # Light mode
    - scheme: default
      primary: blue
      accent: blue
      toggle:
        icon: material/brightness-7
        name: Switch to dark mode
    # Dark mode
    - scheme: slate
      primary: blue
      accent: blue
      toggle:
        icon: material/brightness-4
        name: Switch to light mode
  features:
    - navigation.instant
    - navigation.tracking
    - navigation.tabs
    - navigation.sections
    - navigation.expand
    - navigation.top
    - search.suggest
    - search.highlight
    - content.code.copy
    - content.action.edit
  icon:
    repo: fontawesome/brands/github

plugins:
  - search
  - git-revision-date-localized:
      enable_creation_date: true

markdown_extensions:
  - admonition
  - pymdownx.details
  - pymdownx.superfences
  - pymdownx.highlight:
      anchor_linenums: true
  - pymdownx.inlinehilite
  - pymdownx.snippets
  - pymdownx.tabbed:
      alternate_style: true
  - tables
  - attr_list
  - md_in_html
  - toc:
      permalink: true

nav:
  - Home: index.md
  - Getting Started:
      - Installation: getting-started/installation.md
      - Quick Start: getting-started/quick-start.md
      - Configuration: getting-started/configuration.md
  - User Guide:
      - CLI Usage: user-guide/cli-usage.md
      - Python API: user-guide/python-api.md
      - systemd Service: user-guide/systemd-service.md
      - Conversion Engines: user-guide/conversion-engines.md
  - Architecture:
      - Overview: architecture.md
      - Performance: architecture/performance.md
      - Research Foundation: architecture/research.md
  - Troubleshooting: troubleshooting.md
  - Development:
      - Contributing: contributing.md
      - Testing: development/testing.md
      - Release Process: development/release-process.md
  - About:
      - Changelog: changelog.md
      - License: license.md

extra:
  version:
    provider: mike
  social:
    - icon: fontawesome/brands/github
      link: https://github.com/Ai4GenXers/pdf-sentinel
    - icon: fontawesome/brands/python
      link: https://pypi.org/project/pdf-sentinel/

[rtd-command-info] start-time: 2025-11-13T05:51:38.124026Z, end-time: 2025-11-13T05:51:38.537091Z, duration: 0, exit-code: 1
python -m mkdocs build --clean --site-dir $READTHEDOCS_OUTPUT/html --config-file mkdocs.yml
INFO    -  Cleaning site directory
INFO    -  Building documentation to directory: /home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/checkouts/latest/_readthedocs/html
WARNING:root:Parallel processing failed: .
 To fall back to serial processing, use 'enable_parallel_processing: False' setting.
Traceback (most recent call last):
  File "<frozen runpy>", line 198, in _run_module_as_main
  File "<frozen runpy>", line 88, in _run_code
  File "/home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages/mkdocs/__main__.py", line 370, in <module>
    cli()
  File "/home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages/click/core.py", line 1462, in __call__
    return self.main(*args, **kwargs)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages/click/core.py", line 1383, in main
    rv = self.invoke(ctx)
         ^^^^^^^^^^^^^^^^
  File "/home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages/click/core.py", line 1850, in invoke
    return _process_result(sub_ctx.command.invoke(sub_ctx))
                           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages/click/core.py", line 1246, in invoke
    return ctx.invoke(self.callback, **ctx.params)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages/click/core.py", line 814, in invoke
    return callback(*args, **kwargs)
           ^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages/mkdocs/__main__.py", line 288, in build_command
    build.build(cfg, dirty=not clean)
  File "/home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages/mkdocs/commands/build.py", line 292, in build
    files = config.plugins.on_files(files, config=config)
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages/mkdocs/plugins.py", line 593, in on_files
    return self.run_event('files', files, config=config)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages/mkdocs/plugins.py", line 566, in run_event
    result = method(item, **kwargs)
             ^^^^^^^^^^^^^^^^^^^^^^
  File "/home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages/mkdocs_git_revision_date_localized_plugin/plugin.py", line 242, in on_files
    raise e
  File "/home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages/mkdocs_git_revision_date_localized_plugin/plugin.py", line 237, in on_files
    self.parallel_compute_commit_timestamps(files=files, original_source=original_source, is_first_commit=False)
  File "/home/docs/checkouts/readthedocs.org/user_builds/pdf-sentinel/envs/latest/lib/python3.12/site-packages/mkdocs_git_revision_date_localized_plugin/plugin.py", line 198, in parallel_compute_commit_timestamps
    assert Path(abs_src_path).exists()
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^
AssertionError
