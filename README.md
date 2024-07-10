This repo contains corrections to transcripts / dictionaries in datasets that I've edited as part of my work.

## CSS10 Spanish
- Cleaned invalid characters: `bÅ“uf` to `bœuf`.
- `Vds.` normalized to `Ustedes`.
- `Yquién` to `Y quién`.
- `Schöenbrunn` to `Schönbrunn`.
- Split joined words like `unaJunta`. 

## AISHELL-3 test set
The transcripts are raw Hanzi that humans read, and the pinyin given is likely run through ASR. There are errors from 字 (0.02%) > audio (0.2%) > pinyin (2% estimated). When 字 and pinyin don't match, either:
1) Pinyin will be corrected, if the audio has mispronunciations: 南 lan2/nan1 > nan2, 东莞 wan3 > guan3, 哪儿 lang3 > nar3.
- Most rare characters are read wrongly e.g. 疃、歙、垤. In these cases the audio will not match the pinyin at all.
2) 字 will be corrected, if misreadings fit the context: 替 > 帮 bang1 我 wo3 or 累 lei3 计 > 积 ji1.
3) Nothing is corrected, if it's a common non-dictionary pronunciation: 友 you3 谊 yi2 (dictionary yi4) or 违 wei3 约 yue1 (dictionary wei2).

Further edits:
- Instances of 地 where it should be di4
- 轻声 allowed mostly: 招 zhao1 呼 hu5 but generally not allowed in the middle: 葡 pu2 萄 tao5 > tao2 酒 jiu3.
- 吗 = ma1, 嘛 = ma5
- 什么 changed to shen3 me5, even though dictionary says shen2 me5 (as this is how it's pronounced almost all the time)
- Impacted sandhi are corrected: 有 you3 > you2 什 shen3 么 or 菜谱 pu2 > pu3 有 you2 什 shen3 么 or 可 ke2 以 yi2 > yi3 理 li2 解 jie3.

## CMU Dictionary
corrected invalid pronunciations
