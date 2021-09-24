---
title: Exchange 2013 のトランスポート エージェントの名前空間
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5c40788e-c182-4502-9202-206e6aaa53f8
description: 2013 .NET Frameworkのカスタム トランスポート エージェントを作成するために使用できるカスタム トランスポート エージェントのクラスとメンバー Exchangeします。
ms.openlocfilehash: 076ddb8e2ccbdfa195a68aca6b296337a2876b55
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537131"
---
# <a name="transport-agent-namespaces-in-exchange-2013"></a>Exchange 2013 のトランスポート エージェントの名前空間

2013 .NET Frameworkのカスタム トランスポート エージェントを作成するために使用できるカスタム トランスポート エージェントのクラスとメンバー Exchangeします。
  
**製品:** Exchange Server 2013 
  
この記事では、2013 年のトランスポート エージェントの作成に使用できる参照情報を含む名前空間Exchange Serverします。 さらに、トランスポート パイプラインを通過する電子メール メッセージの読み取りおよび変更をトランスポート エージェントで行うために使用できるクラスについても説明します。
  
## <a name="transport-agent-class-library"></a>トランスポート エージェントのクラス ライブラリ

次の名前空間には、トランスポート エージェントの作成と拡張に使用できる型が含まれています。

**表 1..NET Framework名前空間**

|**名前空間**|**説明**|
|:-----|:-----|
|[Microsoft。Exchange。データ](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.aspx) <br/> |データと構成の例外を指定する型が含まれています。  <br/> |
|[Microsoft。Exchange.Data.Common](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Common.aspx) <br/> |ローカライズとエラー処理をサポートする型が含まれています。  <br/> |
|[Microsoft。Exchange。Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |iCalendar データの読み取りと書き込みを可能にする型が含まれています。  <br/> |
|[Microsoft。Exchange。Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |TNEF データの読み取りと書き込みを可能にする型が含まれています。  <br/> |
|[Microsoft。Exchange。Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |vCard データの読み取りと書き込みを可能にする型が含まれています。  <br/> |
|[Microsoft。Exchange。Data.Globalization](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Globalization.aspx) <br/> |ローカライズされたコンテンツを生成するカルチャと文字セットの操作を可能にする型が含まれています。  <br/> |
|[Microsoft。Exchange。Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |MIME データの読み取りと書き込みを可能にする型が含まれています。  <br/> |
|[Microsoft。Exchange。Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |MIME データのエンコードとデコードを可能にする型が含まれています。  <br/> |
|[Microsoft。Exchange。Data.TextConverters](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |各種のテキスト形式によるデータの読み書きと、それらの形式間での変換を可能にする型が含まれています。  <br/> |
|[Microsoft。Exchange。Data.Transport](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.aspx) <br/> |トランスポート パイプラインに関するルーティング情報、ホスト情報、およびドメイン情報へのアクセスを可能にする型が含まれています。  <br/> |
|[Microsoft。Exchange。Data.Transport.Delivery](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.aspx) <br/> |2013 年の配信エージェントの拡張をサポートExchangeが含まれる。  <br/> |
|[Microsoft。Exchange。Data.Transport.Email](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.aspx) <br/> |電子メール メッセージの読み取り、書き込み、および変更をサポートする型が含まれています。  <br/> |
|[Microsoft。Exchange。Data.Transport.Routing](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.aspx) <br/> |2013 年のトランスポート ルーティング動作の拡張をサポートするExchangeが含まれています。  <br/> |
|[Microsoft。Exchange。Data.Transport.Smtp](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.aspx) <br/> |2013 トランスポート SMTP 動作の拡張をサポートするExchangeが含まれています。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange のトランスポート エージェント](transport-agents-in-exchange-2013.md)   
- [Exchange 2013 におけるトランスポート エージェントの概念](transport-agent-concepts-in-exchange-2013.md) 
- 
  [Exchange 用 EWS リファレンス](https://msdn.microsoft.com/library/6eddd052-f59f-45b4-b846-7e53d4d7eb16%28Office.15%29.aspx)
- [Exchange 2013 のエージェント構成ファイルの要素](agents-configuration-file-elements-for-exchange-2013.md)
    

