# svm - Semantic Version Manager

Utility to manage [Semantic Versioning](https://semver.org) in your projects.

## Requirements

- PHP 8.x

## Usage

```bash
svm bump|dry-bump|bump-and-tell -M|--major | -m|--minor | -p|--patch <VERSION_FILE>
```
### Commands

- bump - Bump the version according to the flag supplied, rewrites the file;
- bump-and-tell - Bump the version according to the flag supplied, rewrites the file and outputs the bumped version to STDOUT;
- dry-bump - Bump the version according to the flag supplied, ouputs it to STDOUT, doesn't rewrites the file.

### Flags

Should be obvious, but anyway:

- -M|--major - Bumps Major, Resets minor and patch
- -m|--minor - Bumps minor, Resets patch
- -m|--minor - Bumps patch

## Roadmap

### Version 1.0.0 (you're here):

- Bumps and resets numbers based on the simplest semantric versioning (item #2 of the spec);
- Rewrites the version file automatically if instructed;
- Only outputs the bumped version if instructed;
- Alternatively, both rewrite the file AND outputs the bumped version.

### Version 2.0.0

- Do the same with pre-release versions (item #9 of the spec);
- Take correct precedence into consideration.

### Version 3.0.0

- Deal with metadata (item #10 of the spec);
- Take correct precedence into consideration.
