---
title: Exchange 2013 のトランスポート エージェントのコード サンプル
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 626345ec-918f-4d91-932f-e6ce92553ccb
description: 2013 で使用できるトランスポート エージェントのサンプルに関するExchangeします。
ms.openlocfilehash: 56334f661947cffceaf18eb257feeb6504a71ecb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545715"
---
# <a name="transport-agent-code-samples-for-exchange-2013"></a>Exchange 2013 のトランスポート エージェントのコード サンプル

2013 で使用できるトランスポート エージェントのサンプルに関するExchangeします。
  
**製品:** Exchange Server 2013
  
2013 年から 2013 年に含まれる API を使用してExchange Server機能を拡張するエージェントを開発できます。 この記事では、トランスポート動作をプログラムによって拡張する方法の学習に利用できるサンプル エージェントに関する情報について説明します。 サンプル エージェントには、各コンポーネントのソース コードが含まれています。 
  
次の表に、2013 年のサンプル エージェントExchange示します。
  
**表 1.トランスポート エージェントのサンプル**

|**サンプルの名前**|**説明**|
|:-----|:-----|
|[Exchange 2013: ウイルス対策トランスポート エージェントを作成する](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-6e544269) <br/> |このエージェントは [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) イベントと [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) イベントに応答し、受信メッセージをアウトプロセス サーバーに送信し、メッセージを非同期的に調べて変更されたバージョンを返します。  <br/> |
|[Exchange 2013: 帯域幅ログ トランスポート エージェントの作成](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) <br/> |このエージェントは [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) イベントと [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) イベントに応答し、指定された受信者の帯域幅使用量をキャプチャし、帯域幅の使用状況情報をテキスト ファイルに記録します。  <br/> |
|[Exchange 2013: 本文変換トランスポート エージェントを作成する](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) <br/> |このエージェントは、着信メッセージの形式を判断し、フィルター処理が必要かどうかを決定することで、電子メール メッセージのスクリプトをフィルターで除去します。フィルター処理が必要になる場合は、コンテンツを HTML に変換し、フィルターを適用してから元の形式に戻します。  <br/> |
|[Exchange 2013: SMTP ログ トランスポート エージェントを作成する](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-fc23dc33) <br/> |このエージェントは [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) イベントに応答し、メッセージをローカル ハード ディスク上のファイルに非同期的に記録します。  <br/> |
|[Exchange 2013: 送信者を一時的にブロックするトランスポート エージェントを作成する](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-52a767d8) <br/> |このエージェントは [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) イベントと [OnRcptCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnRcptCommand.aspx) イベントに応答し、メッセージ送信者が以前にフロントエンド トランスポート サービスにメッセージを送信したかどうかを判断します。 送信者が以前にメッセージをフロント エンド トランスポート サービスに送信していない場合、その送信者は送信者のリストに追加され、メッセージは拒否され、クライアントには後で再試行するように通知する応答が返されます (グレイリスト方式とも呼ばれます)。 送信者が以前の送信者のリストに含まれている場合は、エージェントがメッセージを拒否することはありません。  <br/> |
|[Exchange 2013: メールボックス サーバー ログ トランスポート エージェントを作成する](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-fc8632e5) <br/> |このエージェントは [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) トランスポート パイプライン イベントに応答し、メッセージをローカル ハード ディスク上のファイルに同期的に記録します。  <br/> |
|[Exchange 2013: X ヘッダー トランスポート エージェントを作成する](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-32f62f5a) <br/> |このエージェントは [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) イベントに応答し、メッセージ内の X ヘッダーの読み取りおよび変更を行います。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange 2013 におけるトランスポート エージェントの概念](transport-agent-concepts-in-exchange-2013.md)    
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)    
- [2013 年の RoutingAgent トランスポート エージェントExchangeする](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)   
- [2013 年の SmtpReceiveAgent トランスポート エージェントExchangeする](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)    
- [2013 年の DeliveryAgent トランスポート エージェントExchangeする](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    

