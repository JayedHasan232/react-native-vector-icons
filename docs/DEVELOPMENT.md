# Handy reminders for developers

Things we use

* nx - for building and releasing (all behind pnpm scripts)

## Font versioning

Font package versions are now independent of upstream font versions and we track the mapping in the README.md

## Publishing

This will auto detect which packages need to be published on NPM and ask which versions you want to set the packages to.

```sh
pnpm run release
```

## Building

```sh
# Regenerate and update the font packages
pnpm run generate

# Build everything
pnpm run prepare
```

## Alpha release

```sh
# Add --dry-run to test
pnpm nx release version --verbose --package @react-native-vector-icons/lucide --preid=alpha
pnpm nx release publish --verbose --package @react-native-vector-icons/lucide --tag alpha
```
