---
layout: post
title: "Blog update process"
date: 2013-04-15 14:21
comments: true
categories: [Octopress]
---
Clone Repository
``` bash
git clone https://github.com/username/username.github.com.git -b source
cd username.github.com
git clone https://github.com/username/username.github.com.git -b master _deploy
cd ..
```

Blog Posts
``` bash
rake new_post["title"]
# creates /source/super-awesone/index.markdown
```
Generate/Preview/Deploy
``` bash
rake generate # Generates posts and pages
rake preview  # Watches, and mounts a webserver at http://localhost:4000
rake deploy   # Deploy blog to github
```

Commit source
``` bash
git add .
git commit -m 'your message'
git push
```
