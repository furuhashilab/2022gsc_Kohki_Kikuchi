# 2022gsc_Kohki_Kikuchi
菊池洸希の2022年度ゼミ論用レポジトリ
# 【2022年度ゼミ論】「Mapbox GL JS」Style Specificationの日本語訳作成と図式化
地球社会共生学部　地球社会共生学科　4年A組89番  

学籍番号：1A119059  　氏名：菊池洸希 

指導教員：古橋 大地教授   

©︎Furuhashi Laboratory/Kikuchi Kohki, CC BY 4.0

## 概要  
本研究では、「Mapbox GL JS Style Specification - Layers」の日本語訳を作成し、その概要を図式化した。

## Introduction
　1970年代、四分木（Quadtree)というデータ構造が生まれてから今日に至るまでデジタルマップは進化を続けてきた。2000年代にはタイル技術が生まれ、2005年にGoogleがラスターピラミッドの機能を持ったラスタータイルマップの完成版であるGoogleマップをリリースした。2006年、ブラウザで地図データを表示するためのJavaScriptライブラリであるOpenLayersがリリース。ライブラリを非公開にしているGoogleマップに対して、OpenLayersはオープンソースであった。さらに2011年には、これらに並んで広く使われているLeafletがVladimir Agafonkin氏によって開発される。Vladimir Agafonkin氏が2013年にMapboxに加入すると、翌年にベクタータイルマップに対応したオープンソースライブラリである「Mapbox GL JS」をリリースした。これは2020年に行われたv2.0への移行によって独自ライセンス化するが、この件に批判的なユーザー達が同年、MapboxGLエコシステムのフォークであるMapLibreを開始した。こうしてデジタル地図は進化を続け、現在では非常に速く、軽量で、自由な地図開発が可能になっている。しかし、地図開発において重要なドキュメントの多くは日本語対応していないのが現状である。今後、日本でより多くの人が地図開発を行えるようにこれらのドキュメントを日本語に翻訳していく必要がある。また、地図開発の学習を始める上で、ドキュメントの構造が図式化されているとより理解が深まるが、まだドキュメントの図式化は進んでいない。本研究では、国土地理院が開発している「地理院地図Vector（仮称）」にも採用されている「Mapbox GL JS」のStyle Specificationで特に重要な項目であるLayersの日本語訳を作成し、その概要を図式化した。

## Methods　　
本研究で行うことは以下の2つである。
  
### ①「Mapbox GL JS Style Specification - Layers」の日本語訳の作成

