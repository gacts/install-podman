<p align="center">
  <img src="https://github.com/gacts/install-podman/assets/7326800/d427cdc0-a49d-4153-8a75-e8c9827f0574" alt="Logo" width="140" />
</p>

# Install Podman

![Release version][badge_release_version]
[![Build Status][badge_build]][link_build]
[![License][badge_license]][link_license]

Composite GitHub Action installs a fresh Podman version in your GitHub Actions workflow.

## Usage

```yaml
jobs:
  install-podman:
    runs-on: ubuntu-latest
    steps:
      - uses: gacts/install-podman@v1
        #with:
        #  kind: unstable # `testing` by default

      - run: dnscontrol version # any dnscontrol command can be executed
```

> Tip: Use [Dependabot][use_dependabot] to maintain your `gacts/install-podman` version updated in your GitHub workflows.

## Support

[![Issues][badge_issues]][link_issues]
[![Issues][badge_pulls]][link_pulls]

If you find any action errors - please, [make an issue][link_create_issue] in the current repository.

## License

This is open-sourced software licensed under the [MIT License][link_license].

[badge_build]:https://img.shields.io/github/actions/workflow/status/gacts/install-podman/test.yml?branch=master&maxAge=30
[badge_release_version]:https://img.shields.io/github/release/gacts/install-podman.svg?maxAge=30
[badge_license]:https://img.shields.io/github/license/gacts/install-podman.svg?longCache=true
[badge_issues]:https://img.shields.io/github/issues/gacts/install-podman.svg?maxAge=45
[badge_pulls]:https://img.shields.io/github/issues-pr/gacts/install-podman.svg?maxAge=45

[link_build]:https://github.com/gacts/install-podman/actions
[link_license]:https://github.com/gacts/install-podman/blob/master/LICENSE
[link_issues]:https://github.com/gacts/install-podman/issues
[link_create_issue]:https://github.com/gacts/install-podman/issues/new
[link_pulls]:https://github.com/gacts/install-podman/pulls

[use_dependabot]:https://docs.github.com/en/code-security/supply-chain-security/keeping-your-dependencies-updated-automatically/keeping-your-actions-up-to-date-with-dependabot
