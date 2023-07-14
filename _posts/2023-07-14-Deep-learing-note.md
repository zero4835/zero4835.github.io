---
layout: post
title: Deep-Learing note
date: 2023-07-14
Author: Natsusaka
tags: [Deep-Learing, note]
comments: true
toc: true
--- 

專題的原因開始使用深度學習來做情緒分析。

### 深度學習(Deep-Learing)

機械學習的分支，為一種類人工神經網路架構，深度表示中間有很多層來工作並模擬神經的運作，是基於機械學習對資料進行學習的演算法，應用領域包括但不限於識別圖片、文字、聲音的日常場景，也常被用於任務的自動化例如自然語言處理(NLP)。

在使用深度學習前我已統計的方式來做情緒分.析:
1. 把輸入的文本斷詞
2. 根據NTUSD_traditional的情緒分析集pos.txt和neg.txt來統計各個斷詞是否出現其中

