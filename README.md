<p align="center"><a href="//writebar.js.org" title="writebar.js.org"><img src="assets/logo.svg"/></a></p>
<h1 align="center">WriteBar</h1>
<p align="center">
  Experimental distraction-free text editor,<br/>
  that displays focus text line right over the keyboard (on the Macbook Pro TouchBar).
</p>
<h2 align="center">
  <a href="//github.com/alexander-shvets/writebar/releases">ChangeLog</a>
  | 
  <a href="dist/WriteBar.dmg">v0.2.1-beta.dmg</a>
</h2>
<p align="center"><a href="//facebook.com/groups/uxclubs/permalink/973396292808999/"><img width="600" src="assets/screenshot.jpg" alt="screenshot"/></a></p>

### Discuss

- [Intro Video post @ Facebook UX Club](//facebook.com/groups/uxclubs/permalink/973396292808999/)
- [Feature Requests and Issues @ GitHub](//github.com/alexander-shvets/writebar/issues)     

## Development

Download source code:    
```shell
git clone git@github.com:alexander-shvets/writebar.git
cd writebar
```

Install (or update) macOS package manager ([Homebrew][]):
```shell
brew update || /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Install Node package manager ([yarn][]):
```shell
yarn || brew install yarn
```

Install application dependencies:
```shell
yarn
```

Install (global or local) dev-dependencies*:    
```shell
yarn global add electron
yarn global add electron-packager
yarn global add electron-installer-dmg
```
_* doesn't listed in [`package.json`][] becouse I doesn't use js builder yet (which will exclude unused dependencies from application installation package)_

Run app in dev mode:    
```shell
yarn start
```

Build App and Installation Package (dmg):    
```shell
yarn packdist
```
Release files should be generated in [`dist`][] directory.

[`package.json`]: //github.com/alexander-shvets/writebar/blob/master/package.json
[`dist`]: //github.com/alexander-shvets/writebar/tree/master/dist
[Homebrew]: //brew.sh
[yarn]: //yarnpkg.com

