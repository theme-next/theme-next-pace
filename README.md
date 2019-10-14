<h1 align="center"><a href="https://github.com/HubSpot/pace">Progress bar</a> for <a href="https://github.com/theme-next">NexT</a></h1>

<h1 align="center">Installation</h1>

<h2>If you want to use the CDN instead of clone this repo, please jump to the Step 3.</h2>

<h2 align="center">Step 1 &rarr; Go to NexT dir</h2>

Change dir to **NexT** directory. There must be `layout`, `source`, `languages` and other directories:

```sh
$ cd themes/next
$ ls
_config.yml  crowdin.yml  docs  gulpfile.js  languages  layout  LICENSE.md  package.json  README.md  scripts  source
```

<h2 align="center">Step 2 &rarr; Get module</h2>

Install module to `source/lib` directory:

```sh
$ git clone https://github.com/theme-next/theme-next-pace source/lib/pace
```

<h2 align="center">Step 3 &rarr; Set it up</h2>

Enable module in **NexT** `_config.yml` file and select your theme:

```yml
pace:
  enable: true
  # Themes list:
  # big-counter | bounce | barber-shop | center-atom | center-circle | center-radar | center-simple
  # corner-indicator | fill-left | flat-top | flash | loading-bar | mac-osx | material | minimal
  theme: minimal
```

**And, if you wants to use the CDN, then need to set:** (you also need to find your corresponding theme css link in <a href="https://www.jsdelivr.com/package/npm/pace-js?path=themes">jsdelivr</a>)

```yml
vendors:
  ...
  pace: //cdn.jsdelivr.net/npm/pace-js@1/pace.min.js
  pace_css: //cdn.jsdelivr.net/npm/pace-js@1/themes/blue/pace-theme-minimal.css
```

<h1 align="center">Update</h1>

```sh
$ cd themes/next/source/lib/pace
$ git pull
```
