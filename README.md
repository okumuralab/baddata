# 政府統計のチェックリスト

三重大学教育学部 [奥村晴彦](http://oku.edu.mie-u.ac.jp/~okumura/)

## チェックリスト

* 機械判読に適したデータ形式か
* 政府標準利用規約（第2.0版）[PDF](http://www.kantei.go.jp/jp/singi/it2/densi/kettei/gl2_betten_1.pdf) に従っているか

## 具体例

### IDを付ける

県ごとのデータはJIS X 0401「都道府県コード」を付け，その順に並べる。自治体ごとのデータにも総務省[全国地方公共団体コード](http://www.soumu.go.jp/denshijiti/code.html)を付けると集約が簡単になる（参考：ウィキペディア[全国地方公共団体コード](https://ja.wikipedia.org/wiki/全国地方公共団体コード)）。

首相官邸の[地方公共団体に向けたデータフォーマット標準例](http://www.kantei.go.jp/jp/singi/it2/densi/kettei/dataformat/index.html)には「○○町」「○○町」…のように自治体名ごとにデータが列挙されているが，全国地方公共団体コードも付けることが望ましい。

IDのない対象物については，必要に応じてID付与を検討する（[北本朝展氏のツイート](https://twitter.com/KitamotoAsanobu/status/791118012107493376)参照）。

## 参考リンク

* [政府統計の総合窓口 e-Stat](http://www.e-stat.go.jp)
* 首相官邸 [電子行政オープンデータに関連する決定等](http://www.kantei.go.jp/jp/singi/it2/densi/)
* 松原勇介 [政府ホームページ利用規約の一覧](https://gist.github.com/whym/1f84065b5811ab96fd85)
* 奥村晴彦「「ネ申Excel」問題」情報処理学会情報教育シンポジウムSSS2013論文集，pp.93-98（2013年8月）[PDF](http://oku.edu.mie-u.ac.jp/~okumura/SSS2013.pdf)

