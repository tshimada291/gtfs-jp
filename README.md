# gtfs-jp-list
日本国内で公開されている「標準的なバス情報フォーマット」およびGTFSのオープンデータ一覧です。

## Caution
**当リストに掲載しているデータの「品質」は保証していません。（当リストは、掲載されているデータの品質を保証・認証するものではありません。）** 現在、一部のGTFS/GTFS-JPオープンデータ・公開データについて不正確なデータが掲載されている事例が確認されています。 **時刻案内や経路案内など正確性を要するアプリやシステム等への利用（有償・無償限らず）やその他商用・有償サービスでの利用、あるいは研究・分析目的の利用を検討している場合は、以下の点について十分に確認のうえ、利用目的にそぐわないデータについては利用を控える・除外するようお願いいたします。**（可能であれば、データ提供元（feed_publisher）への連絡・情報提供をお願いいたします。）
* **データの有効期限切れ**（feed_info.txtのfeed_end_date（無い場合はcalendar.txtのend_date、またはcalendar_dates.txtの最後の日付）が期限を過ぎている（当リストの「feed_end_date」から判別可能です）） 
  * ダイヤ改正に対応できていない可能性があります。
  * ダイヤ改正は無いものの、期限だけ更新されていない（データ提供元が期限の更新を失念している）場合もあります。
* **停留所・標柱情報（stops.txt）の位置情報が不正確**
  * のりばの位置が本来の位置を示さずに、ある1か所（道路の真ん中、交差点の真ん中など）に重なっている
* **最新のダイヤに対応していない**
  * 有効期限内となっているが、古いダイヤ情報が残っていたり、新しい路線・便の情報が未掲載・抜けているケースが確認されています。
  * 時刻や経路の案内に使用した際、現存しない便やのりば等を案内したり、新設された便やのりば等を案内できない事態が考えられます。
    * アーカイブとして残されている過去データについてはこれに該当しません。
* その他
  * 経路データや運賃データの登録誤りなどがあります。

## URL
* GTFS / GTFS-JP (static data list)
  * https://tshimada291.github.io/gtfs-jp-list/gtfs-jp-list.csv 
* GTFS-RT (realtime data list)
  * https://tshimada291.github.io/gtfs-jp-list/gtfs-rt-list.csv

## License
[Creative Commons — CC0](https://creativecommons.org/publicdomain/zero/1.0/)
* [CC0について (Creative Commons Japan)](https://creativecommons.jp/sciencecommons/aboutcc0/)

## Attribute
* 静的データリスト
  * official：公式・公認のデータであれば1、個人等による作成データの場合は0としています。
  * fixed_url：配信元のzipデータURLが固定URLであれば1、なければ0としています。（直近の状況をみて指定しているため、変わる場合があります。）
  * api_key：APIキーが必要であれば1、なければ0としています。
* 動的データリスト
  * rt_api_key：APIキーが必要であれば1、なければ0としています。
  * interval_sec：データ更新間隔を秒単位で記してあります。（配信サイトに記載ない場合は空欄としています。）

## Notice
* 静的データリストの更新はおおむね1週間に1回を予定しています。
  * 動的データリストについては不定期となります。 
* 試験公開につき、ファイルの内容について項目名などを変更する場合があります。

## History
2021.3.5　掲載開始

## External links
* [GTFS・「標準的なバス情報フォーマット」オープンデータ一覧](https://tshimada291.sakura.ne.jp/transport/gtfs-list.html)
* [GTFS.JP](https://www.gtfs.jp/)
