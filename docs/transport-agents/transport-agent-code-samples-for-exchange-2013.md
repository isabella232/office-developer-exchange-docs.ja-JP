---
title: Exchange 2013 のトランスポート エージェントのコード サンプル
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 626345ec-918f-4d91-932f-e6ce92553ccb
description: Exchange 2013 で利用可能なサンプルトランスポートエージェントに関する情報を検索します。
ms.openlocfilehash: c14a4e34102b55014cc6507e375929c186f5f6e9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461801"
---
# <a name="transport-agent-code-samples-for-exchange-2013"></a>Exchange 2013 のトランスポート エージェントのコード サンプル

Exchange 2013 で利用可能なサンプルトランスポートエージェントに関する情報を検索します。
  
**製品:** Exchange Server 2013
  
Exchange Server 2013 に含まれる Api を使用して、トランスポート機能を拡張するエージェントを開発できます。 この記事では、トランスポート動作をプログラムによって拡張する方法の学習に利用できるサンプル エージェントに関する情報について説明します。 サンプル エージェントには、各コンポーネントのソース コードが含まれています。 
  
次の表に、Exchange 2013 のサンプルエージェントを示します。
  
**表1トランスポートエージェントのサンプル**

|**サンプルの名前**|**説明**|
|:-----|:-----|
|[Exchange 2013: ウイルス対策トランスポートエージェントを構築する](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-6e544269) <br/> |このエージェントは、 [Onendofdata](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx)および[onsubmittedmessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx)イベントに応答して、メッセージを非同期で調べ、変更されたバージョンを返すプロセス外のサーバーに受信メッセージを送信します。  <br/> |
|[Exchange 2013: 帯域幅ログトランスポートエージェントを構築する](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) <br/> |このエージェントは、 [Onsubmittedmessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx)イベントと[onsubmittedmessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)イベントに応答し、指定された受信者の帯域幅使用状況をキャプチャして、帯域幅使用状況の情報をテキストファイルに記録します。  <br/> |
|[Exchange 2013: 本文変換トランスポートエージェントを構築する](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) <br/> |このエージェントは、着信メッセージの形式を判断し、フィルター処理が必要かどうかを決定することで、電子メール メッセージのスクリプトをフィルターで除去します。フィルター処理が必要になる場合は、コンテンツを HTML に変換し、フィルターを適用してから元の形式に戻します。  <br/> |
|[Exchange 2013: SMTP ログトランスポートエージェントを作成する](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-fc23dc33) <br/> |このエージェントは[Onendofdata](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx)イベントに応答し、ローカルハードディスク上のファイルにメッセージを非同期的に記録します。  <br/> |
|[Exchange 2013: 送信者を一時的にブロックするトランスポートエージェントを構築する](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-52a767d8) <br/> |このエージェントは、 [Onendofheaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx)および[Onrcptcommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnRcptCommand.aspx)イベントに応答し、メッセージの送信者が以前にフロントエンドトランスポートサービスにメッセージを送信したかどうかを判断します。 送信者が以前にメッセージをフロント エンド トランスポート サービスに送信していない場合、その送信者は送信者のリストに追加され、メッセージは拒否され、クライアントには後で再試行するように通知する応答が返されます (グレイリスト方式とも呼ばれます)。 送信者が以前の送信者のリストに含まれている場合は、エージェントがメッセージを拒否することはありません。  <br/> |
|[Exchange 2013: メールボックスサーバーログトランスポートエージェントを構築する](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-fc8632e5) <br/> |このエージェントは、 [Onルーブル tedmessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) transport pipeline イベントに応答し、メッセージをローカルハードディスク上のファイルに同期的に記録します。  <br/> |
|[Exchange 2013: X ヘッダートランスポートエージェントを構築する](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-32f62f5a) <br/> |このエージェントは、 [Onendofheaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx)イベントに応答し、メッセージ内の X ヘッダーを読み取りおよび変更します。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange 2013 におけるトランスポート エージェントの概念](transport-agent-concepts-in-exchange-2013.md)    
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)    
- [Exchange 2013 用の RoutingAgent トランスポートエージェントの作成](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)   
- [Exchange 2013 用の SmtpReceiveAgent トランスポートエージェントを作成する](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)    
- [Exchange 2013 用の DeliveryAgent トランスポートエージェントの作成](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    

