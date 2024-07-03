# demo- name:  asdf
  sourceRepos:
  - '*'
  clusterResourceWhitelist:
    - group: ""
      kind: Namespace
    # also allow kargo Project cluster resource,
    # all details why is documented currently in
    # https://github.com/akuity/kargo/issues/2058
    - group: kargo.akuity.io
      kind: Project
  appOfAppsRepo:
    repoURL: https://github.com/suxess-it/asdf-apps
    path: k3d-apps
    revision: main
  multiStageKargoAppSet:
    organization: suxess-it
- name:  dd
  sourceRepos:
  - '*'
  clusterResourceWhitelist:
    - group: ""
      kind: Namespace
    # also allow kargo Project cluster resource,
    # all details why is documented currently in
    # https://github.com/akuity/kargo/issues/2058
    - group: kargo.akuity.io
      kind: Project
  appOfAppsRepo:
    repoURL: https://github.com/suxess-it/dd-apps
    path: k3d-apps
    revision: main
  multiStageKargoAppSet:
    organization: suxess-it
