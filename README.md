static-website-basic-src
=================

タスクランナー(grunt, gulp)の使用を前提とする、サイト基本構造のテンプレートです。
ディレクトリの構造を維持するために空のディレクトリに.gitkeepを配置していますので、適宜削除してください。

このテンプレートは, 

[jade](http://jade-lang.com/)
[sass](http://sass-lang.com/) + [compass](http://compass-style.org/)
[coffee script](http://coffeescript.org/)

を使用する前提で構成しています。

data.jsonはjadeコンパイル時に読み込まれ、変数の内容がhtmlに反映されます。
index2.html
aboutUs/index2.html
は素のHTMLファイルです。jadeを使用しない場合はこちらを使用してください。

common/css/_module.scssはspritesmith([grunt-spritesmith](https://github.com/Ensighten/grunt-spritesmith), [gulp-spritesmith](https://github.com/twolfson/gulp.spritesmith))を使用する前提のmixinが含まれています。

common/css/common.scssは

```
@import 'compass';
@import 'compass/reset';
```

が記述されています。compassを使用しない場合は削除してください。
