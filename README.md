# 微積溯源/Introduction to Calculus

這個項目旨在提供一版經過精細排版和修訂的微積溯源，並同時研究使用XeLaTeX進行中文竪排的技術。

This project aims to provided a beautifully-typed and well-edited version of the book Introduction to Calculus, as well as exploring methods to typeset Chinese vertically with XeLaTeX. 

## 關於微積溯源/About the book Introduction to Calculus

微積溯源乃清代洋務運動之時傅蘭雅、華蘅芳所譯之微積分教科書。這本書由於開創性地翻譯了許多現今數學之專有名詞（如“函數”等），因此有將其整理出的價值。

Introduction to Calculus was a calculus textbook translated by John Fryer and Hua Hengfang during the [Self-Strengthening Movement](https://en.wikipedia.org/wiki/Self-Strengthening_Movement). This book is the origin of many math jargons in modern Chinese thus we believe it is worthy to be digitized.

## 關於本項目/About this project

本項目分爲兩個部分，一者爲整理和修訂文字（即校讎學相關），一者爲研究XeLaTeX竪排中文的技術。目前主要工作均由NSKernel獨自進行。由於NSKernel比較喜歡摸魚，所以進度上沒有任何保證，且文件都只是散落在整個項目內，請見諒。

This project is mainly about two specific jobs. One is to type and edit text; the other is to explore methods to typesetting Chinese vertically using XeLaTeX. Currently most of the project is maintained by NSKernel. Please note that NSKernel does not consider himself fully devoted into this project thus it is not guaranteed  of the progress of this project and the files might not be well-organized.

## 如何使用/貢獻本項目/How to use/contribute to this project

下載後請參照根目錄下的`微積溯源.tex`內的字體設定，找齊字體扔在根目錄下，然後拿XeLaTeX編譯即可。事實上，由於NSKernel懶惰的本質，編譯好的PDF文件也在repo裏，可自行取用。

After cloning your own copy of the project, grab the fonts according to the settings in `微積溯源.tex` and put them at the root of the source code, then compile it with XeLaTeX. However this project also comes with a precompiled PDF file in its repository which you may feel free to use.

本項目歡迎任何人貢獻，如果您有好的patch或者建議，可以直接提交pull request或提issue，我們可以一起討論並提升最終的文字與排版質量。

We welcome anyone to contribute. If you have a good patch or idea, just bring up a pull request or issue so we can discuss and improve the final quality of the text and the typesetting.

*貢獻者名單*：NSKernel（發起人，目前的項目維護者），[SiobaraIsara](https://github.com/SiobaraIsara)（優化了代碼）

*Contributors*: NSKernel (founder, maintainer), [SiobaraIsara](https://github.com/SiobaraIsara) (optimized the source code)

## 參考版PDF的字體選用

本項目儘量選用開源的字體，並且希望能採用舊字形的字體以確保閱讀準確美觀，因此正文採用了ButTaiwan的[源流明朝](https://github.com/ButTaiwan/genryu-font)。此字體基於韓文版的思源宋體，基本符合舊字形標準且通過圓滑邊角和調瘦字框使得其非常適合排印本項目。然而由於此字體主要還是爲台灣地區的情況考慮而設計修改，因此如果它的修改超過了舊字形的限度則我可能考慮fork一份過來保證穩定性。

This project uses opensource fonts at any possible place and aims to produce accurate and beautiful PDF using traditional font style. Thus, I chose the [Genryu-Mincho](https://github.com/ButTaiwan/genryu-font) in the text. The font is based on the Korean version of Source Han Serif and is basically compliant to the traditional font style. The font has smooth edges with a thinner design making it very suitable to typeset this project. However the font is intended to serve the Taiwan region and has modified to do so. So if the modifications are over what a *traditional font style* can be called then I might fork that repo to keep the stability of the produced PDF.

關於正文中公式的字體，由於尚未發現高質量穩定的开源楷体，因此采用了方正公司的方正楷体。此字體可免費商用，因此毋須擔心版權問題。如您仍希望使用開源字體，可自行替換編譯。

For the font in equations, I currently have no knowledge on a high-quality opensource Kai-style font so my choice is the FZKai from FounderType. The font is free and commercial-usage-allowed so there's no concern on copyright or anything. If you still insist on using an opensource alternative, you may replace it and recompile.

## 目前進度/Progress

文字上：目前已經排好了序，正文第一章進行了一半。
排版上：目前仍未能'''優雅'''地解決以下問題：`chapter`頁默認爲`plain`（我們想要`fancy`，目前通過在`chapter`命令下面直接插入`thispagestyle`解決）；左右footer設定分別爲章節名和小節名，然而在序言等沒有小節的地方，我們希望兩側都顯示章節名（目前考慮定義新的pagestyle，但是這也不算優雅吧）
代碼上：主代碼文件可以稱爲髒亂差的典範，基礎設定還需重新整頓，包括清除多餘設定和按類型整理其餘設定。

Text: Finished preface and working on chapter one. 
Typesetting: Still cannot solving the following issues '''elegantly''': the pagestyle of `chapter` page is `plain` (we want `fancy` and we are doing it by inserting `thispagestyle` command directly under the `chapter` command); we set the left and right footers as the chapter name and the section name, but places like the preface do not come with a section name (we are considering defining new pagestyle but we think that is not quite elegant).
Code: The main source file is basically a scrapyard with tons of settings need to be organized including cleaning up unnecessary settings.
