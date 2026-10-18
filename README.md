# pohstep/tap

Homebrew recipes for pohstep's Mac apps.

## Install

```sh
brew tap pohstep/tap
brew install --cask wordbit
brew install --cask chief-status
```

| App | What it does | Source |
| --- | --- | --- |
| [Wordbit](https://github.com/pohstep/wordbit) | One new English word a day in your Mac menu bar | `Casks/wordbit.rb` |
| [Chief Status](https://github.com/pohstep/chief-status) | Shows which of your AI bots are working, done or stuck, in your Mac menu bar | `Casks/chief-status.rb` |

## The apps are unsigned

These apps are not signed by Apple, so the first time you open one, macOS says it can't verify the app. To open it anyway, do one of these once:

- In **Applications**, right-click the app and choose **Open**, then **Open** again.
- Or go to **System Settings → Privacy & Security** and click **Open Anyway**.
- Or, in Terminal:

  ```sh
  xattr -d com.apple.quarantine /Applications/Wordbit.app
  xattr -dr com.apple.quarantine "/Applications/Chief Status.app"
  ```

## Update or remove

```sh
brew upgrade --cask wordbit
brew uninstall --cask wordbit
brew upgrade --cask chief-status
brew uninstall --cask chief-status
```
