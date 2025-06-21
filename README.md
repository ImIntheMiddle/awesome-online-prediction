# 😎 Awesome-Online-Prediction [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome online-prediction papers, tools, and resources.

Created and hosted by the members of group 5 in The 28th **M**eeting on **I**mage **R**ecognition and **U**nderstanding ([MIRU2025](https://cvim.ipsj.or.jp/MIRU2025/index-en.html)) Wakate program.

[画像の認識・理解シンポジウム（MIRU2025）](https://cvim.ipsj.or.jp/MIRU2025/index.html)で企画された [若手プログラム](https://sites.google.com/view/miru2025wakate) における，グループ５による取り組みの成果です．

オンライン予測に関する重要な論文，ライブラリ，学習のためのリソースなどをまとめています．

> [!TIP]
> Super-awesome ones are marked with a star🌟.
> 
> 特に重要なものには星印🌟を付しています．

目標100本：
![](https://geps.dev/progress/10)

# 📑 Papers（論文）
## Awesome-Surveys（サーベイ）
### 1. 🌟[Online Learning: A Comprehensive Survey](https://arxiv.org/abs/1802.02871)
  - Published in 2018, this survey has been cited over 1,000 times and broadly covers online learning and online prediction topics.
  - 2018年の発表だが，1000回以上引用されているサーベイ．オンライン学習やオンライン予測の内容を広く取り上げている．

# 🧰 Tools（ツール）
## Awesome-Libraries（ライブラリ）
### 2. 🌟[River](https://github.com/online-ml/river)
  - a Python library for online machine learning (with over 5k stars), covering time series forecasting, bandits, and so on.
  - オンライン機械学習のためのPythonライブラリ（5000スター超え）で、時系列予測やバンディットなどをカバーしている。
### 3. [scikit-multiflow](https://scikit-multiflow.readthedocs.io/en/stable/index.html)
  - a machine learning library for streaming data in Python (~0.8k stars). Although it can handle drift detection and has a variety of algorithms other than neural networks, River is more common nowadays.
  - ストリーミングデータに適したPython実装の機械学習ライブラリ（約800スター）．ドリフト検出機能を備え，ニューラルネットワーク以外のアルゴリズムも豊富だが，現在ではRiverに主流が移った．
### 4. 🌟[Vowpal Wabbit](https://vowpalwabbit.org/index.html)
  - a machine learning library implemented in various languages (with over 8,500 stars) primarily developed by Microsoft. It supports various learning paradigms, including online learning, and can handle online prediction-related stuff like contextual bandits."
  - Microsoftが中心となって開発している多言語実装の機械学習ライブラリ（8500スター超え）．オンライン学習を含む多様な学習様式に対応しており，Contextual bandits等を扱える．


# 📚 Resources（学習リソース）
## Awesome-Textbooks（書籍）

## Awesome-Japanese-Textbooks（日本語書籍）
### 5. 🌟[機械学習プロフェッショナルシリーズ 「オンライン予測」](https://www.kspub.co.jp/book/detail/1529229.html)
  - 著名な機械学習プロフェッショナルシリーズより，オンライン予測にフォーカスして書かれた一冊．エキスパート統合問題やオンライン凸最適化など，オンライン予測の主要な内容を一通り学べる．

## Videos（動画）
### 6. [Predict with online prediction in Vertex AI](https://youtu.be/TEE7uUbXWDY?si=nHXMfZyTb13KpmWD)
  - Awesome tutorial on how to make predictions on tabular dataset with online prediction in Vertex AI. [GitHub Link](https://github.com/rafaello9472/c4ds/tree/main/Predict%20with%20online%20prediction%20in%20Vertex%20AI)
  - GoogleのVertex AIを用いて表形式のデータに対してオンライン予測を行う方法についてのチュートリアル．[GitHub Link](https://github.com/rafaello9472/c4ds/tree/main/Predict%20with%20online%20prediction%20in%20Vertex%20AI)
### 7. ["Online" prediction vs "batch" prediction in machine learning](https://youtu.be/DnmWTIeQ7PM?si=Mg8xcbWXyzlP3vLY)
  - Awesome explanation by Chip Huyen on the difference between online prediction and more common batch prediction and their applications.
  - Chip Huyenによる，オンライン予測と馴染み深いバッチ予測との違いやそれらの応用例についての短い解説．
### 8. [ML Drift: Identifying Issues Before You Have a Problem](https://youtu.be/uOG685WFO00?si=7_ti70FDTD-B5tbO)
  - Awesome presentation by Amy Hodler on ML drifts and how to fix it. [Blog](https://www.fiddler.ai/blog/drift-in-machine-learning-how-to-identify-issues-before-you-have-a-problem)
  - Amy Hodlerによる，MLドリフトやその解決方法についてのプレゼンテーション．[ブログ](https://www.fiddler.ai/blog/drift-in-machine-learning-how-to-identify-issues-before-you-have-a-problem)

## Articles（記事）
### 9. [Deus Ex Machina「Online learning and online prediction（オンライン学習とオンライン予測について）」](https://deus-ex-machina-ism.com/?p=17082)
  - Good for understanding the confusing differences between online learning and online prediction, and for gaining an overview of their respective scopes.
  - 混同しやすいオンライン学習とオンライン予測の違いを知り，それぞれの範囲を概観するのに良い．
### 10. [Deus Ex Machina「Overview of online forecasting technology and various applications and implementations（オンライン予測技術の概要と様々な適用事例と実装例）」](https://deus-ex-machina-ism.com/?p=53594)
  - It introduces algorithms, libraries, applications, and suitable books for learning used in online prediction.
  - オンライン予測で使用されるアルゴリズム，ライブラリ，応用例，学習に適した書籍が紹介されている．
