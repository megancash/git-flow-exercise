# 8 Completed Release

| Date | Phase |
| --- | --- |
| February 28<sup>th</sup> | Release |

It is the last day of the month and no more requests have come in from the, time to push the code to production and merge changes to the release back into the `develop` branch.

## :running: Activities

### 1 - Merge Release Branch into `main`

__One Team Member__

Merge `release-1.1.0` into `main`.

```sh
$ git checkout release-1.1.0

$ git pull

$ git checkout main

$ git pull

$ git merge --no-ff release-1.1.0

$ git push
```


### 2 - Merge Release Branch into `develop`

__One Team Member__

Next we will work to get changes made to the release merged back down into `develop`, so switch to the release branch and pull down all the latest changes:
```sh
$ git checkout release-1.1.0

$ git checkout develop

$ git merge --no-ff release-1.0.0

$ git push
```

:bulb: Always make sure that `develop` is up to date before merging. There may be some merge conflicts that will need to be addressed at this point.


### 3 - Create a Release tag in GitHub

__One Team Member__
Choose one team member to create a Release in GitHub:

1. On the source repository page, click the "# releases" link in the stats bar at the top (or append `/releases` to the repo URL).
2. Click new release.
3. Name the release tag v1.1.0, choose the main branch, and document the changes comprising the release.

The release feature in GitHub is an easy way to keep track of changes associated with each release. Files may also be uploaded and attached to the release, so they can also act as a place to store any additional files related to the release that are not tracked in version control.


## :tada: We're done!

You did it! Feel free at this time to navigate around the source repository, yours and others' forks and reflect back on all the hard work that was done to get v1.1.0 out the door :sunglasses:.

## Quick Links

- [Readme](../readme.md)
- [1. Setup](1-setup.md)
- [2. Feature Branches](2-feature-branches.md)
- [3. Code Review](3-code-review.md)
- [4. Fetching Latest](4-fetching-latest.md)
- [5. Hotfix](5-hotfix.md)
- [6. Release Branch](6-release-branch.md)
- [7. Release Bugs](7-release-bugs.md)
