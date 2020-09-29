# wangwei-gold.github.io

gitbook build

### 建立分支 gh-pages 用于显示静态网页
git checkout -b gh-pages

### 同步拷贝 master 目录得到的 _book 到 gh-pages
git checkout master -- _book
cp -r _book/* ./

### 提交更新
git add ./*
git commit -m 'update gh-pages'
git push origin gh-pages
