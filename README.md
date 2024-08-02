# Bock

## Development

### [Recommended] Contribute to this project in your browser. 

1. [Navigate to this project in nimba.dev](https://www.nimba.dev/projects/bock)
2. Create / Go To a Task record.
3. In the `Developer` card, click "Assign" and select yourself.
4. Click `Create Org` (NOT `Create Scratch Org`)

### [Advanced] Contribute to this project on your device. 

1. [Set up CumulusCI](https://cumulusci.readthedocs.io/en/latest/tutorial.html) in your preferred development environnment.
2. Run `cci flow run dev_org --org dev` to deploy this project.
3. Run `cci org browser dev` to open the org in your browser.

## Releases

### To release a new `beta` version of this package:

1. Run `git checkout main` to switch to the main branch.
2. Run `git pull` to download the latest changes from Github.
3. Run `cci flow run release_unlocked_beta --org dev --debug` to release a new beta version of this package.
4. Run `cci org browser dev` to open the org in your browser.

### To release a new `production` version of this package:

1. Run `git checkout main` to switch to the main branch.
2. Run `git pull` to download the latest changes from Github.
3. Run `cci flow run release_unlocked_production --org dev --debug` to release a new beta version of this package.
4. Run `cci org browser dev` to open the org in your browser.
5. [OPTIONAL] Run `cci flow run install_prod --org <target-org-alias>` to install the package and _all of its dependencies_ in `<target-org-alias>`.
