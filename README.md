# Specify home directory for zipping Cypress tests

See https://www.browserstack.com/docs/automate/cypress/home-directory

## Work around

If needing to include files outside of the tests directory AND need to define additional npm dependencies, i.e. `npm_dependencies`, the must include `"exclude": ["FolderB/bstackPackages.tar.gz"]` in `browserstack.json`

```bash
cd FolderB
browserstack-cypress run
```