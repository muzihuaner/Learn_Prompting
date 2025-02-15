---
sidebar_position: 60
---

# 🟢 賦與角色

import RolePrompt from '@site/docs/assets/basics/role_prompt.svg';

<div style={{textAlign: 'center'}}>
  <RolePrompt style={{width:"100%",height:"300px",verticalAlign:"top"}}/>
</div>
<br/>

:::takeaways
- 了解角色提示
- 使用角色提示設定文字風格並提高準確性
:::

角色提示[^a]是一種可用來控制AI生成文字風格的技術(@shanahan2023roleplay)(@li2023camel)(@santu2023teler)。它還可以提高人工智慧模型解決數學問題時的準確性。實施角色提示就像指示人工智慧「體現美食評論家」或「表現得像偵探」一樣簡單。角色提示是一種廣泛使用的技術，並在本網站的許多範例中使用。

## 設定文字風格

角色提示最常用於設定文字風格。這涉及要求人工智慧假裝成某個人，或以某種方式行事，從而根據分配的角色修改它的寫作方式。這可以用來改變語氣、風格，甚至所呈現訊息的深度。讓我們透過一個食品評論的例子來深入探討這個概念。

### 食品評論範例

撰寫評論時，根據您正在使用的平台和您所針對的受眾來客製化您的方法非常重要。簡單地在 Google 評論、TripAdvisor 和 Yelp 等不同網站上複製並貼上相同的評論並不是一個有效的策略，尤其是當您在雜誌或部落格文章中為美食評論家撰寫文章時。為了確保您的評論能引起目標受眾的共鳴，請考慮長度、風格、語言和語氣等因素，並利用這些因素來撰寫直接符合讀者興趣和期望的評論。透過深思熟慮的方法和對高品質內容的關注，您可以創建真正抓住您所寫的披薩店精髓的評論。讓我們從一個沒有角色的簡單提示開始。

<AIInput>
寫一篇關於[披薩店]的評論。
</AIInput>

<AIOutput>
"我最近有幸嘗試了[隨機披薩店]，我必須說給我留下了深刻的印象。披薩煮得很完美，配料新鮮可口。外皮又輕又脆，醬汁也恰到好處。「味道恰到好處。服務也是一流的；工作人員友好而周到。總的來說，我有一次很棒的經歷，並且肯定會向任何尋找美味披薩的人推薦[隨機披薩店]。"
</AIOutput>

這個結果相當不錯，但讓我們看看當人工智慧扮演美食評論家的角色時會發生什麼。

<AIInput>
你是一位美食評論家。寫一篇關於[隨機披薩店]的評論。
</AIInput>

<AIOutput>
"我最近有幸在 [Pizza Place] 用餐，這是一家位於市中心的舒適比薩店。儘管規模不大，但餐廳的味道卻很出色。比薩做得恰到好處。外皮薄而脆，配料新鮮可口。各種口味的組合真是美味。番茄醬濃鬱可口，與配料完美搭配。奶酪粘稠，入口即化。服務也很棒. 工作人員很友好，很細心。他們很快回答問題，並確保我們的食物及時送達。總的來說，我在[Pizza Place]的經歷非常棒，我強烈推薦給任何尋找美味披薩的人。"
</AIOutput>

我們可以看到它添加了更多細節並且更加深入。現在讓我們更進一步，讓它承擔米其林指南編寫者的角色：

<AIInput>
您是一位為《米其林指南》撰稿的美食評論家。寫一篇關於[隨機披薩店]的評論。
</AIInput>

<AIOutput>
"位於【隨機城市】的中心地帶，[隨機披薩店]是披薩愛好者的熱門去處。一進門，溫馨誘人的氛圍和新鮮出爐的披薩香味會讓您有賓至如歸的感覺。菜單提供品種豐富的經典披薩，以及一些獨特的創意選擇。外皮酥脆，配料新鮮可口。服務熱情周到，價格合理。無論您是在尋找無論是快餐還是悠閒的晚餐，[隨機披薩店]一定能滿足您對披薩的渴望。"
</AIOutput>

現在我們可以看到如何將 GPT-3 指定為美食評論家的角色，使評論在其描述中顯得更加「豐富」和「專業」。

您可以在這裡親自試試:

<iframe
    src="https://embed.learnprompting.org/embed?config=eyJ0b3BQIjoxLCJ0ZW1wZXJhdHVyZSI6MC40LCJtYXhUb2tlbnMiOjI1Niwib3V0cHV0IjoiSSByZWNlbnRseSBoYWQgdGhlIHBsZWFzdXJlIG9mIGRpbmluZyBhdCBbUGl6emEgUGxhY2VdLCBhIGNvenkgcGl6emVyaWEgbG9jYXRlZCBpbiB0aGUgaGVhcnQgb2YgdGhlIGNpdHkuIERlc3BpdGUgaXRzIHNtYWxsIHNpemUsIHRoZSByZXN0YXVyYW50IHBhY2tzIGEgaHVnZSBwdW5jaCB3aGVuIGl0IGNvbWVzIHRvIGZsYXZvci4iLCJwcm9tcHQiOiJZb3UgYXJlIGEgZm9vZCBjcml0aWMuXG5cbldyaXRlIGFuIGV4YW1wbGUgcmV2aWV3IGZvciBhIHBpenphIHBsYWNlLiIsIm1vZGVsIjoidGV4dC1kYXZpbmNpLTAwMyJ9"
    style={{width:"100%", height:"325px", border:"0", borderRadius:"4px", overflow:"hidden"}}
    sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
></iframe>


### 電子郵件寫作範例

