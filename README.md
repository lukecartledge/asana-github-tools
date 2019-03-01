# Asana and Github tools for better project management.

**_Features:_**

1. Asana Task ID - Automatically assign Task numbers to newly created Asana cards (eg. FR-1)
2. Asana/Github Sync - Automatically assign and update card status (Draft, Review, Approved, Staging, Production) based on a Github Pull Request's status (Coming soon).

**_Getting started:_**

1. Add the following variables into a .env file in the root folder of this app:

```
BASE_URL=https://featureready.herokuapp.com
PRODUCTION_BRANCH_NAME=master
STAGING_BRANCH_NAME=develop
GITHUB_PATOKEN=GGGG
GITHUB_OWNER_NAME=yoongfook
GITHUB_REPO_NAME=featureready
ASANA_PATOKEN=0/9cccccccccccccccccccccccccccc
ASANA_WORKSPACE_ID=111122222223333333
ASANA_PROJECT_ID=1111222224444444
ASANA_PROJECT_PREFIX=FR
```

2. Run `npm setup-tags` to setup all the required tags/custom-fields on your Asana project

3. Run `npm setup-hooks` to setup all required hooks when creating a task etc

**_Useful commands_**

`npm list-hooks` - lists all hooks on Asana