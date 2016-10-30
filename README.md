# 政府統計のチェックリスト

三重大学教育学部 [奥村晴彦](http://oku.edu.mie-u.ac.jp/~okumura/)

まだ書き始めたばかりの初期段階です。ご意見は[Issues](https://github.com/okumuralab/baddata/issues)にどうぞ。

## チェックリスト

* 機械判読に適したデータ形式か（PDFは不適。Excel形式か，可能ならCSV，JSONを使う）
* [政府標準利用規約（第2.0版）](http://www.kantei.go.jp/jp/singi/it2/densi/kettei/gl2_betten_1.pdf) または同じことだが [CC BY](https://creativecommons.org/licenses/by/4.0/legalcode.ja) に従っているか（参考：松原勇介 [政府ホームページ利用規約の一覧](https://gist.github.com/whym/1f84065b5811ab96fd85)）
* 永続的なURLを使っているか（参考：[国の機関サイトの残存率](http://warp.ndl.go.jp/contents/reccommend/collection/linkrot.html) 5年で60%が消滅）

## 具体例

工事中

### 一覧情報が不足

<blockquote class="twitter-tweet" data-lang="ja"><p lang="ja" dir="ltr">実は、学校の「校名・住所・電話番号・URL・メールアドレス」の５つ組は、文部科学省のどこもデータを持っていない。それでは緊急時に連絡のしようがない。それはまずいと思い、全学校の基本情報をオープンデータにするサービスを始めます。それがedumap。　<a href="https://twitter.com/hashtag/netcommons?src=hash">#netcommons</a></p>&mdash; norico arai (@noricoco) <a href="https://twitter.com/noricoco/status/491553304652951552">2014年7月22日</a></blockquote> <script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

→ [edumap](http://www.edumap.jp)

例えば全国自治体について，ホームページから情報を自動収集したり，○○担当部局に郵便を出す必要が生じた場合，地方公共団体コード（あるいは国税庁の法人番号）・公式ホームページURL・郵便番号付き住所等を対応づけるデータが欲しいが，人間が地道に探さないと簡単には得られない。

### IDを付ける

<blockquote class="twitter-tweet" data-lang="ja"><p lang="ja" dir="ltr"><a href="https://twitter.com/noricoco">@noricoco</a> <a href="https://twitter.com/h_okumura">@h_okumura</a> <a href="https://twitter.com/konotarogomame">@konotarogomame</a> 機械可読も大事ですが、私はIDの重要性を訴えたいです。IDは複数のデータを紐付ける基盤で、政府が一元付与・運用すれば皆で共有できる。道路の話で言えば、実は高速道路さえ公的IDがないのですよ。ビックリです。</p>&mdash; 北本 朝展 (@KitamotoAsanobu) <a href="https://twitter.com/KitamotoAsanobu/status/791118012107493376">2016年10月26日</a></blockquote> <script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

県ごとのデータはJIS X 0401「都道府県コード」を付け，その順に並べる。自治体ごとのデータにも総務省[全国地方公共団体コード](http://www.soumu.go.jp/denshijiti/code.html)を付けると集約が簡単になる（参考：ウィキペディア[全国地方公共団体コード](https://ja.wikipedia.org/wiki/全国地方公共団体コード)）。

首相官邸の[地方公共団体に向けたデータフォーマット標準例](http://www.kantei.go.jp/jp/singi/it2/densi/kettei/dataformat/index.html)には「○○町」「○○町」…のように自治体名ごとにデータが列挙されているが，全国地方公共団体コードも付けることが望ましい。

## 参考リンク

* [政府統計の総合窓口 e-Stat](http://www.e-stat.go.jp)
* 首相官邸 [電子行政オープンデータに関連する決定等](http://www.kantei.go.jp/jp/singi/it2/densi/)
* 総務省 [オープンデータ戦略の推進](http://www.soumu.go.jp/menu_seisaku/ictseisaku/ictriyou/opendata/)
* 奥村晴彦 [「ネ申Excel」問題](http://oku.edu.mie-u.ac.jp/~okumura/SSS2013.pdf) 情報処理学会情報教育シンポジウムSSS2013論文集，pp.93-98（2013年8月）
* Tim Berners-Lee [クールなURIは変わらない](http://www.kanzaki.com/docs/Style/URI)
