# Handy reminders for developers

Things we use

* nx - for building and releasing (all behind yarn scripts)

## Font versioning

Font package versions are now independent of upstream font versions and we track the mapping in the README.md

## Publishing

This will auto detect which packages need to be published on NPM and ask which versions you want to set the packages to.

```sh
yarn release
```

## Building

```sh
# Regenerate and update the font packages
yarn generate

# Build everything
yarn prepare
```

## Alpha release

```sh
# Add --dry-run to test
yarn nx release version --verbose --package @react-native-vector-icons/lucide --preid=alpha
yarn nx release publish --verbose --package @react-native-vector-icons/lucide --tag alpha
```
