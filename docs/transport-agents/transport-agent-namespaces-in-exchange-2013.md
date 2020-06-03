---
title: Exchange 2013 のトランスポート エージェントの名前空間
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c40788e-c182-4502-9202-206e6aaa53f8
description: Exchange 2013 用のカスタムトランスポートエージェントを作成するために使用できる .NET Framework のクラスとメンバーについて説明します。
ms.openlocfilehash: fc2d9108c910a730bb48c5be028797f0f15ad4ad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461794"
---
# <a name="transport-agent-namespaces-in-exchange-2013"></a>Exchange 2013 のトランスポート エージェントの名前空間

Exchange 2013 用のカスタムトランスポートエージェントを作成するために使用できる .NET Framework のクラスとメンバーについて説明します。
  
**製品:** Exchange Server 2013 
  
この記事では、Exchange Server 2013 のトランスポートエージェントの作成に使用できる参照情報を含む名前空間について説明します。 さらに、トランスポート パイプラインを通過する電子メール メッセージの読み取りおよび変更をトランスポート エージェントで行うために使用できるクラスについても説明します。
  
## <a name="transport-agent-class-library"></a>トランスポート エージェントのクラス ライブラリ

次の名前空間には、トランスポート エージェントの作成と拡張に使用できる型が含まれています。

**表1.NET Framework の名前空間**

|**名前空間**|**説明**|
|:-----|:-----|
|[Microsoft のデータ交換](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.aspx) <br/> |データと構成の例外を指定する型が含まれています。  <br/> |
|[Microsoft. データ共有](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Common.aspx) <br/> |ローカライズとエラー処理をサポートする型が含まれています。  <br/> |
|[ContentTypes を行います。](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |iCalendar データの読み取りと書き込みを可能にする型が含まれています。  <br/> |
|[ContentTypes (. Tnef)](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |TNEF データの読み取りと書き込みを可能にする型が含まれています。  <br/> |
|[ContentTypes (. vCard)](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |vCard データの読み取りと書き込みを可能にする型が含まれています。  <br/> |
|[Microsoft によるデータのグローバリゼーション](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Globalization.aspx) <br/> |ローカライズされたコンテンツを生成するカルチャと文字セットの操作を可能にする型が含まれています。  <br/> |
|[Microsoft. データの Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |MIME データの読み取りと書き込みを可能にする型が含まれています。  <br/> |
|[(データの場合)](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |MIME データのエンコードとデコードを可能にする型が含まれています。  <br/> |
|[Microsoft のデータ変換器](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |各種のテキスト形式によるデータの読み書きと、それらの形式間での変換を可能にする型が含まれています。  <br/> |
|[Microsoft Exchange.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.aspx) <br/> |トランスポート パイプラインに関するルーティング情報、ホスト情報、およびドメイン情報へのアクセスを可能にする型が含まれています。  <br/> |
|[その後、配送。](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.aspx) <br/> |Exchange 2013 配信エージェントの拡張機能をサポートする型が含まれています。  <br/> |
|[その後、電子メール](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.aspx) <br/> |電子メール メッセージの読み取り、書き込み、および変更をサポートする型が含まれています。  <br/> |
|[Microsoft Exchange Server のルーティング](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.aspx) <br/> |Exchange 2013 トランスポートルーティングの動作の拡張をサポートする型が含まれています。  <br/> |
|[その後、Smtp (トランスポート)](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.aspx) <br/> |Exchange 2013 トランスポート SMTP の動作の拡張をサポートする型が含まれています。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange のトランスポート エージェント](transport-agents-in-exchange-2013.md)   
- [Exchange 2013 におけるトランスポート エージェントの概念](transport-agent-concepts-in-exchange-2013.md) 
- 
  [Exchange 用 EWS リファレンス](https://msdn.microsoft.com/library/6eddd052-f59f-45b4-b846-7e53d4d7eb16%28Office.15%29.aspx)
- [Exchange 2013 のエージェント構成ファイルの要素](agents-configuration-file-elements-for-exchange-2013.md)
    

