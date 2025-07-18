# 😎 Awesome-Online-Prediction [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome online-prediction papers, tools, and resources.

Created and hosted by the members of group 5 in the 28th **M**eeting on **I**mage **R**ecognition and **U**nderstanding ([MIRU2025](https://cvim.ipsj.or.jp/MIRU2025/index-en.html)) Wakate program.

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

ノルマ100本：
![](https://geps.dev/progress/63)

# 📑 Papers（論文）
## Awesome-Surveys（サーベイ）
### 1. 🌟[Hoi _et al._(2018), Online Learning: A Comprehensive Survey](https://arxiv.org/abs/1802.02871)
  - Published in 2018, this survey has been cited over 1,000 times and broadly covers online learning and online prediction topics.
  - 2018年の発表だが，1000回以上引用されているサーベイ．オンライン学習やオンライン予測の内容を広く取り上げている．
### 2. 🌟[Foster and Rakhlin (2023), Foundations of Reinforcement Learning and Interactive Decision Making](https://arxiv.org/abs/2312.16730)
  - This lecture note introduces various decision-making problems, including online learning and prediction, and explains the theoretical foundations of online reinforcement learning.
  - オンライン学習・予測を含めた各種の意思決定問題について紹介し，オンライン強化学習の理論的基礎までを解説した講義ノート．
### 3. [Online Learning and Online Convex Optimization](https://www.cs.huji.ac.il/~shais/papers/OLsurvey.pdf)
  - a
  - a
### 4. [Orabona (2019), A Modern Introduction to Online Learning](https://arxiv.org/abs/1912.13213)
  - a
  - a

## Awesome-Theoretical Research（基礎研究）
### 5. [Suehiro _et al._(ALT2012), Online Prediction under Submodular Constraints](https://api.lib.kyushu-u.ac.jp/opac_download_md/1932327/alt12.pdf)
  - a
  - a
### 6. [Dai _et al._(CVPR2025), Label Shift Meets Online Learning: Ensuring Consistent Adaptation with Universal Dynamic Regret](https://openaccess.thecvf.com/content/CVPR2025/html/Dai_Label_Shift_Meets_Online_Learning_Ensuring_Consistent_Adaptation_with_Universal_CVPR_2025_paper.html)
  - a
  - a

## Awesome-Applied Research（応用研究）
### 7. [Song _et al._ (Machine Learning, 2024), No Regret Sample Selection with Noisy Labels](https://arxiv.org/abs/2003.03179)
  - a
  - a
### 8. [Song _et al._ (WACV2020), Adaptive Aggregation of Arbitrary Online Trackers with a Regret Bound](https://openaccess.thecvf.com/content_WACV_2020/papers/Song_Adaptive_Aggregation_of_Arbitrary_Online_Trackers_with_a_Regret_Bound_WACV_2020_paper.pdf)
  - a
  - a
### 9. [Matsuo _et al._(ICASSP2023), Learning from Label Proportion with Online Pseudo-Label Decision by Regret Minimization](https://arxiv.org/abs/2302.08947)
  - a
  - a
### 10. [Švihrová _et al._ (2025), *Designing digital health interventions with causal inference and multi-armed bandits: a review*](https://www.frontiersin.org/journals/digital-health/articles/10.3389/fdgth.2025.1435917/full)
  - ヘルスケア分野における Just-In-Time Interventiobn に多腕バンディット問題と因果解析を導入する方法論に関するレビュー論文。
  - 被験者の健康状態を逐次的にモニタリングし、適切なタイミングで"介入"して行動変容を促す枠組み。

### 11. [Kumar _et al._ (2024), *Using adaptive bandit experiments to increase and investigate engagement in mental health*](https://ojs.aaai.org/index.php/AAAI/article/view/30328)
  - メンタルヘルスにおける個別化医療にバンディット問題を適用することを目指したシミュレーション論文．

### 12. [Gutiérrez _et al._ (2017), *A Multi-armed Bandit to Smartly Select a Training Set from Big Medical Data*](https://link.springer.com/chapter/10.1007/978-3-319-66179-7_5)
  - 大規模な医療画像データから訓練データセットを適切かつ効率的に選択する問題を多腕バンディット問題として定式化した。
  - 脳画像から得られる特徴量から年齢を予測する問題において、事前に観測できるメタデータから有用なサンプルを選択するという問題に落とし込んだ。
  - データをクラスタリングし、有益そうなクラスタを活用しつつ、他のクラスタも探索していく、というアプローチをとった。
  - 手法は線形回帰ベースで深層学習ではない

### 13. [Zheng and Kwok (2017), *Follow the Moving Leader in Deep Learning*](https://proceedings.mlr.press/v70/zheng17a.html)
  - **谷口調査中**

================================

# 🧰 Tools（ツール）
## Awesome-Libraries（ライブラリ）
### 51. 🌟[River](https://github.com/online-ml/river)
  - A Python library for online machine learning (with over 5k stars), covering time series forecasting, bandits, and so on.
  - オンライン機械学習のためのPythonライブラリ（5000スター超え）で、時系列予測やバンディットなどをカバーしている。
### 52. [scikit-multiflow](https://scikit-multiflow.readthedocs.io/en/stable/index.html)
  - A machine learning library for streaming data in Python (~0.8k stars). Although it can handle drift detection and has a variety of algorithms other than neural networks, River is more common nowadays.
  - ストリーミングデータに適したPython実装の機械学習ライブラリ（約800スター）．ドリフト検出機能を備え，ニューラルネットワーク以外のアルゴリズムも豊富だが，現在ではRiverに主流が移った．
### 53. 🌟[Vowpal Wabbit](https://vowpalwabbit.org/index.html)
  - A machine learning library implemented in various languages (with over 8,500 stars), primarily developed by Microsoft. It supports various learning paradigms, including online learning, and can handle online prediction-related stuff like contextual bandits."
  - Microsoftが中心となって開発している多言語実装の機械学習ライブラリ（8500スター超え）．オンライン学習を含む多様な学習様式に対応しており，Contextual bandits等を扱える．
### 54. 🌟[MOA](https://moa.cms.waikato.ac.nz/)
  - An open-source Java framework designed for sequential data processing, boasting over 600 stars.
  - JAVAで実装された，逐次データ処理用のオープンソースフレームワーク．600スター超え． 
### 55. [CapyMOA](https://capymoa.org/)
  - Python implementation of MOA, significantly faster than River and suited for real-time processing.
  - MOAのPython版．Riverよりも大幅に高速化されており，リアルタイム処理向き．
### 56. [Jubatas](http://jubat.us/ja/index.html)
  - A distributed processing framework for online machine learning, jointly developed by PFN and NTT.
  - PFNとNTTが共同で開発していたオンライン機械学習向けの分散処理フレームワーク．
### 57. [Deep-River](https://online-ml.github.io/deep-river/)
  - A library suitable for online learning of deep learning models implemented in PyTorch. Same developers as River (online-ml)."
  - PyTorchで実装された深層学習モデルのオンライン学習に適したライブラリ．Riverと同じonline-mlが開発．

## Awesome-Probability Inequalities (確率不等式)
### 58. [Probability inequalities](https://probability.oer.math.uconn.edu/wp-content/uploads/sites/2187/2020/08/ch15M.pdf)
  - Introduction of several probability inequalities used in proofs.
  - 証明に使用される確率不等式がいくつか紹介されている．
### 59. 🌟[Markov's Inequality ... Made Easy!](https://www.youtube.com/watch?v=e-nAr3MkAII)
  - Awesome YouTube video on Markov's inequality.
  - マルコフの不等式について解説したYouTube動画．
### 60. 🌟[Chebyshev's Inequality ... Made Easy!](https://www.youtube.com/watch?v=mlelI1LA9o4)
  - Awesome YouTube video on Chebyshev's inequality.
  - チェビシェフの不等式について解説したYouTube動画．
### 61. 🗾[【大学数学】チェビシェフの不等式【確率統計】](https://www.youtube.com/watch?v=d-ugoDdXWrU)
  - ヨビノリによるチェビシェフの不等式についての解説動画．
### 62. [What is the Chernoff Bound?](https://www.youtube.com/watch?v=WKUeBoQp2Uo)
  - Awesome YouTube video on Chernoff bound.
  - チェルノフ限界について解説したYouTube動画．
### 63. [L 27 | Cauchy Schwarz Inequality | Probability & Statistics | Digital Communication](https://www.youtube.com/watch?v=14-JD5KiUz0)
  - Awesome YouTube video on Cauchy-Schwarz inequality.
  - コーシー＝シュワルツの不等式について解説したYouTube動画．
  - チェルノフ限界について解説したYouTube動画．
### 64. [Jensen's Inequality](https://www.youtube.com/watch?v=u0_X2hX6DWE)
  - Awesome YouTube video on Jensen's inequality.
  - イェンセンの不等式について解説したYouTube動画．
### 65. [A Visual Introduction to Hoeffding's Inequality - Statistical Learning Theory](https://www.youtube.com/watch?v=lsYPC0MuLJA)
  - Awesome YouTube video visualizing the concept of Hoeffding's inequality.
  - へフディングの不等式について視覚的に解説したYouTube動画．
### 66. [Supplemental Lecture notes Hoeffding’s inequality](https://cs229.stanford.edu/extra-notes/hoeffding.pdf)
  - Lecture material of Stanford University, including an explanation of moment generating functions and a proof of Hoeffding's inequality.
  - モーメント母関数の解説やHoeffdingの不等式の証明を含んだ，スタンフォード大学の講義資料．
### 67. 🗾[ヘフディングの不等式(Hoeffding's inequality)と諸々の確率の評価の不等式](https://ludu-vorton.hatenablog.com/entry/2019/06/06/073000)
  - 統計的学習理論で確率の評価で用いられる様々な不等式（へフディングの不等式を含む）についての解説．

## Awesome-Convex Optimization (凸最適化)
### 68. [Subgradients/Subderivatives - Convex Analysis](https://www.youtube.com/watch?v=o0rOaN5uo64)
  - Awesome YouTube video on subgradients and subderivatives.
  - 劣勾配/劣微分について解説したYouTube動画．
### 69. [Lipschitz Continuity | Lipschitz Condition](https://www.youtube.com/watch?v=P-OFTp3BPis) 
  - Awesome YouTube video on Lipschitz continuity.
  - リプシッツ連続について解説したYouTube動画．
### 70. 🗾[リプシッツ連続とは～定義と性質・他の連続性との関係など～](https://mathlandscape.com/lipschitz/)
  - リプシッツ連続の定義や例，性質，その他の連続性との関連性について解説した記事．
### 71. [Lagrange Multipliers](https://www.youtube.com/watch?v=5-CUqogfPLY)
  - Awesome YouTube video on Lagrange multipliers.
  - ラグランジュの未定乗数法について解説したYouTube動画．
### 72. [Understanding Lagrange Multipliers Visually](https://www.youtube.com/watch?v=5A39Ht9Wcu0)
  - Awesome YouTube video visualizing the concept of Lagrange multipliers.
  - ラグランジュの未定乗数法について視覚的に解説したYouTube動画．
### 73. 🗾[ラグランジュの未定乗数法の気持ち【条件付き極値問題】](https://www.youtube.com/watch?v=vAwqZmwf4W8)
  - ヨビノリによるラグランジュの未定乗数法についての解説動画．図形的意味についての解説を含む．
### 74. 🗾[制約付き最適化問題(KKT条件/ラグランジュ未定乗数法)](https://www.youtube.com/watch?v=bdWTCq98H5c)
  - ヨビノリによるラグランジュの未定乗数法についての解説動画．KKT条件（不等式制約の場合の解法）についての解説を含む．
### 75. 🗾[ラグランジュの未定乗数法とは～意味と証明～](https://mathlandscape.com/lagrange-multiplier/)
  - ラグランジュの未定乗数法の意味，定理とその証明を解説した記事．

## Awesome-Gradient Descent (勾配降下法)
### 76. [Gradient descent, how neural networks learn | Deep Learning Chapter 2](https://youtu.be/IHZwWFHWa-w?si=zRN94_SPD4hrQUUI)
  - Awesome explanation of gradient descent in deep learning by 3Blue1Brown.
  - 3Blue1Brownによる，深層学習における勾配降下法についての解説．
### 77. [Optimization for Deep Learning (Momentum, RMSprop, AdaGrad, Adam)](https://youtu.be/NE88eqLngkg?si=qSmU5hpaeYiUtEZw)
  - Awesome explanation of the various online learning methods used in deep learning.
  - 深層学習に用いられる様々なオンライン学習手法についての解説．
### 78. [Mini Batch Gradient Descent (C2W2L01)](https://www.youtube.com/watch?v=4qJaSmvhxi8)
  - Awesome YouTube video by Andrew Ng explaining mini-batch gradient descent.
  - Andrew Ngによる，ミニバッチ勾配降下法について解説したYouTube動画.
### 79. [Understanding Mini-Batch Gradient Descent (C2W2L02)](https://www.youtube.com/watch?v=-_4Zi8fCZO4)
  - The second YouTube video by Andrew Ng explaining mini-batch gradient descent.
  - Andrew Ngによる，ミニバッチ勾配降下法について解説したYouTube動画の２本目.

# 📚 Resources（学習リソース）
## Awesome-slides（スライド）
### 80. [Online Convex Optimization and Its Surprising Applications](https://groups.oist.jp/sites/default/files/imce/u129210/mlss/Lecture_slide/MLSS2024_Francesco_Orabona.pdf)
  - a
  - a
### 81. [Online Learning Methods for Big Data Analytics](http://www.mysmu.edu.sg/faculty/chhoi/libol/icdm14tuto/index.html)
  - Awesome tutorial presented at IEEE ICDM2014
  - IEEE ICDM2014で発表されたチュートリアル講演．
### 82. [Learning Methods for Online Prediction Problems](https://users.cecs.anu.edu.au/~ssanner/MLSS2010/Bartlett1.pdf)
  - a
  - a
### 83. [Follow the Leader: Theory and Applications](https://www.cs.ubc.ca/labs/lci/mlrg/slides/2019_summer_3_follow_the_leader.pdf)
  - Slides explaining Follow The Leader (FTL) and its derivative algorithms in online learning, along with their applications.
  - オンライン学習におけるFollow The Leader (FTL) やその派生アルゴリズム，そしてそれらの応用について解説したスライド．
### 84. 🗾[多腕バンディット問題の理論とアルゴリズム](https://ibisml.org/archive/ibis2014/ibis2014_bandit.pdf)
  - a
  - a
### 85.🗾[オンライン予測の理論と応用](https://www.lab2.kuis.kyoto-u.ac.jp/keisan-genkai/reports/2005/zentai_1/04-takimoto.pdf)
  - 機械学習プロフェッショナルシリーズ「オンライン予測」（後述）の著者でもある瀧本英二先生によるスライド．オンライン予測におけるエキスパート統合問題とその応用例を取り上げている．

## Awesome-Textbooks（書籍）
### 86. [Prediction, Learning, and Games](https://www.cambridge.org/core/books/prediction-learning-and-games/A05C9F6ABC752FAB8954C885D0065C8F)
  - a
  - a
### 87. [Introduction to Online Convex Optimization](https://sites.google.com/view/intro-oco/)
  - a
  - a
### 88. 🌟🗾[機械学習プロフェッショナルシリーズ 「オンライン予測」](https://www.kspub.co.jp/book/detail/1529229.html)
  - 著名な機械学習プロフェッショナルシリーズより，オンライン予測にフォーカスして書かれた一冊．エキスパート統合問題やオンライン凸最適化など，オンライン予測の主要な内容を一通り学べる．
### 89. 🗾[機械学習プロフェッショナルシリーズ 「オンライン機械学習」](https://www.kspub.co.jp/book/detail/1529038.html)
  - 同じく機械学習プロフェッショナルシリーズより，オンライン機械学習を取り上げた一冊（出版は「オンライン予測」よりも前）．オンライン予測を含む，より広範な内容を学べる．「オンライン予測」よりも平易．
### 90. 🗾[機械学習プロフェッショナルシリーズ 「バンディット問題の理論とアルゴリズム」](https://www.kspub.co.jp/book/detail/1529175.html)
  - 同じく機械学習プロフェッショナルシリーズより．バンディット問題におけるリグレット解析や応用例などをより専門的に扱っている．

## Videos（動画）
### 91. 🌟[An introduction to regret analysis: environment models and best-of-both-worlds](https://youtu.be/pCER8iuTdR4?si=XAL6lP5tj0mMf8yp)
  - Awesome introduction on online learning, regret analysis, and best-of-both-worlds algorithms in the Machine Learning Summer School 2024.
  - オンライン学習，リグレット解析，Best-of-both-worldsアルゴリズムについてのMachine Learning Summer School 2024での講演．
### 92. [Predict with online prediction in Vertex AI](https://youtu.be/TEE7uUbXWDY?si=nHXMfZyTb13KpmWD)
  - Awesome tutorial on how to make predictions on tabular datasets with online prediction in Vertex AI. [GitHub Link](https://github.com/rafaello9472/c4ds/tree/main/Predict%20with%20online%20prediction%20in%20Vertex%20AI)
  - GoogleのVertex AIを用いて表形式のデータに対してオンライン予測を行う方法についてのチュートリアル．[GitHub Link](https://github.com/rafaello9472/c4ds/tree/main/Predict%20with%20online%20prediction%20in%20Vertex%20AI)
### 93. ["Online" prediction vs "batch" prediction in machine learning](https://youtu.be/DnmWTIeQ7PM?si=Mg8xcbWXyzlP3vLY)
  - Awesome explanation by Chip Huyen on the difference between online prediction and more common batch prediction and their applications.
  - Chip Huyenによる，オンライン予測と馴染み深いバッチ予測との違いやそれらの応用例についての短い解説．
### 94. [ML Drift: Identifying Issues Before You Have a Problem](https://youtu.be/uOG685WFO00?si=7_ti70FDTD-B5tbO)
  - Awesome presentation by Amy Hodler on ML drifts and how to fix them. [Blog](https://www.fiddler.ai/blog/drift-in-machine-learning-how-to-identify-issues-before-you-have-a-problem)
  - Amy Hodlerによる，MLドリフトやその解決方法についてのプレゼンテーション．[ブログ](https://www.fiddler.ai/blog/drift-in-machine-learning-how-to-identify-issues-before-you-have-a-problem)

## Articles（記事）
### 95. [What is Online Machine Learning?](https://medium.com/value-stream-design/online-machine-learning-515556ff72c5)
  - A blog post explaining the concept of online machine learning.
  - オンライン学習のコンセプトについて解説したブログ記事．
### 96. [Anomalies detection using River](https://medium.com/spikelab/anomalies-detection-using-river-398544d3536)
  - A blog post explaining anomaly detection using River, including practical code examples.
  - Riverを用いた異常検知について，実際のコードを交えて解説したブログ記事．
### 97. 🗾[私のブックマーク「オンライン学習」](https://www.ai-gakkai.or.jp/resource/my-bookmark/my-bookmark_vol30-no5/)
  - 人工知能学会誌の連載「私のブックマーク」でオンライン学習を特集した際の記事．オンライン学習に関するサーベイやチュートリアル，関連学会，関連ライブラリをまとめている．
### 98. 🗾[私のブックマーク「多腕バンディット問題」](https://www.ai-gakkai.or.jp/resource/my-bookmark/my-bookmark_vol31-no5/)
  - 同じく「私のブックマーク」より，多腕バンディット問題を特集した回の記事．逐次的な意思決定であるバンディット問題に関するチュートリアルや関連学会，関連ライブラリ，重要論文をまとめている．
### 99. [Deus Ex Machina「Online learning and online prediction（オンライン学習とオンライン予測について）」](https://deus-ex-machina-ism.com/?p=17082)
  - Good for understanding the confusing differences between online learning and online prediction, and for gaining an overview of their respective scopes.
  - 混同しやすいオンライン学習とオンライン予測の違いを知り，それぞれの範囲を概観するのに良い．
### 100. [Deus Ex Machina「Overview of online forecasting technology and various applications and implementations（オンライン予測技術の概要と様々な適用事例と実装例）」](https://deus-ex-machina-ism.com/?p=53594)
  - It introduces algorithms, libraries, applications, and suitable books for learning used in online prediction.
  - オンライン予測で使用されるアルゴリズム，ライブラリ，応用例，学習に適した書籍が紹介されている．
