# smartsync
===================================

#Author
-----------------------------------
Guangyi Meng tdxmgy@gmail.com

About Smartsync
-----------------------------------
repo smart sync using manifest from a known good build

repo sync --help
Usage: repo sync [<project>...]

Options:
  -h, --help            show this help message and exit
  -f, --force-broken    continue sync even if a project fails to sync
  -l, --local-only      only update working tree, don't fetch
  -n, --network-only    fetch only, don't update working tree
  -d, --detach          detach projects back to manifest revision
  -c, --current-branch  fetch only current branch from server
  -q, --quiet           be more quiet
  -j JOBS, --jobs=JOBS  projects to fetch simultaneously (default 1)
  -m NAME.xml, --manifest-name=NAME.xml
                        temporary manifest to use for this sync
  --no-clone-bundle     disable use of /clone.bundle on HTTP/HTTPS
  -u MANIFEST_SERVER_USERNAME, --manifest-server-username=MANIFEST_SERVER_USERNAME
                        username to authenticate with the manifest server
  -p MANIFEST_SERVER_PASSWORD, --manifest-server-password=MANIFEST_SERVER_PASSWORD
                        password to authenticate with the manifest server
  --fetch-submodules    fetch submodules from server
  --no-tags             don't fetch tags
#  -s, --smart-sync      smart sync using manifest from a known good build
  -t SMART_TAG, --smart-tag=SMART_TAG
                        smart sync using manifest from a known tag

  repo Version options:
    --no-repo-verify    do not verify repo source code

#Infrastructure
-----------------------------------
1.Submit a snapshot xml file to manfeist server when the code build successfully.
2.Run repo sync -s commond to get the known latest good build code.

#License
-----------------------------------
is released under BSD license.
