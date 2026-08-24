# homebrew-tap

Personal Homebrew tap.

## ccmux

Runs each Claude Code session on a chosen Claude subscription or API key, and moves a live
session between them without restarting it.

```
brew install --cask vovean/tap/ccmux
```

Apple Silicon, macOS 14 or newer. Source: [vovean/ccmux](https://github.com/vovean/ccmux).

After installing:

```
ccmux shell-init >> ~/.zshrc   # cc-opus / cc-fable / cc-any wrappers
ccmux install-agent            # start at login (optional)
```

The build is ad-hoc signed rather than Developer ID signed and notarized, so the cask
clears the quarantine flag on install — otherwise Gatekeeper refuses a downloaded copy.
