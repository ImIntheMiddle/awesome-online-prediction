# 😎 Awesome-Online-Prediction [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome online-prediction papers, tools, and resources.

Created and hosted by the members of group 5 in the 28th **M**eeting on **I**mage **R**ecognition and **U**nderstanding ([MIRU2025](https://cvim.ipsj.or.jp/MIRU2025/index-en.html)) Young Researchers Program.

[画像の認識・理解シンポジウム（MIRU2025）](https://cvim.ipsj.or.jp/MIRU2025/index.html)で企画された [若手プログラム](https://sites.google.com/view/miru2025wakate) における，グループ５による取り組みの成果です．

オンライン予測に関する重要な論文，ライブラリ，学習のためのリソースなどをまとめています．

> [!TIP]
> Super-awesome ones are marked with a star🌟.
> 
> Japanese-only references are marked with Japan🗾.
> 
> 特に重要・有用と思われるものには星印🌟を付しています．
> 
> 日本語のみの文献には日本🗾を付しています．

Progress: ![](https://geps.dev/progress/100)

# 📑 Papers（論文）
## Awesome-Surveys（サーベイ）
### 1. 🌟[Hoi _et al._ (Neurocomputing, 2018), Online Learning: A Comprehensive Survey](https://arxiv.org/abs/1802.02871)
  - Published in 2018, this survey has been cited over 1,000 times and broadly covers online learning and online prediction topics.
  - 2018年の発表だが，1000回以上引用されているサーベイ．オンライン学習やオンライン予測の内容を広く取り上げている．
### 2. 🌟[Foster and Rakhlin (arXiv, 2023), Foundations of Reinforcement Learning and Interactive Decision Making](https://arxiv.org/abs/2312.16730)
  - This lecture note introduces various decision-making problems, including online learning and prediction, and explains the theoretical foundations of online reinforcement learning.
  - オンライン学習・予測を含めた各種の意思決定問題について紹介し，オンライン強化学習の理論的基礎までを解説した講義ノート．
### 3. 🌟[Shalev-Shwartz (Foundations and Trends in Machine Learning, 2011), Online Learning and Online Convex Optimization](https://www.cs.huji.ac.il/~shais/papers/OLsurvey.pdf)
  - This paper provides a foundational and comprehensive survey of the theory of online learning, with a special focus on the framework of online convex optimization, which has become a cornerstone of the field. It serves as a key reference for understanding how various online learning algorithms can be unified and analyzed through the central concept of convexity.
  - オンライン学習の理論に関する基礎的かつ包括的な概観を提供するものであり，特にこの分野の基礎となっているオンライン凸最適化のフレームワークに焦点を当てている．様々なオンライン学習アルゴリズムが，凸性という中心的な概念を通じていかに統合され，分析されうるかを理解するための重要な参考文献として位置づけられる．
### 4. [Orabona (arXiv, 2019), A Modern Introduction to Online Learning](https://arxiv.org/abs/1912.13213)
  - This textbook introduces the fundamental concepts and algorithms of online learning from the perspective of online convex optimization, without requiring prior specialized knowledge.
  - 専門的な予備知識を必要とせずに，オンライン凸最適化の観点からオンライン学習の基本概念とアルゴリズムを紹介する教科書．

## Awesome-Theoretical Research（基礎研究）
### 5. [Hannan (Contributions to the Theory of Games, 1957), Approximation to Bayes risk in repeated plays](http://www-stat.wharton.upenn.edu/~steele/Resources/Projects/SequenceProject/Hannan.pdf)
  -   This paper provides a foundational framework for sequential decision-making under uncertainty by introducing a strategy for repeated games. Its key contribution is demonstrating that the regret—the difference between the cumulative loss of the sequential strategy and that of the best single fixed strategy chosen in hindsight—is provably bounded and grows at a sublinear rate of $O(\sqrt{N})$, where $N$ is the number of repetitions. This work established a formal basis for regret minimization, a central concept in online prediction, and provided one of the first concrete algorithms with a performance guarantee against an arbitrary sequence of outcomes.
  - この論文は，繰り返しゲームにおける戦略を導入することにより，不確実性の下での逐次意思決定の基礎的な枠組みを提供した．その中心的な貢献は，リグレット（逐次戦略の累積損失と，後から見て最善であった単一の固定戦略の損失との差）が，証明可能に有界であり，繰り返し回数を $N$ として $O(\sqrt{N})$ という準線形なレートで増大することを示した点にある．この研究は，オンライン予測の中心概念であるリグレット最小化の形式的な基礎を築き，任意の結果系列に対する性能保証を持つ最初の具体的なアルゴリズムの一つを提示した．
### 6. 🌟[Nesterov (Soviet Mathematics Doklady, 1983), A Meyhod of Solving a Convex Programming Problem with Convergence Rate O(1/k²)](https://hengshuaiyao.github.io/papers/nesterov83.pdf)
  - This paper introduces what is now known as Nesterov's Accelerated Gradient (NAG) method, a landmark achievement in convex optimization. Its role in online prediction is a fundamental building block for creating highly efficient algorithms. By providing a method that achieves a faster convergence rate of $O(1/k^2)$ for smooth convex functions, it enables online learning algorithms to adapt much more rapidly and achieve better performance (i.e., lower regret), forming the theoretical basis for many state-of-the-art methods in online convex optimization.
  - この論文は，現在ネステロフの加速勾配法として知られる凸最適化における画期的な成果を導入したものである．オンライン予測におけるこの論文の役割は，非常に効率的なアルゴリズムを作成するための基本的な構成要素である．平滑な凸関数に対して $O(1/k^2)$ という速い収束率を達成する手法を提供することによって，オンライン学習アルゴリズムがより迅速に適応し，より良いパフォーマンス（すなわち，より低いリグレット）を達成することを可能にし，オンライン凸最適化における多くの最先端手法の理論的基礎を形成している．
### 7. [Littlestone (Machine Learning, 1988), Learning Quickly When Irrelevant Attributes Abound: A New Linear-Threshold Algorithm](https://link.springer.com/article/10.1023/A:1022869011914)
  - This paper introduces the Winnow algorithm, which is a seminal contribution to online learning. Its primary importance lies in providing a mistake-bound model that is highly effective in high-dimensional settings where many attributes are irrelevant. The number of mistakes Winnow makes grows only logarithmically with the number of irrelevant attributes, making it significantly more efficient than previous algorithms like the Perceptron in such scenarios. This established a foundational approach for handling sparse target concepts efficiently within the online learning framework.
  - この論文は，オンライン学習への独創的な貢献である Winnow アルゴリズムを導入したものである．その主な重要性は，多くの属性が無関係である高次元の状況において非常に効果的な誤り回数保証付きのモデルを提供した点にある．Winnow が犯す誤りの回数は，無関係な属性の数に対して対数的にしか増加しないため，このようなシナリオにおいてパーセプトロンのような以前のアルゴリズムよりも著しく効率的である．これにより，オンライン学習の枠組みの中で，スパースなターゲット概念を効率的に扱うための基礎的なアプローチを確立した．
### 8. [Herbster and Warmuth (Machine Learning, 1998), Tracking the Best Expert](https://link.springer.com/article/10.1023/A:1007424614876)
  - This paper extends the online prediction framework to non-stationary environments, introducing an algorithm that tracks the best-performing expert whose identity may change over time, thus moving beyond simpler models that assume a single, static best expert.
  - この論文は，時間の経過とともに性能が最も良い専門家が変化しうる非定常環境へオンライン予測の枠組みを拡張した．単一の静的な最良エキスパートを仮定する単純なモデルから脱却し，変化する最良エキスパートを追跡するアルゴリズムを導入したものである．
### 9. 🌟[Vovk (JCSS, 1998), A Game of Prediction with Expert Advice](https://www.sciencedirect.com/science/article/pii/S0022000097915567)
  - This paper establishes a foundational game-theoretic framework for online prediction, where the problem is modeled as a game between a predictor and an adversary. It introduces the concept of "prediction with expert advice" and provides a powerful "Aggregating Algorithm" that guarantees the predictor's loss to be close to the loss of the best expert in hindsight, thereby offering a robust theoretical underpinning for the field.
  - この論文は，予測問題を予測者と敵対者の間のゲームとしてモデル化する，オンライン予測のための基礎的なゲーム理論的枠組みを確立したものである．「エキスパートの助言を伴う予測」という概念を導入し，予測者の損失が事後的に見て最良のエキスパートの損失に近くなることを保証する強力な「集約アルゴリズム」を提供し，この分野に強固な理論的基礎を与えた，
### 10. [Kivinen and Warmuth (EuroCOLT1999), Averaging Expert Predictions](https://link.springer.com/chapter/10.1007/3-540-49097-3_13)
  - This paper is a fundamental research in online learning algorithms that generate their own predictions by averaging expert predictions, specifically proposing a method where the algorithm's prediction is a weighted average of the experts' predictions, with weights that decrease exponentially according to the loss incurred by each expert, and demonstrating that the algorithm's additional loss is bounded by the logarithm of the number of experts.
  - この論文は，専門家の予測を平均することで自己の予測を生成するオンライン学習アルゴリズムに関する基礎研究である．具体的には，アルゴリズムの予測が専門家の予測の重み付き平均であり，その重みは各専門家が被った損失に応じて指数関数的に減少し，アルゴリズムの追加損失が専門家数の対数によって束縛されることを示したものである．
### 11. [Kivinen and Warmuth (Machine Learning, 2001), Relative Loss Bounds for Multidimensional Regression Problems](https://link.springer.com/article/10.1023/A:1017938623079)
  - This paper extends the theoretical analysis of online learning algorithms, previously limited to one-dimensional output, to multidimensional output, and specifically derived relative loss bounds for multidimensional generalized linear regression problems. This provided a more practical evaluation criterion for multidimensional problems by eliminating probabilistic assumptions about the data and comparing the algorithm's performance to the best offline predictor.
  - この論文は，それまで一次元出力に限定されていたオンライン学習アルゴリズムの理論的解析を多次元出力へと拡張し，特に多次元の一般化線形回帰問題に対して相対的な損失限界を導出した．これにより，データの確率的な仮定を排除し，アルゴリズムの性能を最良のオフライン予測器と比較するという，より実践的な評価基準を多次元問題に提供した．
### 12. 🌟[Zinkevich (ICML2003), Online Convex Programming and Generalized Infinitesimal Gradient Ascent](https://people.eecs.berkeley.edu/~brecht/cs294docs/week1/03.Zinkevich.pdf)
  - This paper introduces the "Online Convex Programming" framework for uniformly handling many online prediction problems and showed that a simple gradient-descent-based algorithm can achieve a low regret of $O(\sqrt{T})$ compared to the best single decision in hindsight.
  - この論文は，多くのオンライン予測問題を統一的に扱うための「オンライン凸計画法」というフレームワークを提案し，単純な勾配降下法に基づくアルゴリズムで，後知恵で最適であった単一の決定と比較して $O(\sqrt{T})$ という低いリグレットを達成できることを示した．
### 13. 🌟[Kalai and Vempara (JCSS, 2005), Efficient algorithms for online decision problems](https://www.sciencedirect.com/science/article/pii/S0022000004001394) 
  - This paper introduces the "Follow the Perturbed Leader" (FPL) algorithm, a simple and computationally efficient method for online decision problems. Its key contribution is demonstrating that by adding random noise to the simple strategy of following the leader, it's possible to achieve performance (regret bounds) competitive with much more complex algorithms, especially in situations with a vast number of experts or actions. This opened the door for applying theoretically guaranteed online learning to many problems where it was previously computationally impractical.
  - この論文は，「Follow the Perturbed Leader」（FPL）アルゴリズムという，オンライン決定問題に対する単純かつ計算効率の良い手法を導入した．その主要な貢献は，これまでの最善手を選択するという単純な戦略にランダムなノイズを加えるだけで，特にエキスパートや行動の選択肢が膨大な状況において，はるかに複雑なアルゴリズムに匹敵する性能（リグレット限界）を達成できることを示した点にある．これにより，計算が非現実的であった多くの問題に対して，理論的に性能が保証されたオンライン学習を適用する道を拓いた．
### 14. [Crammer _et al._ (JMLR, 2006), Online Passive-Aggressive Algorithms](https://jmlr.org/papers/v7/crammer06a.html)
  - This paper proposes a new framework in online learning called "Passive-Aggressive" (PA) algorithms. Its core lies in performing updates based on the margin (prediction confidence): if the prediction is correct and has a sufficient margin, it remains "passive" and does nothing, but if the margin is insufficient, it acts "aggressively" by making the minimal update required to satisfy the margin constraint. This simple and clear approach provided a powerful online learning method that is computationally efficient and has theoretical performance guarantees (regret bounds), especially for large-scale datasets and data streams.
  - この論文は，オンライン学習における「パッシブ・アグレッシブ」（PA）アルゴリズムという新たな枠組みを提唱した．その核心は，マージン（予測の信頼度）に基づいて更新を行う点にあり，予測が正しく，かつ十分なマージンがある場合は「パッシブ」に何もしないが，マージンが不十分な場合は「アグレッシブ」に，マージン制約を満たす最小限の更新を行うというものである．この単純明快なアプローチにより，特に大規模なデータセットやストリームデータに対して，計算効率が高く，かつ理論的な性能保証(リグレット限界)を持つ強力なオンライン学習手法を提供した．
### 15. [Hazan _et al._ (Machine Learning, 2007), Logarithmic Regret Algorithms for Online Convex Optimization](https://link.springer.com/article/10.1007/s10994-007-5016-8)
  - This paper significantly improves upon the previous general regret bound of $O(\sqrt{T})$ in online convex optimization. Its core contribution lies in being the first to propose an algorithm that achieves logarithmic regret, $O(\log{T})$, under the condition that the loss functions possess the property of "strong convexity." This demonstrates that for a specific (yet important) class of problems, online learning can converge to the optimal solution much more rapidly, thus opening a new frontier in regret analysis.
  - この論文は，それまでのオンライン凸最適化における一般的なリグレット限界であった $O(\sqrt{T})$ を大幅に改善する．その核心的な貢献は，損失関数が「強凸性」という性質を持つ場合に限定すれば，$O(\log{T})$ という対数的なリグレットを達成できるアルゴリズムを初めて提案した点にある，これにより，特定の（しかし重要な）問題クラスにおいては，オンライン学習がはるかに速く最適解に収束することを示し，リグレット解析の新たな地平を切り拓いた．
### 16. [Cesa-Bianchi _et al._ (Machine Learning, 2007), Improved second-order bounds for prediction with expert advice](https://arxiv.org/abs/math/0602629)
  - This paper re-evaluates the performance of online prediction with expert advice using a more precise measure called "second-order bounds." Whereas previous first-order bounds related regret only to the cumulative loss of the best expert, this research derived tighter regret bounds by taking into account the "variance" of the experts' losses. This demonstrated that in situations where expert losses are stable, the algorithm can perform significantly better than previously thought, adding a new layer of depth to the performance analysis of online learning algorithms.
  - この論文は，エキスパートからの助言によるオンライン予測の性能評価を，より精密な「二次の限界 (second-order bounds) 」という尺度で捉え直した．従来の一次の限界がリグレットを最良のエキスパートの累積損失のみに関連付けていたのに対し，この研究ではエキスパートたちの損失の「分散」を考慮に入れることで，よりタイトなリグレット限界を導出した．これにより，エキスパートたちの損失が安定している状況では，アルゴリズムが従来考えられていたよりもはるかに優れた性能を発揮することを示し，オンライン学習アルゴリズムの性能解析に新たな深みを与えたものである．
### 17. [Crammer _et al._ (EMNLP2009), Multi-Class Confidence Weighted Algorithms](https://aclanthology.org/D09-1052/)
  - This paper extends "Confidence-Weighted" (CW) learning, a sophisticated evolution of Passive-Aggressive algorithms, to the multi-class classification setting. Its groundbreaking aspect is that instead of updating a single parameter vector, it models parameter uncertainty with a multivariate Gaussian distribution and adjusts the magnitude of updates according to its "confidence" (the inverse of the variance). By updating the weights of low-confidence (infrequently observed) features more aggressively and high-confidence weights more conservatively, it enables more informed and efficient learning, especially for high-dimensional, sparse data common in fields like Natural Language Processing, significantly influencing subsequent online learning research.
  - この論文は，それまでのパッシブ・アグレッシブアルゴリズムなどを発展させ，「信頼度加重」（Confidence-Weighted, CW）学習という，より洗練されたオンライン学習手法を多クラス分類問題へと拡張した．単一のパラメータベクトルを更新するのではなく，パラメータの不確実性を多変量正規分布でモデル化し，その「信頼度」(分散の逆数)に応じて更新の度合いを調整するという点が画期的である，信頼度が低い(あまり観測されていない)特徴の重みは大きく，信頼度が高い重みは小さく更新することで，特に自然言語処理などで見られる高次元で疎なデータに対して，より情報量に基づいた効率的な学習を可能にし，その後のオンライン学習研究に大きな影響を与えた．
### 18. 🌟[Crammer _et al._ (NeurIPS2009), Adaptive Regularization of Weight Vectors](https://papers.nips.cc/paper_files/paper/2009/hash/8ebda540cbcc4d7336496819a46a1b68-Abstract.html)
  - This paper introduces the "Adaptive Regularization of Weight Vectors" (AROW) algorithm, which overcomes a key limitation of preceding methods like Confidence-Weighted (CW) learning: vulnerability to noisy data. Its primary role is to significantly improve robustness by incorporating a soft-margin objective while inheriting the concept of "confidence" from CW (representing parameter uncertainty with a covariance matrix). This established a more practical algorithm that enjoys the benefits of second-order adaptive updates while remaining stable against mislabeled examples.
  - この論文は，先行研究である信頼度加重 (CW) 学習の課題，すなわちノイズの多いデータへの脆弱性を克服する「重みベクトルの適応的正則化」(AROW) アルゴリズムを提案した．その主要な役割は，CW が持つ「信頼度」の概念（パラメータの不確実性を共分散行列で表現する点）を引き継ぎつつ，ソフトマージン目的を導入することで，頑健性を大幅に向上させた点にある．これにより，信頼度に基づいた適応的な更新という二次のオンライン学習手法の利点を享受しながら，誤ったラベルを持つサンプルに対しても安定した学習を可能にし，より実用的なアルゴリズムを確立したものである．
### 19. 🌟[Duchi _et al._ (JMLR, 2010), Adaptive Subgradient Methods for Online Learning and Stochastic Optimization](https://jmlr.org/papers/v12/duchi11a.html)
  - This paper shatters the limitations of previous online learning methods using fixed learning rates by proposing "Adaptive Subgradient Methods," most notably its prime example, "AdaGrad," which adaptively adjusts the learning rate for each individual parameter (feature). Its core innovation lies in automatically adjusting the learning rate based on the magnitude of past gradients, applying smaller learning rates to frequently occurring features and larger rates to infrequent ones. This mechanism dramatically improved learning efficiency and performance, especially for the high-dimensional, sparse data common in fields like Natural Language Processing, and laid the foundation for many subsequent adaptive learning rate algorithms (e.g., RMSProp, Adam).
  - この論文は，それまでのオンライン学習で一般的であった固定の学習率を用いる手法の限界を打ち破り，個々のパラメータ（特徴）ごとに学習率を適応的に調整する「適応的劣勾配法」(Adaptive Subgradient Methods)，特にその代表格である「AdaGrad」を提案した．その核心は，過去の勾配の大きさに応じて学習率を自動で調整する点にあり，頻繁に現れる特徴には小さな学習率を，稀にしか現れない特徴には大きな学習率を適用する，この仕組みにより，特に自然言語処理などで頻出する高次元で疎なデータに対して，学習の効率と性能を劇的に向上させ，その後の多くの適応的学習率アルゴリズム (例:RMSProp, Adam) の礎を築いたものである．
### 20. [McDonald _et al._ (NAACL HLT2010), Distributed Training Strategies for the Structured Perceptron](https://aclanthology.org/N10-1069.pdf)
  - This paper is the first to systematically propose and compare "distributed training strategies" for the structured perceptron, for which single-machine training was previously the mainstream, to efficiently train it on large-scale datasets. Its key role lies in introducing various distributed strategies, from simple mini-batch learning to the more sophisticated iterative parameter mixing, and experimentally clarifying their impact on training speed and final prediction performance. By doing so, it showed a concrete path for adapting online learning algorithms to the era of big data and contributed significantly to the subsequent development of distributed learning research.
  - この論文は，それまで単一のマシンでの学習が主流であった構造化パーセプトロンを，大規模なデータセットに対して効率的に学習させるための「分散学習戦略」を初めて体系的に提案・比較した．その重要な役割は，単純なミニバッチ学習から，より洗練された反復パラメータ混合 (iterative parameter mixing) まで，様々な分散戦略を導入し，それらが学習速度と最終的な予測性能に与える影響を実験的に明らかにした点にある．これにより，オンライン学習アルゴリズムをビッグデータの時代に適応させるための具体的な道筋を示し，後の分散学習研究の発展に大きく貢献した．
### 21. [Chu _et al._ (KDD2011), Unbiased online active learning in data streams](https://dl.acm.org/doi/10.1145/2020408.2020444)
  - Awesome paper that addresses unbiased online active learning in data streams, providing theoretical guarantees for selective sampling strategies.
  - データストリームに対する不偏オンライン能動学習に取り組み，選択的サンプリング戦略の理論保証を与えた論文．
### 22. [Shalev-Shwartz _et al._ (Mathematical Programming, 2017), Pegasos: primal estimated sub-gradient solver for SVM](https://link.springer.com/article/10.1007/s10107-010-0420-4)
  - Awesome paper that introduces Pegasos algorithm for SVM training with convergence guarantees.
  - SVM（サポートベクターマシン）の学習のためのアルゴリズムであるPegasosを提案し，収束保証を与えた論文．
### 23. 🌟[Cesa-Bianchi and Lugosi (JCSS, 2012), Combinatorial bandits](https://www.sciencedirect.com/science/article/pii/S0022000012000219)
  - Awesome paper that introduces combinatorial bandits framework, extending multi-armed bandits to combinatorial action spaces with efficient algorithms.
  - 組合せ論的バンディットの枠組みを導入し，多腕バンディットを組合せ行動空間に拡張して効率的アルゴリズムを提供した論文．
### 24. 🌟[Suehiro _et al._ (ALT2012), Online Prediction under Submodular Constraints](https://api.lib.kyushu-u.ac.jp/opac_download_md/1932327/alt12.pdf)
  - Awesome paper that studies online prediction under submodular constraints, providing regret bounds for constrained online learning problems.
  - 劣モジュラ制約下でのオンライン予測に取り組み，制約付きオンライン学習問題のリグレット境界を与えた論文．
### 25. [Wang _et al._ (ICML2012), Exact Soft Confidence-Weighted Learning](https://arxiv.org/abs/1206.4612)
  - Awesome paper that develops exact soft confidence-weighted learning, providing precise probabilistic updates for online classification with theoretical guarantees.
  - オンライン分類における，理論保証付きのより優れた確率的更新として「Exact Soft Confidence-Weighted Learning」を提案した論文．
### 26. 🌟[Bubeck and Slivkins (COLT2012), The best of both worlds: stochastic and adversarial bandits](http://sbubeck.com/COLT12_BS.pdf)
  - Awesome paper that achieves the best of both worlds in bandits, providing algorithms that perform well in both stochastic and adversarial settings simultaneously.
  - バンディット問題で確率的・敵対的両設定で同時に最良性能を達成した論文．
### 27. [Neu and Bartók (ALT2013), An efficient algorithm for learning with semi-bandit feedback](https://arxiv.org/abs/1305.2732)
  - Awesome paper that provides efficient algorithms for semi-bandit feedback, extending bandit learning to partial information settings with multiple simultaneous actions.
  - セミバンディットフィードバックから学習する効率的なアルゴリズムを提供し，バンディット学習を複数同時行動を伴う部分情報設定に拡張した論文．
### 28. [Gaillard _et al._ (COLT2014), A Second-order Bound with Excess Losses](https://arxiv.org/abs/1402.2044)
  - Awesome paper that derives second-order regret bounds with excess losses, providing tighter analysis for online learning algorithms using variance information.
  - 過剰損失を用いた2次リグレット境界を導出し，分散情報を活用したオンライン学習アルゴリズムにより厳密な解析を与えた論文．
### 29. 🌟[Kingma and Ba (ICLR2015), Adam: A Method for Stochastic Optimization](https://arxiv.org/abs/1412.6980)
  - Awesome paper that introduces Adam optimizer combining advantages of AdaGrad and RMSprop, becoming the most widely used adaptive optimization method.
  - AdaGradとRMSpropの利点を組み合わせたAdamオプティマイザーを導入し，最も広く使用される適応的最適化手法となった論文．
### 30. [Luo and Schapire (COLT2015), Achieving All with No Parameters: AdaNormalHedge](https://proceedings.mlr.press/v40/Luo15.pdf)
  - Awesome paper that proposes AdaNormalHedge, a truly parameter-free algorithm for expert advice that simultaneously achieves multiple objectives without prior information including adaptive regret and unknown competitor performance. 
  - エキスパート統合問題において，事前情報（ステップサイズやエキスパートの数など）を必要としないパラメータフリーなオンラインアルゴリズム「AdaNormalHedge」を提案．
### 31. [Hazan _et al._ (ICML2017), Efficient Regret Minimization in Non-Convex Games](https://proceedings.mlr.press/v70/hazan17a.html)
  - Awesome paper that studies online algorithms for non-convex loss functions, defining a new measure called "local regret" based on projected gradient magnitudes from time-smoothed losses and proposing algorithms to efficiently minimize it.
  - 非凸な損失関数を対象としたオンラインアルゴリズムの研究．時間平滑化した損失（過去k回の損失を平均したもの）から計算される射影勾配の大きさを基にした新しい尺度「局所リグレット」を定義し，それを効率的に最小化するアルゴリズムを提案．
  ### 32. 🌟[Zheng and Kwok (ICML2017), Follow the Moving Leader in Deep Learning](https://proceedings.mlr.press/v70/zheng17a.html)
  - Awesome paper that proposes Follow the Moving Leader (FTML), a variant of FTRL for deep learning optimization that adapts quickly to changes by weighting recent samples more heavily. 
  - 深層学習の最適化において，最近のサンプルをより重く重み付けすることで変化に素早く適応するFollow the Moving Leader (FTML) アルゴリズムを提案した論文．
### 33. 🌟[Zhang _et al._ (NeurIPS2018), Adaptive Online Learning in Dynamic Environments](https://arxiv.org/abs/1810.10815)
  - Awesome paper that first establishes theoretical lower bounds for dynamic regret against arbitrary comparison sequences and proposes "Ader" which adaptively combines multiple OGD experts with different step sizes using a meta-algorithm.
  - 任意の比較対象シーケンスに対する動的リグレットの理論的な下限を初めて提示した研究．理論的な下限と一般的なOGDとの動的リグレットに乖離があることを指摘し，その解決策として異なるステップサイズを持つ複数のOGD（エキスパート）をメタアルゴリズムで適応的に統合する手法「Ader」を提案．
### 34. [Finn _et al._ (ICLR2019), Online Meta-Learning](https://arxiv.org/abs/1902.08438)
  - Awesome paper that introduces online meta-learning which merges ideas from meta-learning and online learning, proposing the follow the meta leader algorithm extending MAML with O(log T) regret guarantee.
  - メタ学習とオンライン学習のアイデアを融合したオンラインメタ学習を導入し，MAMLを拡張したfollow the meta leaderアルゴリズムをO(log T)のregret保証とともに提案した論文．
### 35. [Zhao _et al._ (NeurIPS2020), Dynamic Regret of Convex and Smooth Functions](https://arxiv.org/abs/2007.03479)
  - Awesome paper that enhances dynamic regret bounds by exploiting smoothness conditions, replacing the dependence on T with problem-dependent quantities like gradient variation and comparator loss, making bounds adaptive to problem difficulty.
  - 凸かつ滑らかな関数に対する動的リグレットを研究し，滑らかさ条件を活用してTへの依存を勾配変動や比較対象の損失などの問題依存量に置き換え，問題の難易度に適応的な境界を提案した論文．
### 36. [Ito (NeurIPS2021), On Optimal Robustness to Adversarial Corruption in Online Decision Problems](https://arxiv.org/abs/2109.10963)
  - Awesome paper that studies optimal robustness to adversarial corruption in online decision problems, analyzing how online algorithms can maintain performance guarantees when a fraction of inputs are adversarially corrupted.
  - オンライン決定問題における敵対的摂動に対する最適な頑健性を研究し，入力の一部に敵対的な摂動が加わった場合でもオンラインアルゴリズムが性能保証を維持する方法を解析した論文．
### 37. 🌟[Zimmert and Seldin (JMLR, 2021), Tsallis-INF: An Optimal Algorithm for Stochastic and Adversarial Bandits](https://arxiv.org/abs/1807.07623)
  - Awesome paper that derives Tsallis-INF algorithm using online mirror descent with Tsallis entropy regularization, achieving optimal regret in both stochastic and adversarial multi-armed bandits.
  - Tsallisエントロピー正則化を用いたオンラインミラー降下法に基づくTsallis-INFアルゴリズムを導出し，確率的・敵対的多腕バンディット両方で最適なリグレットを達成した論文．
### 38. 🌟[Baby _et al._ (NeurIPS2023), Online Label Shift: Optimal Dynamic Regret meets Practical Algorithms](https://neurips.cc/virtual/2023/poster/71994)
  - Awesome paper that tackles online learning under changing data distributions, developing practical algorithms that automatically adapt to distribution shifts without prior knowledge while achieving optimal theoretical guarantees.
  - データ分布が変化するオンライン学習環境において，分布シフトに事前知識なしで自動適応する実用的アルゴリズムを開発し，最適な理論保証を達成した論文．
### 39. [Dai _et al._ (CVPR2025), Label Shift Meets Online Learning: Ensuring Consistent Adaptation with Universal Dynamic Regret](https://openaccess.thecvf.com/content/CVPR2025/html/Dai_Label_Shift_Meets_Online_Learning_Ensuring_Consistent_Adaptation_with_Universal_CVPR_2025_paper.html)
  - Awesome paper that addresses label shift in online learning settings by constructing a novel convex risk estimator and enhanced online algorithm, achieving minimax optimal universal dynamic regret.
  - オンライン学習環境でのラベルシフト問題に対して新しい凸リスク推定器とオンラインアルゴリズムを構築し，minimax最適な汎用動的リグレットを達成した論文．

## Awesome-Applied Research（応用研究）
### 40. 🌟[Bashratat _et al._ (CVPR2008), Learning object motion patterns for anomaly detection and improved object detection](https://ieeexplore.ieee.org/document/4587510)
  - Awesome paper that learns object motion patterns in surveillance videos for anomaly detection and improved object detection.
  - 監視映像における応用として，物体の動きパターンをオンライン学習し，異常検知と物体検出を改善する手法を提案した論文．
### 41. [Arora _et al._ (Theory of Computing, 2012), The Multiplicative Weights Update Method: a Meta-Algorithm and Applications](https://theoryofcomputing.org/articles/v008a006/)
  - Awesome paper that presents multiplicative weights update as a meta-algorithm with broad applications across computer science and optimization.
  - 乗法的重み更新をメタアルゴリズムとして捉え，その幅広い応用を示した論文．
### 42. [Ho _et al._(NeurIPS2013), More Effective Distributed ML via a Stale Synchronous Parallel Parameter Server](https://fid3024.github.io/papers/2013%20-%20More%20Effective%20Distributed%20ML%20via%20a%20Stale%20Sychronous%20Parallel%20Parameter%20Server.pdf)
  - Awesome paper that introduces Stale Synchronous Parallel Parameter Server for distributed machine learning, improving efficiency through asynchronous updates.
  - 分散機械学習のための「Stale Synchronous Parallel Parameter Server」を導入し，非同期更新により効率性を向上させた論文．
### 43. [McMahan _et al._ (KDD2013), Ad Click Prediction: a View from the Trenches](https://research.google/pubs/ad-click-prediction-a-view-from-the-trenches/)
  - Awesome paper that presents practical insights for ad click prediction from large-scale deployment, bridging theory and real-world online learning applications.
  - 大規模なデプロイ環境における広告クリック予測に取り組み，オンライン学習の理論と実世界における応用を橋渡しした論文．
### 44. [Grnarova _et al._ (ICLR2018), An Online Learning Approach to Generative Adversarial Networks](https://arxiv.org/abs/1706.03269)
  - Awesome paper that applies online learning techniques to GAN training for improved stability.
  - GANの訓練にオンライン学習手法を適用して安定性を向上させた論文．
### 45. [Song _et al._ (Machine Learning, 2024), No Regret Sample Selection with Noisy Labels](https://arxiv.org/abs/2003.03179)
  - Awesome paper that proposes adaptive k-set selection for training DNNs with noisy labels while providing theoretical regret bounds. 
  - ノイジーラベルを持つデータでのDNN訓練において，理論的なリグレット保証を持つ適応的k-set選択手法を提案した論文．
### 46. [Song _et al._ (WACV2020), Adaptive Aggregation of Arbitrary Online Trackers with a Regret Bound](https://openaccess.thecvf.com/content_WACV_2020/papers/Song_Adaptive_Aggregation_of_Arbitrary_Online_Trackers_with_a_Regret_Bound_WACV_2020_paper.pdf)
  - Awesome paper that proposes delayed-Hedge algorithm for aggregating arbitrary online trackers with theoretical regret guarantees in adversarial environments.
  - 敵対的環境において理論的リグレット保証を持つdelayed-Hedgeアルゴリズムを用い，任意のオンライントラッカーを集約する手法を提案した論文．
### 47. [Matsuo _et al._ (ICASSP2023), Learning from Label Proportion with Online Pseudo-Label Decision by Regret Minimization](https://arxiv.org/abs/2302.08947)
  - Awesome paper that proposes online pseudo-labeling with regret minimization for Learning from Label Proportions, effectively handling large bag sizes.
  - Learning from Label Proportions (LLP) において，リグレット最小化による擬似ラベルのオンライン決定手法を提案した論文．大きなbagサイズでも効果的に動作する．
### 48. [Švihrová _et al._ (Frontiers in Digital Health, 2025), Designing digital health interventions with causal inference and multi-armed bandits: a review](https://www.frontiersin.org/journals/digital-health/articles/10.3389/fdgth.2025.1435917/full)
  - Awesome paper that reviews how to design digital health interventions using multi-armed bandits and causal inference for Just-In-Time Adaptive Interventions in behavioral change support systems.
  - ヘルスケア分野におけるJust-In-Time Interventionに多腕バンディット問題と因果解析を導入する方法論に関するレビュー論文．被験者の健康状態を逐次的にモニタリングし，適切なタイミングで"介入"して行動変容を促す枠組み．
### 49. [Kumar _et al._ (AAAI2024), Using adaptive bandit experiments to increase and investigate engagement in mental health](https://ojs.aaai.org/index.php/AAAI/article/view/30328)
  - Awesome paper that presents a software system using Thompson Sampling bandit algorithms for adaptive text-message-based mental health interventions, evaluated with 1100 users to simultaneously improve engagement and collect data for analysis.
  - メンタルヘルスにおける個別化医療においてThompson Samplingを用いたバンディットアルゴリズムを適用し，シミュレーションと1100人のユーザで実験システムを評価した論文．
### 50. [Gutiérrez _et al._ (MICCAI2017), A Multi-armed Bandit to Smartly Select a Training Set from Big Medical Data](https://link.springer.com/chapter/10.1007/978-3-319-66179-7_5)
  - Awesome paper that formulates efficient training set selection from large-scale medical imaging data as a multi-armed bandit problem, using clustering-based exploration-exploitation for age prediction from brain images.
  - 大規模な医療画像データから訓練データセットを適切かつ効率的に選択する問題を多腕バンディット問題として定式化し，脳画像から得られる特徴量から年齢を予測する問題に取り組んだ論文．事前に観測できるメタデータから有用なサンプルを選択するという問題に落とし込み，データをクラスタリングして有益そうなクラスタを活用しつつ、他のクラスタも探索していく、というアプローチをとった．手法は線形回帰ベースで深層学習ではない．
### 51. [Pandian _et al._ (Scientific Reports, 2025), Enhancing lane detection in autonomous vehicles with multi-armed bandit ensemble learning](https://www.nature.com/articles/s41598-025-86743-z)
  - Awesome paper that introduces Multi-Armed Bandit Ensemble (MAB-Ensemble) for lane detection in autonomous vehicles, dynamically selecting optimal CNN models based on environmental conditions using Thompson sampling.
  - 自動運転車のレーン検出において，Thompson Samplingを用いて環境条件に基づいて最適なCNNモデルを動的選択するMulti-Armed Bandit Ensemble (MAB-Ensemble)を提案した論文．

# 🧰 Tools（ツール）
## Awesome-Libraries（ライブラリ）
### 52. 🌟[River](https://github.com/online-ml/river)
  - A Python library for online machine learning (with over 5k stars), covering time series forecasting, bandits, and so on.
  - オンライン機械学習のためのPythonライブラリ（5000スター超え）で、時系列予測やバンディットなどをカバーしている。
### 53. [scikit-multiflow](https://scikit-multiflow.readthedocs.io/en/stable/index.html)
  - A machine learning library for streaming data in Python (~0.8k stars). Although it can handle drift detection and has a variety of algorithms other than neural networks, River is more common nowadays.
  - ストリーミングデータに適したPython実装の機械学習ライブラリ（約800スター）．ドリフト検出機能を備え，ニューラルネットワーク以外のアルゴリズムも豊富だが，現在ではRiverに主流が移った．
### 54. 🌟[Vowpal Wabbit](https://vowpalwabbit.org/index.html)
  - A machine learning library implemented in various languages (with over 8,500 stars), primarily developed by Microsoft. It supports various learning paradigms, including online learning, and can handle online prediction-related stuff like contextual bandits."
  - Microsoftが中心となって開発している多言語実装の機械学習ライブラリ（8500スター超え）．オンライン学習を含む多様な学習様式に対応しており，Contextual bandits等を扱える．
### 55. [MOA](https://moa.cms.waikato.ac.nz/)
  - An open-source Java framework designed for sequential data processing, boasting over 600 stars.
  - JAVAで実装された，逐次データ処理用のオープンソースフレームワーク．600スター超え． 
### 56. [CapyMOA](https://capymoa.org/)
  - Python implementation of MOA, significantly faster than River and suited for real-time processing.
  - MOAのPython版．Riverよりも大幅に高速化されており，リアルタイム処理向き．
### 57. [Jubatas](http://jubat.us/ja/index.html)
  - A distributed processing framework for online machine learning, jointly developed by PFN and NTT.
  - PFNとNTTが共同で開発していたオンライン機械学習向けの分散処理フレームワーク．
### 58. [Deep-River](https://online-ml.github.io/deep-river/)
  - A library suitable for online learning of deep learning models implemented in PyTorch. Same developers as River (online-ml)."
  - PyTorchで実装された深層学習モデルのオンライン学習に適したライブラリ．Riverと同じonline-mlが開発．

## Awesome-Probability Inequalities (確率不等式)
### 59. [Probability inequalities](https://probability.oer.math.uconn.edu/wp-content/uploads/sites/2187/2020/08/ch15M.pdf)
  - Introduction of several probability inequalities used in proofs.
  - 証明に使用される確率不等式がいくつか紹介されている．
### 60. 🌟[Markov's Inequality ... Made Easy!](https://www.youtube.com/watch?v=e-nAr3MkAII)
  - Awesome YouTube video on Markov's inequality.
  - マルコフの不等式について解説したYouTube動画．
### 61. 🌟[Chebyshev's Inequality ... Made Easy!](https://www.youtube.com/watch?v=mlelI1LA9o4)
  - Awesome YouTube video on Chebyshev's inequality.
  - チェビシェフの不等式について解説したYouTube動画．
### 62. 🗾[【大学数学】チェビシェフの不等式【確率統計】](https://www.youtube.com/watch?v=d-ugoDdXWrU)
  - ヨビノリによるチェビシェフの不等式についての解説動画．
### 63. [What is the Chernoff Bound?](https://www.youtube.com/watch?v=WKUeBoQp2Uo)
  - Awesome YouTube video on Chernoff bound.
  - チェルノフ限界について解説したYouTube動画．
### 64. [L 27 | Cauchy Schwarz Inequality | Probability & Statistics | Digital Communication](https://www.youtube.com/watch?v=14-JD5KiUz0)
  - Awesome YouTube video on Cauchy-Schwarz inequality.
  - コーシー＝シュワルツの不等式について解説したYouTube動画．
  - チェルノフ限界について解説したYouTube動画．
### 65. [Jensen's Inequality](https://www.youtube.com/watch?v=u0_X2hX6DWE)
  - Awesome YouTube video on Jensen's inequality.
  - イェンセンの不等式について解説したYouTube動画．
### 66. [A Visual Introduction to Hoeffding's Inequality - Statistical Learning Theory](https://www.youtube.com/watch?v=lsYPC0MuLJA)
  - Awesome YouTube video visualizing the concept of Hoeffding's inequality.
  - へフディングの不等式について視覚的に解説したYouTube動画．
### 67. [Supplemental Lecture notes Hoeffding’s inequality](https://cs229.stanford.edu/extra-notes/hoeffding.pdf)
  - Lecture material of Stanford University, including an explanation of moment generating functions and a proof of Hoeffding's inequality.
  - モーメント母関数の解説やHoeffdingの不等式の証明を含んだ，スタンフォード大学の講義資料．
### 68. 🗾[ヘフディングの不等式(Hoeffding's inequality)と諸々の確率の評価の不等式](https://ludu-vorton.hatenablog.com/entry/2019/06/06/073000)
  - 統計的学習理論で確率の評価で用いられる様々な不等式（へフディングの不等式を含む）についての解説．

## Awesome-Convex Optimization (凸最適化)
### 69. [Subgradients/Subderivatives - Convex Analysis](https://www.youtube.com/watch?v=o0rOaN5uo64)
  - Awesome YouTube video on subgradients and subderivatives.
  - 劣勾配/劣微分について解説したYouTube動画．
### 70. [Lipschitz Continuity | Lipschitz Condition](https://www.youtube.com/watch?v=P-OFTp3BPis) 
  - Awesome YouTube video on Lipschitz continuity.
  - リプシッツ連続について解説したYouTube動画．
### 71. 🗾[リプシッツ連続とは～定義と性質・他の連続性との関係など～](https://mathlandscape.com/lipschitz/)
  - リプシッツ連続の定義や例，性質，その他の連続性との関連性について解説した記事．
### 72. [Lagrange Multipliers](https://www.youtube.com/watch?v=5-CUqogfPLY)
  - Awesome YouTube video on Lagrange multipliers.
  - ラグランジュの未定乗数法について解説したYouTube動画．
### 73. [Understanding Lagrange Multipliers Visually](https://www.youtube.com/watch?v=5A39Ht9Wcu0)
  - Awesome YouTube video visualizing the concept of Lagrange multipliers.
  - ラグランジュの未定乗数法について視覚的に解説したYouTube動画．
### 74. 🗾[ラグランジュの未定乗数法の気持ち【条件付き極値問題】](https://www.youtube.com/watch?v=vAwqZmwf4W8)
  - ヨビノリによるラグランジュの未定乗数法についての解説動画．図形的意味についての解説を含む．
### 75. 🗾[制約付き最適化問題(KKT条件/ラグランジュ未定乗数法)](https://www.youtube.com/watch?v=bdWTCq98H5c)
  - ヨビノリによるラグランジュの未定乗数法についての解説動画．KKT条件（不等式制約の場合の解法）についての解説を含む．
### 76. 🗾[ラグランジュの未定乗数法とは～意味と証明～](https://mathlandscape.com/lagrange-multiplier/)
  - ラグランジュの未定乗数法の意味，定理とその証明を解説した記事．

## Awesome-Gradient Descent (勾配降下法)
### 77. 🌟[Gradient descent, how neural networks learn | Deep Learning Chapter 2](https://youtu.be/IHZwWFHWa-w?si=zRN94_SPD4hrQUUI)
  - Awesome explanation of gradient descent in deep learning by 3Blue1Brown.
  - 3Blue1Brownによる，深層学習における勾配降下法についての解説．
### 78. [Optimization for Deep Learning (Momentum, RMSprop, AdaGrad, Adam)](https://youtu.be/NE88eqLngkg?si=qSmU5hpaeYiUtEZw)
  - Awesome explanation of the various online learning methods used in deep learning.
  - 深層学習に用いられる様々なオンライン学習手法についての解説．
### 79. [Mini Batch Gradient Descent (C2W2L01)](https://www.youtube.com/watch?v=4qJaSmvhxi8)
  - Awesome YouTube video by Andrew Ng explaining mini-batch gradient descent.
  - Andrew Ngによる，ミニバッチ勾配降下法について解説したYouTube動画.
### 80. [Understanding Mini-Batch Gradient Descent (C2W2L02)](https://www.youtube.com/watch?v=-_4Zi8fCZO4)
  - The second YouTube video by Andrew Ng explaining mini-batch gradient descent.
  - Andrew Ngによる，ミニバッチ勾配降下法について解説したYouTube動画の２本目.

# 📚 Resources（学習リソース）
## Awesome-slides（スライド）
### 81. 🌟[Online Convex Optimization and Its Surprising Applications](https://groups.oist.jp/sites/default/files/imce/u129210/mlss/Lecture_slide/MLSS2024_Francesco_Orabona.pdf)
  - Awesome slides from MLSS2024 by Orabona on online convex optimization algorithms such as OGD and OMD, and their applications to other fields. The content is quite mathematical but beneficial.
  - MLSS2024における，OrabonaによるOGDやOMDといったオンライン凸最適化のアルゴリズムとその他分野への応用についてのスライド．かなり数学的な内容だが有益．
### 82. [Online Learning Methods for Big Data Analytics](http://www.mysmu.edu.sg/faculty/chhoi/libol/icdm14tuto/index.html)
  - Awesome tutorial presented at IEEE ICDM2014.
  - IEEE ICDM2014で発表されたチュートリアル講演．
### 83. [Learning Methods for Online Prediction Problems](https://users.cecs.anu.edu.au/~ssanner/MLSS2010/Bartlett1.pdf)
  - Awesome lecture materials from UC Berkeley covering topics from the expert aggregation problem to online convex optimization, with applications such as portfolio optimization.
  - UC Berkeleyにおける講義資料．エキスパート統合問題からオンライン凸最適化，応用としてポートフォリオ最適化までを扱っている．
### 84. [Follow the Leader: Theory and Applications](https://www.cs.ubc.ca/labs/lci/mlrg/slides/2019_summer_3_follow_the_leader.pdf)
  - Slides explaining Follow The Leader (FTL) and its derivative algorithms in online learning, along with their applications.
  - オンライン学習におけるFollow The Leader (FTL) やその派生アルゴリズム，そしてそれらの応用について解説したスライド．
### 85. 🗾[多腕バンディット問題の理論とアルゴリズム](https://ibisml.org/archive/ibis2014/ibis2014_bandit.pdf)
  - 確率的，および敵対的バンディット問題における，報酬最大化（リグレット最小化）のためのアルゴリズムを解説したスライド．
### 86.🗾[オンライン予測の理論と応用](https://www.lab2.kuis.kyoto-u.ac.jp/keisan-genkai/reports/2005/zentai_1/04-takimoto.pdf)
  - 機械学習プロフェッショナルシリーズ「オンライン予測」（後述）の著者でもある瀧本英二先生によるスライド．オンライン予測におけるエキスパート統合問題とその応用例を取り上げている．

## Awesome-Textbooks（書籍）
### 87. 🌟[Prediction, Learning, and Games](https://www.cambridge.org/core/books/prediction-learning-and-games/A05C9F6ABC752FAB8954C885D0065C8F)
  - The bible on online learning, focusing on regret minimization and game-theoretic approaches to sequential decision-making
  - リグレット最小化やゲーム理論を通じて逐次意思決定問題を扱う，オンライン学習のバイブル的書籍．
### 88. [Introduction to Online Convex Optimization](https://sites.google.com/view/intro-oco/)
  - Awesome book by Hazan that covers a wide range of topics in the theory of online convex optimization.
  - Hazanによる，オンライン凸最適化の理論に関する多様なトピックをカバーした入門書．
### 89. 🌟🗾[機械学習プロフェッショナルシリーズ 「オンライン予測」](https://www.kspub.co.jp/book/detail/1529229.html)
  - 著名な機械学習プロフェッショナルシリーズより，オンライン予測にフォーカスして書かれた一冊．エキスパート統合問題やオンライン凸最適化など，オンライン予測の主要な内容を一通り学べる．
### 90. 🗾[機械学習プロフェッショナルシリーズ 「オンライン機械学習」](https://www.kspub.co.jp/book/detail/1529038.html)
  - 同じく機械学習プロフェッショナルシリーズより，オンライン機械学習を取り上げた一冊（出版は「オンライン予測」よりも前）．オンライン予測を含む，より広範な内容を学べる．「オンライン予測」よりも平易．
### 91. 🗾[機械学習プロフェッショナルシリーズ 「バンディット問題の理論とアルゴリズム」](https://www.kspub.co.jp/book/detail/1529175.html)
  - 同じく機械学習プロフェッショナルシリーズより．バンディット問題におけるリグレット解析や応用例などをより専門的に扱っている．

## Videos（動画）
### 92. 🌟[An introduction to regret analysis: environment models and best-of-both-worlds](https://youtu.be/pCER8iuTdR4?si=XAL6lP5tj0mMf8yp)
  - Awesome introduction on online learning, regret analysis, and best-of-both-worlds algorithms in the Machine Learning Summer School 2024.
  - オンライン学習，リグレット解析，Best-of-both-worldsアルゴリズムについてのMachine Learning Summer School 2024での講演．
### 93. [Predict with online prediction in Vertex AI](https://youtu.be/TEE7uUbXWDY?si=nHXMfZyTb13KpmWD)
  - Awesome tutorial on how to make predictions on tabular datasets with online prediction in Vertex AI. [GitHub Link](https://github.com/rafaello9472/c4ds/tree/main/Predict%20with%20online%20prediction%20in%20Vertex%20AI)
  - GoogleのVertex AIを用いて表形式のデータに対してオンライン予測を行う方法についてのチュートリアル．[GitHub Link](https://github.com/rafaello9472/c4ds/tree/main/Predict%20with%20online%20prediction%20in%20Vertex%20AI)
### 94. ["Online" prediction vs "batch" prediction in machine learning](https://youtu.be/DnmWTIeQ7PM?si=Mg8xcbWXyzlP3vLY)
  - Awesome explanation by Chip Huyen on the difference between online prediction and more common batch prediction and their applications.
  - Chip Huyenによる，オンライン予測と馴染み深いバッチ予測との違いやそれらの応用例についての短い解説．
### 95. [ML Drift: Identifying Issues Before You Have a Problem](https://youtu.be/uOG685WFO00?si=7_ti70FDTD-B5tbO)
  - Awesome presentation by Amy Hodler on ML drifts and how to fix them. [Blog](https://www.fiddler.ai/blog/drift-in-machine-learning-how-to-identify-issues-before-you-have-a-problem)
  - Amy Hodlerによる，MLドリフトやその解決方法についてのプレゼンテーション．[ブログ](https://www.fiddler.ai/blog/drift-in-machine-learning-how-to-identify-issues-before-you-have-a-problem)

## Articles（記事）
### 96. [What is Online Machine Learning?](https://medium.com/value-stream-design/online-machine-learning-515556ff72c5)
  - A blog post explaining the concept of online machine learning.
  - オンライン学習のコンセプトについて解説したブログ記事．
### 97. [Anomalies detection using River](https://medium.com/spikelab/anomalies-detection-using-river-398544d3536)
  - A blog post explaining anomaly detection using River, including practical code examples.
  - Riverを用いた異常検知について，実際のコードを交えて解説したブログ記事．
### 98. 🌟🗾[私のブックマーク「オンライン学習」](https://www.ai-gakkai.or.jp/resource/my-bookmark/my-bookmark_vol30-no5/)
  - 人工知能学会誌の連載「私のブックマーク」でオンライン学習を特集した際の記事．オンライン学習に関するサーベイやチュートリアル，関連学会，関連ライブラリをまとめている．
### 99. 🗾[私のブックマーク「多腕バンディット問題」](https://www.ai-gakkai.or.jp/resource/my-bookmark/my-bookmark_vol31-no5/)
  - 同じく「私のブックマーク」より，多腕バンディット問題を特集した回の記事．逐次的な意思決定であるバンディット問題に関するチュートリアルや関連学会，関連ライブラリ，重要論文をまとめている．
### 100. [Deus Ex Machina「Online learning and online prediction（オンライン学習とオンライン予測について）」](https://deus-ex-machina-ism.com/?p=17082)
  - Good for understanding the confusing differences between online learning and online prediction, and for gaining an overview of their respective scopes.
  - 混同しやすいオンライン学習とオンライン予測の違いを知り，それぞれの範囲を概観するのに良い．
### 101. [Deus Ex Machina「Overview of online forecasting technology and various applications and implementations（オンライン予測技術の概要と様々な適用事例と実装例）」](https://deus-ex-machina-ism.com/?p=53594)
  - It introduces algorithms, libraries, applications, and suitable books for learning used in online prediction.
  - オンライン予測で使用されるアルゴリズム，ライブラリ，応用例，学習に適した書籍が紹介されている．
