---
title: about hexo
date: 2018-01-04 22:18:39
tags:
---

github를 이용해서 blog를 하기
위해 [hexo](https://hexo.io/ko/index.html)를 적용해 보았다.  jekyll
보다 훨씬 쉬워서 맘에
든다. [이곳](http://futurecreator.github.io/2016/06/21/hexo-basic-usage/)에서
많은 도움을 얻었다.

# 자주 사용하는 명령어

```
hexo new [layout] <title>
hexo serve -o
hexo serve --draft -o
hexo g -d
hexo g -w
```

# 글을 작성 하는 방법

```
hexo new "aaa"
hexo g
hexo serve -o
hexo d
```

# 글을 삭제 하는 방법

```
rm source/_post/a.md
hexo clean # delete database file, public folder
hexo g
hexo serve -o
hexo d
```