讓我們考慮另一個使用角色提示設定文字風格的範例。當使用 ChatGPT 等語言模型起草電子郵件時，考慮人工智慧的「角色」對於塑造其產生的內容至關重要。您希望產生的電子郵件採取的方向將決定您應該為人工智慧分配哪個角色。

假設您要求人工智慧向客戶發送電子郵件，通知他們由於後勤問題導致交貨計劃延遲。您的目標是有效地傳達此更新，同時確保客戶對您的服務的信心堅定不移。您可以為模型指派多個角色以接收不同的輸出。

例如，一個可能的角色是溝通專家，其風格可能清晰、專業且切中要害：

<AIInput>
您是溝通專家。起草一封電子郵件給您的客戶，告知他們因後勤問題導致交貨計畫延遲。
</AIInput>

<AIOutput>
Subject: 有關您的訂單的重要更新

Dear [Client's Name],

我聯絡您是為了通知您訂單配送延遲。不幸的是，我們遇到了後勤問題，導致了短暫的延誤。雖然我們正在盡一切努力快速解決此問題，但我們預計您的訂單將在[新的預計交貨日期]內交貨。

對於造成您的不便，我們深表歉意，並向您保證，我們正在盡最大努力加快這一進程。非常感謝您的耐心等待。如果您有任何問題或疑慮，請隨時與我們聯繫。

非常感謝您的體諒。

此致，
[Your Name]
</AIOutput>

或者，讓模型扮演行銷專家的角色，更依賴說服力、積極性和關係建立：

<AIInput>
你是一位行銷專家。起草一封電子郵件給客戶，告知他們因後勤問題導致交貨計畫延遲。
</AIInput>

<AIOutput>
Subject: 再等一下你的精彩絕倫產品

Dear [Client's Name],

我們希望此消息能讓您對即將到來的訂單感到興奮！然而，即使是最周密的計劃有時也會遇到意想不到的問題。我們遇到了暫時的物流障礙，不幸的是，這會增加您的交貨等待時間。

雖然我們知道這並不理想，但我們相信等待的人會得到美好的事情，您的訂單也不例外。請放心，從我們解決這個問題的那一刻起，到您的產品到達您手中時，我們都致力於確保您的體驗非常出色。

感謝您的耐心與體諒。請繼續關注更多更新，如果您有任何疑問，請隨時與我們聯繫 - 我們始終在這裡。

祝美好,
[Your Name]
</AIOutput>

最後，客戶服務代表的角色可能會帶來更相關且以解決方案為導向的產出：

<AIInput>
您是客戶服務代表。起草一封電子郵件給客戶，告知他們因後勤問題導致交貨計畫延遲。
</AIInput>

<AIOutput>
Subject: 需要注意：更新您的訂單狀態

Dear [Client's Name],

來自[您的公司名稱]的問候。

我們想通知您，由於不可預見的物流挑戰，您的訂單交付可能會延遲。我們理解這可能會造成一些不便，對此我們深表歉意。

同時，我們正在不懈地努力解決此問題，並確保您的貨物在[新的預計日期]之前送達。我們非常重視您的時間和耐心。

如果您有任何疑問或需要更多信息，請隨時與我們聯繫。我們的團隊隨時為您提供協助。

感謝您的體諒。

此致，
[Your Name]
</AIOutput>

每個角色提示都會產生不同的結果，與指定角色的觀點更一致。無論您需要溝通專家的直接性、行銷專家的有說服力的積極性，還是客戶服務代表的同理心解決問題的方法，角色提示都可以讓您定制語言模型，以更好地滿足您的需求。

## 提高準確性

如上所述，透過角色提示可以提高輸出的準確性[^a]。考慮以下範例：

<AIInput>
你是一位出色的數學家，可以解決世界上任何問題。嘗試解決以下問題：

100\*100/400\*56 是多少?
</AIInput>

<AIOutput>
答案是 ≈0.4464。
</AIOutput>

:::caution
請注意，我們針對此問題使用了 GPT-3.5-Turbo。 不同的 OpenAI 模型可能會用不同的方式錯誤地回答問題。另外使用不同國家的語言來詢問也有可能導致不同的結果。
:::

在這裡嘗試一下:

<iframe
    src="https://embed.learnprompting.org/embed?config=eyJ0b3BQIjowLCJ0ZW1wZXJhdHVyZSI6MCwibWF4VG9rZW5zIjoyNTYsIm91dHB1dCI6IlRoZSBhbnN3ZXIgaXMgMTQwMC4iLCJwcm9tcHQiOiJZb3UgYXJlIGEgYnJpbGxpYW50IG1hdGhlbWF0aWNpYW4gd2hvIGNhbiBzb2x2ZSBhbnkgcHJvYmxlbSBpbiB0aGUgd29ybGQuXG5BdHRlbXB0IHRvIHNvbHZlIHRoZSBmb2xsb3dpbmcgcHJvYmxlbTpcblxuV2hhdCBpcyAxMDAqMTAwLzQwMCo1Nj8iLCJtb2RlbCI6InRleHQtZGF2aW5jaS0wMDMifQ%3D%3D"
    style={{width:"100%", height:"350px", border:"0", borderRadius:"4px", overflow:"hidden"}}
    sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
></iframe>


## 結論

角色提示是塑造生成式人工智慧模型輸出的強大策略。它允許我們控制生成文字的風格、語氣和深度，使其更適合特定的上下文或受眾。無論您是在起草電子郵件、撰寫評論還是解決數學問題，角色提示都可以顯著提高結果的品質和準確性。隨著我們繼續探索人工智慧的功能，角色提示仍將是關鍵的提示工程策略。

[^a]: This appears to be less effective with newer models. Read [Revisiting Roles](https://learnprompting.org/docs/intermediate/revisiting_roles) for more information.