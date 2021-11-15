# BoganParts
Various parts and designs by the MakerBogan group.

Basic idea is to have a low friction area with version history for MakerBogan designs.  
'PullRequest' is really just to check 'into a directory owned by that user' and not some weird rebasing.  
Obviously if you would like feedback, the Github system supports that too, but it is NOT required for merge.

# General operation
2 recommended modes

## Mode 1: General users working areas
Branch from master and with the directory structure of ```<username>-WIP``` (work in progress)

This is yours to play / rebase / rework as you need.  Basically a cloud based backup and common area that others can see.  DonBe nice and don't push to other peoples branches.

## Mode 2: Something worth keeping / publishing
Branch from currrent master, normally something like ```<username>-MyCoolNewWidget```

Add directory with the cleaned / squashed 'released' version of your widget
```<username>/MyCoolNewWidget/```

Nominally include a README.md and stl / 3mf / photos files and anything else you might want

Generate a merge PR and we can merge it quickly.
