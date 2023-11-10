# 書籍『確率的シミュレーション』サンプルコード

### 書籍情報
大久保 潤 著, 『確率的シミュレーション』, 森北出版(2023)のサンプルコードを掲載しています。  
[出版社のページ: https://www.morikita.co.jp/books/mid/009721](https://www.morikita.co.jp/books/mid/009721)

（注意）「理解を深めるために参考になれば」という意図で作成しています。バグ等含まれる可能性もあります。勉強のためのみに利用してください。

### コードについて
- 「`.ipynb`」形式のものを掲載しています。なお、１つのセルのみにまとめてあるため、コードの部分をコピーして「`.py`」形式で保存すれば、コマンドラインでPythonのコードとして実行できます。
- Google Colaboratoryにそのままアップロードしても動作します。

***
[`chap3_Gillespie_algorithm.ipynb`](https://github.com/junohkubo/stoc_simu_book/blob/main/chap3_Gillespie_algorithm.ipynb)

ギレスピーアルゴリズムのコード。第3章のアルゴリズム3に対応。Lotka-Volterra系に対して、１つのサンプルパスを生成する。図3.7のような図を描画できる。
***
[`chap3_next_reaction_algorithm.ipynb`](https://github.com/junohkubo/stoc_simu_book/blob/main/chap3_next_reaction_algorithm.ipynb)

ネクストリアクション法のコード。第3章のアルゴリズム4に対応。Lotka-Volterra系に対して、１つのサンプルパスを生成する。これも図3.7のような図を描画できる。

***
[`chap5_simulation_for_SDE.ipynb`](https://github.com/junohkubo/stoc_simu_book/blob/main/chap5_simulation_for_SDE.ipynb)

確率微分方程式に対するシミュレーションのコード。第5章のアルゴリズム5に対応。Lotka-Volterra系に対して、１つのサンプルパスを生成する。図5.10(b)のような図を描画できる。

なお、このコードはアルゴリズムとの対応を意識して、わかりやすさを優先したものである。実際には乱数を一度に生成してしまったり、時刻刻みを表す配列を先に用意する書き方のほうがPythonらしい。最適なものではないが、少し改良したものを以下に掲載しておく。

[`chap5_simulation_for_SDE_rapid.ipynb`](https://github.com/junohkubo/stoc_simu_book/blob/main/chap5_simulation_for_SDE_rapid.ipynb)

***
[`chap7_Gillespie_Bayes_estimation.ipynb`](https://github.com/junohkubo/stoc_simu_book/blob/main/chap7_Gillespie_Bayes_estimation.ipynb)

ギレスピーアルゴリズムでデータを生成し、ベイズ推定により速度定数を推定するコード。第7章の7.3節の記載に対応。Lotka-Volterra系に対して、パラメータ c<sub>1</sub> を推定する。図7.7のような図を描画できる。

***
[`chap8_particle_filter.ipynb`](https://github.com/junohkubo/stoc_simu_book/blob/main/chap8_particle_filter.ipynb)

確率微分方程式のシミュレーションでデータを生成し、粒子フィルタでひとつの速度定数を推定するコード。第8章の8.4節の記載に対応。Lotka-Volterra系に対する確率微分方程式を考えて、パラメータ c<sub>3</sub> を推定する。図8.7のような図を描画できる。
