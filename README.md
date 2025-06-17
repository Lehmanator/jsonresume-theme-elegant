# Elegant Theme

[![npm version](https://badge.fury.io/js/jsonresume-theme-elegant.svg)](http://badge.fury.io/js/jsonresume-theme-elegant)

Responsive theme for [JsonResume](https://jsonresume.org/) inspired by card layouts.

[Theme Preview](https://themes.jsonresume.org/theme/elegant)

### Markdown Supported

Supports the following properties:

- `resume.basics.summary`
-  `work[0].summary`
-  `work[0].highlights`
-  `projects[0].summary`
-  `projects[0].highlights`
-  `education[0].courses`
-  `volunteer[0].summary`
-  `volunteer[0].highlights`
-  `awards[0].summary`
-  `publications[0].summary`
-  `references[0].reference`
-  `skills[0].keywords`

If you need more, please file an issue.

### Social Profiles

The profiles are shown in the order in which they are specified in the `basics.profiles` array.
By default, only 5 profiles are shown & others are revealed on demand.

![Profile Section](https://raw.githubusercontent.com/Lehmanator/jsonresume-theme-elegant/main/screenshots/profile.png)

#### Supported Profiles

* `angellist`
* `behance`
* `bitbucket`
* `blogger`
* `codepen`
* `dribbble`
* `dribble`
* `exercism`
* `facebook`
* `flickr`
* `foursquare`
* `github`
* `gitlab`
* `googleplus`
* `gratipay`
* `hackernews`
* `instagram`
* `lastfm`
* `linkedin`
* `medium`
* `meetup`
* `pinterest`
* `reddit`
* `skype`
* `soundcloud`
* `spotify`
* `stackexchange`
* `stackoverflow`
* `telegram`
* `tumblr`
* `twitter`
* `vimeo`
* `youtube`

### Credits

Special thanks to:

- [mudassir0909](https://github.com/mudassir0909): for the [original project](https://github.com/mudassir0909/jsonresume-theme-elegant) this project was originally based on.
- [jenshenneberg](https://github.com/jenshenneberg): for the [fork](https://github.com/mudassir0909/jsonresume-theme-elegant) this project is based on.
- [all contributors to the original project](https://github.com/mudassir0909/jsonresume-theme-elegant/graphs/contributors): for your pull requests.
- [all contributors to this project](https://github.com/Lehmanator/jsonresume-theme-elegant/graphs/contributors): for your pull requests.
- [Smart Fixed Navigation](http://codyhouse.co/demo/smart-fixed-navigation/index.html): for inspiration for the Floating Menu.

### Contributing

```
$ npm install -g grunt
$ npm install -g pug-cli
$ git clone https://github.com/Lehmanator/jsonresume-theme-elegant.git
$ cd jsonresume-theme-elegant
$ npm install
$ grunt watch           // watches for file changes in *.pug & *.less
$ grunt exec:run_server // Do this in a new terminal tab to run node server
```

Visit [http://localhost:8888](http://localhost:8888) to see the theme in action.

##### Testing JSON changes

You can test your changes by updating `resume.json` file inside `node_modules/resume-schema/` folder.
You might want to rerun `grunt exec:run_server` whenever you make any changes to `resume.json`

##### Updating Styles

All the LESS files are organized under the folder `assets/less/`.
Please go through the comments inside `theme.less` to find out which file to put your LESS changes.
Grunt compiles `assets/less/theme.less` to `assets/css/theme.css` which is used eventually in the theme.

**_Please Do not make any changes inside `assets/css/theme.css`_**

##### Updating Javascript

All the javascript changes go into `index.js` which is responsible for rendering the theme.

##### Adding a new icon

Visit this [wiki page](https://github.com/mudassir0909/jsonresume-theme-elegant/wiki/Adding-a-new-icon) on the original project's repo.

### Roadmap

[https://github.com/Lehmanator/jsonresume-theme-elegant/labels/enhancement](https://github.com/Lehmanator/jsonresume-theme-elegant/labels/enhancement)

- [ ] Add icons for additional social platforms.
  - [ ] Codeberg / Forgejo / Gitea
  - [ ] Fediverse / ActivityPub servers
  - [ ] Mastodon
  - [ ] Matrix
  - [ ] Signal
  - [ ] Sourcehut

- [ ] GitHub Actions
  - [ ] Build, lint, & test
  - [ ] Deploy to GitHub Pages

- [ ] Forgejo Actions
  - [ ] Build, lint, & test
  - [ ] Deploy to Codeberg Pages

- [ ] Test compatibility with JSONResume schema.
