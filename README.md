# autocomplete-tailwind

__NOTE:__ This package is forked from [vinkla/autocomplete-tailwind](https://github.com/vinkla/autocomplete-tailwind), where it has been archived and abandoned by the previous owner.

The project is now in a state of maintenance; there is no active development. If you're here because you are using this project but the completions list is not up to date, feel free to make a pull request!

## Creating a New Version of this Package

The following process should be followed to create a new version of this package. (I'm writing these words just as much for myself as I am for anyone interested in sending a PR.)

```shell
# If the project's not set up yet:
npm i

# Grab the latest version of Tailwind CSS
npm update tailwindcss

# Run a script to update the `src/completions.json` file
npm run build

# Run tests to make sure the update hasn't broken anything
npm run test

# Perform a manual visual inspection of the completions
git diff src/completions.json
```

If nothing has failed and the inspection goes well enough, you're ready to create a new version! All this means is that you crack open `package.json` and bump the version number. After that's done, send a pull request!

[MIT](LICENSE) © [Ray Brown](https://raybrown.co)
