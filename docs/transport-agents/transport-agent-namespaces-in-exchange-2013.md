---
title: Exchange 2013 のトランスポート エージェントの名前空間
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c40788e-c182-4502-9202-206e6aaa53f8
description: .NET Framework のクラスおよび Exchange 2013 のカスタムのトランスポート エージェントを作成するのに使用できるメンバーについて説明します。
ms.openlocfilehash: a8189ca9915312b64fefda3091f8f81e51271ad6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759262"
---
# <a name="transport-agent-namespaces-in-exchange-2013"></a>Exchange 2013 のトランスポート エージェントの名前空間

.NET Framework のクラスおよび Exchange 2013 のカスタムのトランスポート エージェントを作成するのに使用できるメンバーについて説明します。
  
**に適用されます:** Exchange Server 2013 
  
この資料では、Exchange Server 2013 のトランスポート エージェントを作成するのに使用できる参照情報が含まれている名前空間に関する情報を提供します。 読み取りおよびトランスポート パイプラインを通過する電子メール メッセージを変更するのには、トランスポート エージェントを使用するクラスについても説明します。
  
## <a name="transport-agent-class-library"></a>トランスポート エージェントのクラス ライブラリ

次の名前空間には、トランスポート エージェントの作成と拡張に使用できる型が含まれています。

**表 1 です。.NET Framework 名前空間**

|**名前空間**|**説明**|
|:-----|:-----|
|[Microsoft.Exchange.Data](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.aspx) <br/> |データと構成の例外を指定する型が含まれています。  <br/> |
|[Microsoft.Exchange.Data.Common](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Common.aspx) <br/> |ローカライズとエラー処理をサポートする型が含まれています。  <br/> |
|[Microsoft.Exchange.Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |iCalendar データの読み取りと書き込みを可能にする型が含まれています。  <br/> |
|[Microsoft.Exchange.Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |TNEF データの読み取りと書き込みを可能にする型が含まれています。  <br/> |
|[Microsoft.Exchange.Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |vCard データの読み取りと書き込みを可能にする型が含まれています。  <br/> |
|[Microsoft.Exchange.Data.Globalization](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Globalization.aspx) <br/> |ローカライズされたコンテンツを生成するカルチャと文字セットの操作を可能にする型が含まれています。  <br/> |
|[Microsoft.Exchange.Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |MIME データの読み取りと書き込みを可能にする型が含まれています。  <br/> |
|[Microsoft.Exchange.Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |MIME データのエンコードとデコードを可能にする型が含まれています。  <br/> |
|[Microsoft.Exchange.Data.TextConverters](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |各種のテキスト形式によるデータの読み書きと、それらの形式間での変換を可能にする型が含まれています。  <br/> |
|[Microsoft.Exchange.Data.Transport](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.aspx) <br/> |トランスポート パイプラインに関するルーティング情報、ホスト情報、およびドメイン情報へのアクセスを可能にする型が含まれています。  <br/> |
|[Microsoft.Exchange.Data.Transport.Delivery](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.aspx) <br/> |Exchange 2013 の配信エージェントの拡張機能をサポートする型が含まれています。  <br/> |
|[Microsoft.Exchange.Data.Transport.Email](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.aspx) <br/> |電子メール メッセージの読み取り、書き込み、および変更をサポートする型が含まれています。  <br/> |
|[Microsoft.Exchange.Data.Transport.Routing](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.aspx) <br/> |Exchange 2013 のトランスポートのルーティング動作の拡張機能をサポートする型が含まれています。  <br/> |
|[Microsoft.Exchange.Data.Transport.Smtp](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.aspx) <br/> |Exchange 2013 配送 SMTP の動作の拡張機能をサポートする型が含まれています。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange のトランスポート エージェント](transport-agents-in-exchange-2013.md)   
- [トランスポート エージェントの概念には、Exchange 2013](transport-agent-concepts-in-exchange-2013.md) 
- [Exchange のサーバー API への参照](http://msdn.microsoft.com/library/6eddd052-f59f-45b4-b846-7e53d4d7eb16%28Office.15%29.aspx)
- [Exchange 2013 のエージェント構成ファイルの要素](agents-configuration-file-elements-for-exchange-2013.md)
    

