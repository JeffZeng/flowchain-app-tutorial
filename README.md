Flowchain 物聯網中文教材

# Chapter1. Flowchain 簡介

如果要「簡單介紹」這是什麼技術，還真的不簡單。所以，不如根據這份中文教材，體驗 Flowchain 在物聯網開發上的創新。

## Flowchain 起源

Flowchain 發源自 [WoT.City](https://wotcity.com) 計畫，WoT 是 Web of Things 的縮寫。要把 Flowchain 說清楚，就必須把 Web of Things 講明白。你可以在[這裡](https://www.w3.org/WoT/IG/wiki/Implementations)找到一份 Web of Things Implementations 的清單，這份清單整理 W3C Web of Things 的相關計畫。

也就是說，WoT.City 是 W3C Web of Things (WoT) 的一個計畫，它也是一個開源項目，也是 WoT 的技術。這就是故事的開始。

WoT.City 主要在處理 *Connectivity*，例如：WebSocket、CoAP 與 Thing Description 等。WoT.City 是 Connecitivity Layer，目前它已經打包成  [wotcity.io](https://www.npmjs.com/package/wotcity.io) 模組，但是你不需要直接使用 wotcity.io 模組。

wotcity.io 被封裝為 [devify-server](https://github.com/DevifyPlatform/devify-server) 模組，devify-server 是一份 IoT server boilerplate，這是什麼呢？簡單說，就是一套給 IoT 用的伺服器程式模板，你可以用 devify-server 很容易寫出一個「負責收集感測器資料」的 IoT server。這套 IoT server 可以執行在 Desktop、Server 或 IoT device 上，它使用的是 Nodoe.js 技術，這表示只要有 Node.js 執行環境的硬體，都可以成為 devify-server 的執行環境。

架構上，devify-server 封裝了 wotcity.io，並且負責 Event Handling、Broker Server 與 Serverless 的角色。不過，你也不需要學習 devify-server 的程式設計。devify-server 再被封裝了，成為 *Flowchain* 技術。

Flowchain 帶來一些好消息，其中之一就是帶來 Flow-Based Programming 的物聯網開發模式。


