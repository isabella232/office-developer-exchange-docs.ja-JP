---
title: Exchange 2013 のトランスポート エージェントのコード サンプル
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 626345ec-918f-4d91-932f-e6ce92553ccb
description: Exchange 2013 で使用可能なサンプルのトランスポート エージェントについての情報を検索します。
ms.openlocfilehash: 122a3351748fa6ffd823a51ce65ffb913332cb2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759258"
---
# <a name="transport-agent-code-samples-for-exchange-2013"></a>Exchange 2013 のトランスポート エージェントのコード サンプル

Exchange 2013 で使用可能なサンプルのトランスポート エージェントについての情報を検索します。
  
**に適用されます:** Exchange Server 2013
  
トランスポート機能を拡張するためのエージェントを開発するのには、Exchange Server 2013 に含まれている Api を使用することができます。 この資料では、トランスポートの動作をプログラムによって拡張する方法について説明するために使用可能なサンプルのエージェントに関する情報を提供します。 サンプル エージェントには、各コンポーネントのソース コードが含まれます。 
  
次の表には、Exchange 2013 のサンプル エージェントが一覧表示します。
  
**表 1 です。トランスポート エージェントのサンプル**

|**サンプル名**|**説明**|
|:-----|:-----|
|[Exchange 2013: ウイルス対策のトランスポート エージェントを作成します。](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-6e544269) <br/> |このエージェントでは、 [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) 、 [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx)イベントに応答し、非同期的にメッセージを検査し、変更されたバージョンを返しますプロセス外のサーバーに着信メッセージを送信します。  <br/> |
|[Exchange 2013: 帯域幅のログ出力のトランスポート エージェントを作成します。](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) <br/> |このエージェントは、 [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx)と[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)イベントに応答する、指定された受信者は、帯域幅使用率をキャプチャし、帯域幅の使用状況に関する情報をテキスト ファイルに記録します。  <br/> |
|[Exchange 2013: 本文の変換のトランスポート エージェントを作成します。](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) <br/> |このエージェントは、着信メッセージの形式を判断し、フィルター処理が必要かどうかを決定することで、電子メール メッセージのスクリプトをフィルターで除去します。フィルター処理が必要になる場合は、コンテンツを HTML に変換し、フィルターを適用してから元の形式に戻します。  <br/> |
|[Exchange 2013: SMTP ログのトランスポート エージェントを作成します。](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-fc23dc33) <br/> |このエージェントでは、 [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx)イベントに応答し、ローカルのハード ディスク上のファイルを非同期的にメッセージをログ出力します。  <br/> |
|[Exchange 2013: 送信者を一時的にブロックするトランスポート エージェントを作成します。](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-52a767d8) <br/> |このエージェントでは、 [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx)と[OnRcptCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnRcptCommand.aspx)のイベントに応答し、かどうかメッセージの送信者が以前メッセージを送信する、フロント エンド トランスポート サービスを決定します。 送信者が送信者の一覧に追加、後で再試行するのにはクライアントに通知するための応答メッセージは拒否され、送信者がない以前にメッセージを送信、フロント エンド トランスポート サービスの場合 (graylisting とも呼ばれます)。 送信者が、送信者の一覧に以前の場合は、エージェントはメッセージを拒否しません。  <br/> |
|[Exchange 2013: メールボックス サーバーのログ出力のトランスポート エージェントを作成します。](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-fc8632e5) <br/> |このエージェントは、 [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)トランスポート パイプラインのイベントに応答し、ローカルのハード ディスク上のファイルを同期的にメッセージをログ出力します。  <br/> |
|[Exchange 2013: X ヘッダーのトランスポート エージェントを作成します。](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-32f62f5a) <br/> |このエージェントは、 [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx)イベントに応答して読み取るし、メッセージに X ヘッダーを変更します。  <br/> |
   
## <a name="see-also"></a>関連項目

- [トランスポート エージェントの概念には、Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)    
- [Exchange 2013 RoutingAgent トランスポート エージェントを作成します。](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)   
- [Exchange 2013 SmtpReceiveAgent トランスポート エージェントを作成します。](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)    
- [Exchange 2013 DeliveryAgent トランスポート エージェントを作成します。](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    

