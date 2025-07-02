# 😎 Awesome-Online-Prediction [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome online-prediction papers, tools, and resources.

Created and hosted by the members of group 5 in The 28th **M**eeting on **I**mage **R**ecognition and **U**nderstanding ([MIRU2025](https://cvim.ipsj.or.jp/MIRU2025/index-en.html)) Wakate program.

[画像の認識・理解シンポジウム（MIRU2025）](https://cvim.ipsj.or.jp/MIRU2025/index.html)で企画された [若手プログラム](https://sites.google.com/view/miru2025wakate) における，グループ５による取り組みの成果です．

オンライン予測に関する重要な論文，ライブラリ，学習のためのリソースなどをまとめています．

> [!TIP]
> Super-awesome ones are marked with a star🌟.
> 
> Japanese-only references are marked with Japan🗾.
> 
> 特に重要・有用なものには星印🌟を付しています．
> 
> 日本語のみの文献には日本🗾を付しています．

ノルマ50本：
![](https://geps.dev/progress/40)

# 📑 Papers（論文）
## Awesome-Surveys（サーベイ）
### 1. 🌟[Hoi _et al._(2018), Online Learning: A Comprehensive Survey](https://arxiv.org/abs/1802.02871)
  - Published in 2018, this survey has been cited over 1,000 times and broadly covers online learning and online prediction topics.
  - 2018年の発表だが，1000回以上引用されているサーベイ．オンライン学習やオンライン予測の内容を広く取り上げている．
    
### 2. [Švihrová _et al._ (2025), *Designing digital health interventions with causal inference and multi-armed bandits: a review*](https://www.frontiersin.org/journals/digital-health/articles/10.3389/fdgth.2025.1435917/full)
  - ヘルスケア分野における Just-In-Time Interventiobn に多腕バンディット問題と因果解析を導入する方法論に関するレビュー論文。
  - 被験者の健康状態を逐次的にモニタリングし、適切なタイミングで"介入"して行動変容を促す枠組み。

### 3. [Kumar _et al._ (2024), *Using adaptive bandit experiments to increase and investigate engagement in mental health*](https://ojs.aaai.org/index.php/AAAI/article/view/30328)
  - メンタルヘルスにおける個別化医療にバンディット問題を適用することを目指したシミュレーション論文．

### 4. [Gutiérrez _et al._ (2017), *A Multi-armed Bandit to Smartly Select a Training Set from Big Medical Data*](https://link.springer.com/chapter/10.1007/978-3-319-66179-7_5)
  - 大規模な医療画像データから訓練データセットを適切かつ効率的に選択する問題を多腕バンディット問題として定式化した。
  - 脳画像から得られる特徴量から年齢を予測する問題において、事前に観測できるメタデータから有用なサンプルを選択するという問題に落とし込んだ。
  - データをクラスタリングし、有益そうなクラスタを活用しつつ、他のクラスタも探索していく、というアプローチをとった。
  - 手法は線形回帰ベースで深層学習ではない

### 5. [Zheng and Kwok (2017), *Follow the Moving Leader in Deep Learning*](https://proceedings.mlr.press/v70/zheng17a.html)
  - **谷口調査中**

### 6. [Dai _et al._ (2025), Label Shift Meets Online Learning: Ensuring Consistent Adaptation with Universal Dynamic Regret](https://proceedings.neurips.cc/paper_files/paper/2023/hash/cf42f133f355e0e07a8957b508b26a1b-Abstract-Conference.html)
  - **谷口調査中**

================================

# 🧰 Tools（ツール）
## Awesome-Libraries（ライブラリ）
### 7. 🌟[River](https://github.com/online-ml/river)
  - a Python library for online machine learning (with over 5k stars), covering time series forecasting, bandits, and so on.
  - オンライン機械学習のためのPythonライブラリ（5000スター超え）で、時系列予測やバンディットなどをカバーしている。
### 8. [scikit-multiflow](https://scikit-multiflow.readthedocs.io/en/stable/index.html)
  - a machine learning library for streaming data in Python (~0.8k stars). Although it can handle drift detection and has a variety of algorithms other than neural networks, River is more common nowadays.
  - ストリーミングデータに適したPython実装の機械学習ライブラリ（約800スター）．ドリフト検出機能を備え，ニューラルネットワーク以外のアルゴリズムも豊富だが，現在ではRiverに主流が移った．
### 9. 🌟[Vowpal Wabbit](https://vowpalwabbit.org/index.html)
  - a machine learning library implemented in various languages (with over 8,500 stars) primarily developed by Microsoft. It supports various learning paradigms, including online learning, and can handle online prediction-related stuff like contextual bandits."
  - Microsoftが中心となって開発している多言語実装の機械学習ライブラリ（8500スター超え）．オンライン学習を含む多様な学習様式に対応しており，Contextual bandits等を扱える．


# 📚 Resources（学習リソース）
## Awesome-slides（スライド）
### 10.🗾[オンライン予測の理論と応用](https://www.lab2.kuis.kyoto-u.ac.jp/keisan-genkai/reports/2005/zentai_1/04-takimoto.pdf)
  - 機械学習プロフェッショナルシリーズ「オンライン予測」（後述）の著者でもある瀧本英二先生によるスライド．オンライン予測におけるエキスパート統合問題とその応用例を取り上げている．

## Awesome-Textbooks（書籍）
### 11. 🌟🗾[機械学習プロフェッショナルシリーズ 「オンライン予測」](https://www.kspub.co.jp/book/detail/1529229.html)
  - 著名な機械学習プロフェッショナルシリーズより，オンライン予測にフォーカスして書かれた一冊．エキスパート統合問題やオンライン凸最適化など，オンライン予測の主要な内容を一通り学べる．
### 12. 🗾[機械学習プロフェッショナルシリーズ 「オンライン機械学習」](https://www.kspub.co.jp/book/detail/1529038.html)
  - 同じく機械学習プロフェッショナルシリーズより，オンライン機械学習を取り上げた一冊（出版は「オンライン予測」よりも前）．オンライン予測を含む，より広範な内容を学べる．
### 13. 🗾[機械学習プロフェッショナルシリーズ 「バンディット問題の理論とアルゴリズム」](https://www.kspub.co.jp/book/detail/1529175.html)
  - 同じく機械学習プロフェッショナルシリーズより．バンディット問題におけるリグレット解析や応用例などをより専門的に扱っている．

## Videos（動画）
### 14. [Predict with online prediction in Vertex AI](https://youtu.be/TEE7uUbXWDY?si=nHXMfZyTb13KpmWD)
  - Awesome tutorial on how to make predictions on tabular datasets with online prediction in Vertex AI. [GitHub Link](https://github.com/rafaello9472/c4ds/tree/main/Predict%20with%20online%20prediction%20in%20Vertex%20AI)
  - GoogleのVertex AIを用いて表形式のデータに対してオンライン予測を行う方法についてのチュートリアル．[GitHub Link](https://github.com/rafaello9472/c4ds/tree/main/Predict%20with%20online%20prediction%20in%20Vertex%20AI)
### 15. ["Online" prediction vs "batch" prediction in machine learning](https://youtu.be/DnmWTIeQ7PM?si=Mg8xcbWXyzlP3vLY)
  - Awesome explanation by Chip Huyen on the difference between online prediction and more common batch prediction and their applications.
  - Chip Huyenによる，オンライン予測と馴染み深いバッチ予測との違いやそれらの応用例についての短い解説．
### 16. [ML Drift: Identifying Issues Before You Have a Problem](https://youtu.be/uOG685WFO00?si=7_ti70FDTD-B5tbO)
  - Awesome presentation by Amy Hodler on ML drifts and how to fix it. [Blog](https://www.fiddler.ai/blog/drift-in-machine-learning-how-to-identify-issues-before-you-have-a-problem)
  - Amy Hodlerによる，MLドリフトやその解決方法についてのプレゼンテーション．[ブログ](https://www.fiddler.ai/blog/drift-in-machine-learning-how-to-identify-issues-before-you-have-a-problem)

## Articles（記事）
### 17. 🗾[私のブックマーク「オンライン学習」](https://www.ai-gakkai.or.jp/resource/my-bookmark/my-bookmark_vol30-no5/)
  - 人工知能学会誌の連載「私のブックマーク」でオンライン学習を特集した際の記事．オンライン学習に関するサーベイやチュートリアル，関連学会，関連ライブラリをまとめている．
### 18. 🗾[私のブックマーク「多腕バンディット問題」](https://www.ai-gakkai.or.jp/resource/my-bookmark/my-bookmark_vol31-no5/)
  - 同じく「私のブックマーク」より，多腕バンディット問題を特集した回の記事．逐次的な意思決定であるバンディット問題に関するチュートリアルや関連学会，関連ライブラリ，重要論文をまとめている．
### 19. [Deus Ex Machina「Online learning and online prediction（オンライン学習とオンライン予測について）」](https://deus-ex-machina-ism.com/?p=17082)
  - Good for understanding the confusing differences between online learning and online prediction, and for gaining an overview of their respective scopes.
  - 混同しやすいオンライン学習とオンライン予測の違いを知り，それぞれの範囲を概観するのに良い．
### 20. [Deus Ex Machina「Overview of online forecasting technology and various applications and implementations（オンライン予測技術の概要と様々な適用事例と実装例）」](https://deus-ex-machina-ism.com/?p=53594)
  - It introduces algorithms, libraries, applications, and suitable books for learning used in online prediction.
  - オンライン予測で使用されるアルゴリズム，ライブラリ，応用例，学習に適した書籍が紹介されている．