Githubレポジトリ[「StyleSpecification4mapbox」](https://github.com/furuhashilab/StyleSpecification4mapbox)内に、「Mapbox GL JS Style Specification[^1] - Layers」の日本語訳をMarkdown形式で作成する。留意点は以下の通り。
[^1]:Mapox. “Mapbox GL JS Style Specification”. Mapbox Docs. 2022-1-6. https://docs.mapbox.com/mapbox-gl-js/style-spec/, (参照 2022-2-3).

- 作業効率化のため、基本的にGoogle Chromeのページ翻訳ツールを利用する。翻訳結果に異常があった場合は、Google翻訳を使って正しい日本語訳を作成する。

<img width="70%" alt="mb_ss_j_miss" src="https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi/blob/8989977e2c36a2d8ec6dcf70e5694c099ea5abe4/mb_ss_j_miss.png">

<img width="70%" alt="gt_01" src="https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi/blob/8989977e2c36a2d8ec6dcf70e5694c099ea5abe4/gt_01.png">

- 各タイトルやワードには原文と同様のリンクを付け、Mapboxのページに移動できるようにする。

<img width="70%" alt="mb_ss_j_link" src="https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi/blob/8989977e2c36a2d8ec6dcf70e5694c099ea5abe4/mb_ss_j_link.png">

- 列挙型で用いられる"visible"や"none"のようなワード、ブルー値で用いられる"true"と"false"、文字列の配列で用いられる"visible"や "none"等のワードは開発の際にそのまま使用することを考慮し、原文の通りに記載する。

<img width="70%" alt="mb_ss_j_word" src="https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi/blob/8989977e2c36a2d8ec6dcf70e5694c099ea5abe4/mb_ss_j_word.png">

### ②「Mapbox GL JS Style Specification - Layers」の図式化

「UML 2 クラス図の概要[^2]」を参照し、UMLクラス図の形式に則り、「Mapbox GL JS Style Specification - Layers」の図式化を行う。図の作成にはCanva(グラフィックデザインプラットフォーム)を利用する。正式な形式に近づけるため、図は英語表記にする。図はレイヤー構造が視覚的に把握できるよう、配置と配色を構造ごとに変更する。また、オプション機能にはアイコンを付け、図をシンプルに表現する。
[^2]:Scott W. Ambler. “UML 2 クラス図の概要”. アジャイルモデリング(AM) 公式サイト. 2003. https://www.ogis-ri.co.jp/otc/swec/process/am-res/am/artifacts/classDiagram.html#DesignClassDiagrams, (参照 2022-2-3).

<img width="70%" alt="canva_01" src="https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi/blob/54ceacd0a529b718793b724247176fbedc7839a0/canva_01.png">

## Results　　

Githubレポジトリ　[StyleSpecification4mapbox/Layers](https://github.com/furuhashilab/StyleSpecification4mapbox/blob/fd5ef5c7cfc9304c7b704431d6ab746eb0ad68a5/Layers.md)

<img alt="qr_StyleSpecification4mapbox:Layers" src="https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi/blob/9d1cab7154cf27f8b7dba5427592b587fa7a98a4/qr_StyleSpecification4mapbox:Layers.png">

UMLクラス図

<img width="80%" alt="uml_layers_01" src="https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi/blob/9d1cab7154cf27f8b7dba5427592b587fa7a98a4/uml_layers_01.png">

## Discussion

### 日本語訳について

**①翻訳できないワードはどう表記すべきか**

<img width="70%" alt="gh_ss_j_antialiased" src="https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi/blob/9d1cab7154cf27f8b7dba5427592b587fa7a98a4/gh_ss_j_antialiased.png">

上記の画像のように、"antialiased"等のワードは翻訳することができない。こういったワードはカタカナ表記、原文通りの表記のどちらにすべきか。

**②開発時に直接書き込むワードとそうでないものの差別化ができていない。**

<img width="70%" alt="gh_ss_j_icon-translate" src="https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi/blob/2d3f8cc93e38bf8541b1aefc351dc853763d723e/gh_ss_j_icon-translate.png">

上記の画像のように、"map"等の開発時に直接書き込むワードにはクォーテーションマーク（日本語には鉤括弧）を付けているが原本と表現が異なる。より理解しやすくするために、原本に近い表現に統一すべきである。

**③翻訳するワードと原文の通りに記載するワードとの線引きが不明瞭であった。**

<img width="70%" alt="gh_ss_j_word" src="https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi/blob/944525522d31315ab5996b39b70a42ee9ee0ce79/gh_ss_j_word.png">

上記の画像のように、「丸」と"round"は同じワードであるが、説明のため上部には「丸」、開発時を意識して下部には"round"と記載した。しかしこの状態では「丸」と"round"が同じワードであると表現できていないため誤解を招く恐れがある。

**④参照URLが多く、MDファイルの中身がまとまっていない**

<img width="70%" alt="gh_ss_j_code" src="https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi/blob/f14a15e55c123b89952311a11d18f08123182196/gh_ss_j_code.png">

上記画像はMDファイルの中身であるが、同じURLが何度も出てきている。このような状態では、アップデートがあった際に簡単に修正することができない。

**解決策**

<img width="70%" alt="mb_ss_j_word" src="https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi/blob/ed5c4a94505d4d92a8ea06adf86b1b9a33ca3b21/React_home.png">

以上に挙げた課題に対し、React Docs[^3]を先行研究として比較対象にし、解決策を提示する。Reactはユーザインタフェース構築のためのJavaScriptライブラリであり、日本語版のドキュメントが用意されている。一部、「Mapbox GL JS Style Specification - Layers」と似ている点もあるため参考にした。
[^3]:React. “Docs”. React. 2020-10-5. https://ja.reactjs.org/docs/getting-started.html, (参照 2022-2-3).

<img width="70%" alt="mb_ss_j_word" src="https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi/blob/ed5c4a94505d4d92a8ea06adf86b1b9a33ca3b21/React_props.png">

課題①に関して、Reactドキュメント内では「コンポーネントコンポジション」と"props"という2つのワードに対し、異なる表記がされている。"props"とは、Reactの機能の1つである。つまり、固有名詞は原文のまま記載するというルールになっていると考えられる。

<img width="70%" alt="mb_ss_j_word" src="https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi/blob/ed5c4a94505d4d92a8ea06adf86b1b9a33ca3b21/React_code.png">

課題②について、Reactドキュメントでも開発時に直接書き込むワードには日本語版でも分かりやすい工夫がされている。「Markdown記法 サンプル集[^4]」に以下の解説があった。
[^4]:@tbpgr. “Markdown記法 サンプル集”. Qiita. 2020-3-27. http://qiita.com/tbpgr/items/989c6badefff69377da7, (参照 2022-2-3).

> バッククォートで文字列を囲むことでコードの一部を表示可能です。
> 
> 記述例   
> インストールコマンドは`gem install hoge`です

よって原本に近づけるため、開発時に直接書き込むワードについてはバッククォートを用いる表現に統一することが望ましい。

課題③については、課題①、②に対する解決策で提示したルールを適応し統一することが適切であると考える。つまり翻訳できないワードについては、固有名詞と開発時に直接書き込むワードは原文の通りに記載し、そうでない場合はカタカナ表記にする。また、同じワードに対し異なる表記を用いることはすべきではない。

課題④について、「Markdown記法 サンプル集[^4]」に適切な解決策を発見した。

> Markdownの文書の途中に長いリンクを記述したくない場合は、同じリンクの参照を何度も利用する場合は、リンク先への参照を定義することができます。
> 
> ```
> [こっちからgoogle][google]  
> その他の文章  
> [こっちからもgoogle][google]  
> 
> [google]: https://www.google.co.jp/
> ```

MD形式での日本語訳作成においては、定義参照リンクを活用することを統一すべきである。

### 図式化について

「Mapbox GL JS Style Specification - Layers」は最も記述の多いドキュメントであり、その多くがタイプの詳細な設定についてである。本研究ではこれらを全て図にまとめるのは情報過多であるとの判断で、タイプ１０種類のみを掲載している。UMLクラス図の継承階層の概念を用いて、レイヤー構造を視覚的に表現するために、それらがどこの項目に属するのかを矢印で示した。本来、UML図では色を使うことはないが、本研究は「Mapbox GL JS Style Specification - Layers」の理解を補助することが目的であるため、階層ごとに色分けをした。本研究の目的に合わせた図を作成することはできたが、「Mapbox GL JS」を用いたウェブ地図の構造はSourcesやRoot等の概念も含めた複雑なものである。それらを含めた全体の構造を表現することを考慮すると、コンポジション表現なども活用すべきである。

## Conclusion　　　

今後の課題としては、以下の３つが挙げられる。　　    
- 「Mapbox GL JS Style Specification - Layers」日本語版の翻訳ルール統一  
- 「Mapbox GL JS Style Specification」全項目の日本語訳作成
- 「Mapbox GL JS Style Specification」各項目および全体の図式化

デジタル地図に関するドキュメントの日本語訳はまだ少ないが、今後日本国内で独自の地図開発が広がると、ドキュメントの日本語訳の需要は高まる。しかし各ドキュメントが独自の翻訳ルールで作成していてはユーザーにとっては理解し難くなる。本研究をさらに進めることでそうしたユーザーのサポートができる。さらにオープンソース等が図式化されていくことでユーザーの理解が深まり、より発展的な活用が期待できる。

## Acknowledgements
本研究を進めるにあたり地球社会共生学部の古橋大地教授をはじめ多くの方々より多大な助言を賜りました。厚く感謝を申し上げます。

## グラレコ

<img width="70%" alt="zemiron_01" src="https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi/blob/main/zemiron_01.png">

## 資料
**進捗管理用プロジェクト**  
https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi/projects/3  
**最終プレゼン資料**  
https://docs.google.com/presentation/d/13QyPYV9XP0rMW9lBEhvvMw2V1saTevBbOVW-3ukvOms/edit?usp=sharing    
**参考文献リスト**   
https://docs.google.com/spreadsheets/d/1XJQ7ZuN18UEj8fmp4vFUclrJZ3TLgDixdDmo9DB-RRg/edit#gid=0　  
**「Mapbox GL JS Style Specification」日本語版　Githubレポジトリ**  
https://github.com/furuhashilab/StyleSpecification4mapbox/blob/ed5cd80c0f0872f9057f81ea1e251339c9d272d4/Layers.md  
**Medium**  
https://medium.com/furuhashilab/2021%E5%B9%B4%E5%BA%A6%E3%82%BC%E3%83%9F%E8%AB%96-mapbox-gl-js-style-specification%E3%81%AE%E6%97%A5%E6%9C%AC%E8%AA%9E%E8%A8%B3%E4%BD%9C%E6%88%90%E3%81%A8%E5%9B%B3%E5%BC%8F%E5%8C%96-5ad5afb1557d
