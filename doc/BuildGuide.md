# ビルドガイド

> [!TIP]
> Github右上のリストボタン押下で目次（アウトライン）が表示され、工程全体を把握しやすくなります。
![2025-03-06_06h52_32](https://github.com/user-attachments/assets/600b59ae-39ec-4d79-b8a6-39246b630301)

　
## 準備
### キット内容物の確認

| 名前 | 数 |
|:-|:-|
|PCB（左右＋Dpad基板）|1式|
|トラックパッドモジュール|1個|
|Dパッドモジュール用カバー|1式|
|マイクロスイッチ|4個|
|ロータリーエンコーダー|2個|
|エンコーダーノブ|2個|
|ホットスワップソケット|48個|
|FFC（フレキシブルフラットケーブル）12PIN|1個|
|FFC（フレキシブルフラットケーブル）5PIN|1個|
|キーボードケース|1式|
|電源スイッチカバー|2個|
|マイコンカバー＆リセットピン|2個|
|マグネット|8個|
|メタルプレート|2個|
|滑り止めシール(2025/04/11～出荷分)|8枚|
|M3ネジ|8本|

![2025-03-07_06h03_27](https://github.com/user-attachments/assets/d0671da1-67af-4749-8326-778872f7eb3c)
<br/><br/><br/>
### 別途ご用意いただくもの

| 必須 | 名前 | 数 | 備考 |参考商品|
|:-|:-|---:|:-|:-|
|★|Seeed Studio XIAO nRF52840 |2個|マイコン本体。安価で入手性が高く、通信も安定しています。|[秋月電子](https://akizukidenshi.com/catalog/g/g117341/)|
|★|Kailh Choc V2互換スイッチ|48個|個人的にDeepSeaMiniがおすすめ。Lofreeなども適合。ChocV1も一応刺さります。|[遊舎工房](https://shop.yushakobo.jp/collections/all-switches/Kailh-Choc-V2%E3%82%B9%E3%82%A4%E3%83%83%E3%83%81) [Kailhswitch](https://kailhswitch.net/products/kailh-deep-sea-silent-min-low-profile-keyboard-switch)|
|★|MX軸ロープロファイルキーキャップ|48個|MX軸なら通常キーキャップも一部適合。|[Womier](https://womierkeyboard.com/products/skyline-r2) [Amazon](https://www.amazon.co.jp/stores/page/90526727-85E5-4BF8-AAD2-FC8A78C07BE3/search?ref_=ast_bln&store_ref=bl_ast_dp_brandLogo_sto&terms=%E3%83%AD%E3%83%BC%E3%83%97%E3%83%AD)|
|★|3.7Vリチウムポリマーバッテリー|2個|厚さ6.3mm幅47mm長さ110mm以下、JST PHコネクタ（ソケットのピッチ2.0mm）※[ソケットの極性に注意！](#%E3%83%90%E3%83%83%E3%83%86%E3%83%AA%E3%83%BC%E5%8F%96%E3%82%8A%E4%BB%98%E3%81%91)|[Amazon](https://www.amazon.co.jp/dp/B09DRJS75J/) [PHコネクタ単品](https://www.amazon.co.jp/dp/B01MXGWMS5/) |
|★|USB-Cケーブル|2本|充電、ファームウェア書き込み用。何百回と抜き差しする事になるのでマグネット式がおすすめ。||
||ケースの滑り止め|1式|グリップラスが評判良いです。テントするなら不要。4月出荷分から同梱済み|[Amazon](https://www.amazon.co.jp/dp/B08C9Z2K4C/])
||テンティング用品|2セット|マグネット式スタンドor三脚orクランプアーム。テントしないなら不要。|[Cramp](https://www.amazon.co.jp/dp/B08LCZ2X7M/) [Magnet](https://www.amazon.co.jp/dp/B0CXPR9BMF/) [Stand1](https://www.amazon.co.jp/dp/B0DKFMLWFX/) |★[Stand2](https://www.amazon.co.jp/dp/B0B6DSD1RK/)|

### 道具類

|必須| 名前 | 備考 |参考商品|
|:-|:-|:-|:-|
|★|はんだごてセット|アマゾンの温度調整付きはんだごて改善版15点セット（ピンセット、はんだ吸い取り線、フラックス、３C型のこて先入り）がおすすめ。|[amazon](https://www.amazon.co.jp/dp/B0CM1WJB5X/)|
|★|プラスドライバー|M3ネジ締める用。||
||フラックスクリーナー|フラックスで基板がべとべとになるので掃除用。||
||両面テープ|バッテリー固定用。無ければマスキングテープやビニテやガムテなどで代用可。||
||ピンセット|はんだ中のパーツ固定用。||
||マスキングテープ|はんだ中のパーツ固定用。||
||ニッパー|基板の分離用。||
||テスター|あると電源投入前に配線のショートをチェックできるので怖さが減ります。またトラブル発生時の問題の特定や、サポートのやりとりするために大変有用となっています。ワニ口タイプなら細いピン等を掴む事で細かい端子までチェックができます。|[amazon](https://www.amazon.co.jp/dp/B09S6Y9RM6/)|

※参考商品は全てアフィリエイトの含まれない直リンクです

※参考商品はあくまで参考であり、全ての商品が検証済みではないことにご注意ください



　
## PCBの組み立て
### PCBの分離
- ニッパー等で赤丸で囲ったライナー部分をカットします。（素手でも折れると思います
