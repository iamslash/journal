---
title: how to build blender on windows
date: 2018-01-05 14:09:39
tags:
---

blender를 windows10에서 visual studio 2015를 이용하여 build해보자.
[이곳](https://wiki.blender.org/index.php/Dev:Doc/Building_Blender/Windows)을 참고하여
Subversion, Git, CMake, Visual Studio 2015 등등 필요한 응용 프로그램들을 설치한다.

```
cd c:\blender-git
git clone git://git.blender.org/blender.git
cd blender
git submodule update --init --recursive
git submodule foreach git checkout master
git submodule foreach git pull --rebase origin master
cd ..
svn checkout https://svn.blender.org/svnroot/bf-blender/trunk/lib/win64_vc14  lib/win64_vc14
cd blender
make full nobuild debug x86 2015
```

make help를 이용하면 자세한 옵션을 알아낼 수 있다.



