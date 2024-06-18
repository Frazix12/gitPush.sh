![Banner](https://capsule-render.vercel.app/api?type=waving&color=0:24ff62,100:34a354&height=200&text=gitPush.sh&&animation=fadeIn&fontColor=ffffff&fontAlignY=34)

<p align="center">
 <img src="https://img.shields.io/badge/Made%20With-Love-20a54c?style=for-the-badge" alt="built-with-love" />
 <img src="https://img.shields.io/github/stars/Frazix12/gitPush.bat?color=20a54c&style=for-the-badge" alt="GitHub stars" />
</p>

<p align="center">
 <h2>🔥 An Open Source <strong>.sh</strong> File For Linux To Easily Push A Git Commit</h2>
</p>
<br />
<br />

# gitPush.sh

```bat
#!/bin/bash

comment="Saved on $(date '+%Y-%m-%d %H:%M:%S')"
if [ -n "$1" ]; then
  username="$1"
  comment="$comment by $username"
fi

echo "$comment"

git checkout development
git add .
git commit -m "$comment"
git push origin

```
