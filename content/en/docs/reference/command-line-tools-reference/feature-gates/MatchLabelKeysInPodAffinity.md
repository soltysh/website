---
title: MatchLabelKeysInPodAffinity
content_type: feature_gate
_build:
  list: never
  render: false

stages:
  - stage: alpha
    defaultValue: false
    fromVersion: "1.29"
    toVersion: "1.30"
  - stage: beta
    defaultValue: true
    fromVersion: "1.31"
    toVersion: "1.32"
  - stage: stable
    defaultValue: true
    locked: true
    fromVersion: "1.33"
---

Enable the `matchLabelKeys` and `mismatchLabelKeys` fields for
[pod (anti)affinity](/docs/concepts/scheduling-eviction/assign-pod-node/).
