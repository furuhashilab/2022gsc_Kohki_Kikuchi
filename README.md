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

## Discussion

## Conclusion　　　

## Acknowledgements
本研究を進めるにあたり地球社会共生学部の古橋大地教授をはじめ多くの方々より多大な助言を賜りました。厚く感謝を申し上げます。

## グラレコ

## 昨年度資料
**Githubレポジトリ**  
https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi  
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
