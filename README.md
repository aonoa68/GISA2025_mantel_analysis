# GISA2025 Mantel Proximity Analysis

このリポジトリは、地理的近接性と感情・文化的指標の関連を Mantel 検定を用いて分析するための Jupyter Notebook とデータセットを収録しています。  
2025年度 地理情報システム学会（GISA 2025）発表「場所と感情の地理的相関分析」に関連しています。

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17432950.svg)](https://doi.org/10.5281/zenodo.17432950)

---

## 📂 構成

```

GISA2025_mantel_analysis/
├─ W4_2025_GISA_mantel_proximity_analysis.ipynb   # 分析ノートブック
├─ pivot_table_id.csv                              # 入力データ
├─ README.md                                       # 本ファイル
└─ requirements.txt                                # 環境依存パッケージ（任意）

````

---

## 🧠 研究概要

- **目的**：地域間の感情・文化的特徴の類似性が地理的距離とどの程度対応しているかを検証する。  
- **手法**：
  - 距離行列：緯度経度から算出した地理距離（例：Haversine距離）
  - 特徴行列：感情スコアまたは文化特徴のピボットテーブル（`pivot_table_id.csv`）
  - 相関解析：Mantel検定（permutation test, Pearson距離）

---

## ⚙️ 実行方法

1. **環境をセットアップ**
   ```bash
   pip install -r requirements.txt
   ```

2. **ノートブックを実行**

   ```bash
   jupyter notebook W4_2025_GISA_mantel_proximity_analysis.ipynb
   ```

3. **Google Colabで開く**
   [Open in Colab](https://colab.research.google.com/github/aonoa68/GISA2025_mantel_analysis/blob/main/W4_2025_GISA_mantel_proximity_analysis.ipynb)

---

## 📊 データ説明

| ファイル名                                          | 内容               | 備考                                      |
| ---------------------------------------------- | ---------------- | --------------------------------------- |
| `pivot_table_id.csv`                           | 各地点の感情・文化的特徴の集計値 | 行＝地点、列＝特徴量                              |
| `W4_2025_GISA_mantel_proximity_analysis.ipynb` | Mantel検定の実装と可視化  | Python (pandas, scikit-bio, matplotlib) |

---

## 🧩 依存パッケージ

```txt
pandas
numpy
scipy
scikit-bio
geopandas
matplotlib
```

---

## 🪪 ライセンス

- **Source code (e.g., .ipynb, .py)**: Licensed under the **MIT License**. See [`LICENSE`](./LICENSE).
- **Data and documentation (e.g., CSVs, README, figures)**: Licensed under **CC BY 4.0**. See [`LICENSE_DATA`](./LICENSE_DATA).

### Attribution format (for data/docs)
Onohara, A. (2025). *GISA2025 Mantel Proximity Analysis* (CC BY 4.0). [https://github.com/aonoa68/GISA2025_mantel_analysis](https://github.com/aonoa68/GISA2025_mantel_analysis)

---

## 📘 引用情報

小野原彩香, 大内啓樹（2025）「場所の感情地図－テキスト埋め込みと空間的近接性による環境段階モデルの検証－」地理情報システム学会（GISA 2025）ポスター発表
`Phase-Dependent Emotion Maps of Place A Mantel Analysis Using Text Embeddings and Spatial Proximity`
