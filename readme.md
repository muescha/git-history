<div align="center">
<a href="https://github.githistory.xyz/babel/babel/blob/master/packages/babel-core/test/browserify.js">
<img alt="demo" src="https://user-images.githubusercontent.com/1911623/52460615-f3899d80-2b49-11e9-8c21-06af4097a527.gif" />
</a>
</div>

# [Git History](https://githistory.xyz)

Quickly browse the history of any GitHub ([GitLab and Bitbucket
coming soon](https://github.com/pomber/git-history/issues/14)) file:

1. Replace `github.com` with `github.githistory.xyz` in any file url
2. There's no step two

[Try it](https://github.githistory.xyz/babel/babel/blob/master/packages/babel-core/test/browserify.js)

> If you like this project consider [backing my open source work on Patreon!](https://patreon.com/pomber)  
> And follow [@pomber](https://twitter.com/pomber) on twitter for updates.

## Browser Extensions

You can also add an `Open in Git History` button to GitHub, GitLab and Bitbucket with the [Chrome](https://chrome.google.com/webstore/detail/github-history-browser-ex/laghnmifffncfonaoffcndocllegejnf) and [Firefox](https://addons.mozilla.org/firefox/addon/github-history/) extensions.

<details><summary>Or you can use a bookmarklet.</summary>

```javascript
javascript: (function() {
  var url = window.location.href;
  var regEx = /^(https?\:\/\/)(www\.)?(github|gitlab|bitbucket)\.(com|org)\/(.*)$/i;
  if (regEx.test(url)) {
    url = url.replace(regEx, "$1$3.githistory.xyz/$5");
    window.open(url, "_blank");
  } else {
    alert("Not a Git File URL");
  }
})();
```

</details>

## [CLI](https://github.com/pomber/git-history/tree/master/cli)

There's also a command line version of Git History that works with any local git repo:

> You need [node](https://nodejs.org/en/) to run this

```bash
$ npx git-file-history path/to/file.ext
```

or

```bash
$ npm install -g git-file-history
$ git-file-history path/to/file.ext
```

### Sponsors

Support this project by becoming a sponsor. Your logo will show up here with a link to your website. [[Become a sponsor](https://opencollective.com/git-history#sponsor)]

<a href="https://opencollective.com/git-history/sponsor/0/website" target="_blank"><img src="https://opencollective.com/git-history/sponsor/0/avatar.svg"></a>

### Backers

Thank you to all our backers! 🙏 [[Become a backer](https://opencollective.com/git-history#backer)]

<a href="https://opencollective.com/git-history#backers" target="_blank"><img src="https://opencollective.com/git-history/backers.svg?width=890"></a>

### Contributors

This project exists thanks to all the people who contribute.
<img src="https://opencollective.com/git-history/contributors.svg?width=890&button=false" />

### Credits

Based on these amazing projects:

- [Prism](https://github.com/PrismJS/prism) by [Lea Verou](https://twitter.com/leaverou)
- [jsdiff](https://github.com/kpdecker/jsdiff) by [Kevin Decker](https://twitter.com/kpdecker)
- [Night Owl](https://github.com/sdras/night-owl-vscode-theme) by [Sarah Drasner](https://twitter.com/sarah_edo)

## License

MIT
