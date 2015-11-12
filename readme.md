## Structure

```
// replace this with `tree` later
package.json
readme.md
license
build/
bin/
  - newPost
  - pagespeed (psi)
  - size
    - list sizes of major files in dist
  - deploy
    - bump version number
    - commit changes in dist sub-repo
    - push dist
gulpfile.js/
  general
    merge-stream
    gulp-if
    streamqueue
    lazypipe
    sourcemaps
    minification
    gulp-rev in prod
    source maps in dev
    gulp-load-plugins
    gulp-filter
    gulp-regex-rename
    browser-sync for dev
    fail hard in prod tasks; plumber dev
    gulp-useref? / gulp-processhtml? / gulp-preprocess?
    gulp-replace?
    incremental builds
    - changed
    - newer
    - cached
    - remember
source/
  - extras
    - CNAME       // for github url
    - robots.txt  // for search engines
    - humans.txt  // for nerds
    - sitemap.xml // for search engines
    - feed.xml    // for feed readers
    - crossdomain.xml
    - browserconfig.xml
    - favicon.ico // generate all favicons
  - images        // minify and rev
  - markup        // jade/md -> html
    - pages       // jade pages
    - posts       // md posts with frontmatter
    - templates   // jade templates used by pages + posts
  - scripts       // es6 + browserify -> js
    - main        // load at end of <body>
    - post        // post-specific scripts
  - styles        // stylus? -> css
```

good gulp examples:
- vigetlabs/gulp-starter
- roots/sage
- google/web-starter-kit
- cferdinandi/kraken
