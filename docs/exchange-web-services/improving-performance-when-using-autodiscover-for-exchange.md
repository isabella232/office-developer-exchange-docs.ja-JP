---
title: Exchange の自動検出を使用するときにパフォーマンスを向上させる
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e65ff6b2-3810-43ad-9728-27308891b193
description: カスタム アプリケーションで自動検出プロセスのパフォーマンスを向上させる方法について説明します。
ms.openlocfilehash: d9eef3bdc76c16cf92bdbb39b36be067f0c06215
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/15/2018
ms.locfileid: "19759120"
---
# <a name="improving-performance-when-using-autodiscover-for-exchange"></a>Exchange の自動検出を使用するときにパフォーマンスを向上させる

カスタム アプリケーションで自動検出プロセスのパフォーマンスを向上させる方法について説明します。
  
などの自動検出する理由の多くにはあります。 ユーザーの介入なしで Exchange に接続するようにアプリケーションを構成することはすばらしい! 場合はこの資料を読んでいるなら、既に理由を把握してすべてを使用し、自動検出では、ここに記載はありませんので気に入っています。 代わりに、潜在的な欠点について説明を行っています: パフォーマンス。
  
自動検出は、低速なプロセスでない本質的には本質的に高速か。 [自動検出プロセス](autodiscover-for-exchange.md)では、多くのネットワークの動作、および遅延が発生する可能性の多くを導入します。 自動検出プロセスには 3 つのフェーズです。3 つすべてでは、パフォーマンスに影響を与える可能性があります。 
  
- 自動検出エンドポイントの候補者のプールを定義する、ドメインに参加しているコンピューターで実行されているアプリケーションでは、 [SCP の参照](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)は、Active Directory ドメイン サービス (AD DS) と通信しているがあります。
    
- 各候補を試してみる: これには、候補のエンドポイントごとの HTTP 要求/応答が必要になります。
    
- その他の候補を試してみる: 自動検出エンドポイント候補のプールに含まれる候補から成果が得られなかったときには、認証されていない GET 要求 (HTTP 要求/応答) と DNS の参照を実行することになります。
    
一見したところでは、それほど大量ではないようです。ただし、自動検出エンドポイント候補のプールが複数の URL であり、プール内で最後の URL まで機能するエンドポイントが見つからないというシナリオではどうなるでしょう。遅延が顕著に現れるようになります。そこで、何ができるかを考えてみましょう。
  
## <a name="consider-the-need-for-scp-lookup"></a>SCP 参照の必要性について検討する

SCP オブジェクトが存在していて適切に構成されている場合は、それによって自動検出プロセスを高速化できます。それ以外の状況では、速度を低下させることがあります。目的の環境内で SCP が使用されていない場合は、自動検出プロセスの SCP 参照の部分をすべて省略して時間を短縮します。
  
EWS のマネージ API では、これを簡単に: [ExchangeService.AutodiscoverUrl](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx)メソッドを呼び出す前に[ExchangeService.EnableScpLookup](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.enablescplookup%28v=exchg.80%29.aspx)プロパティを**false**に設定します。 [AutodiscoverService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice%28v=exchg.80%29.aspx)クラスを使用する場合は、メソッドを呼び出す前に**false を指定**する[AutodiscoverService.EnableScpLookup](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.enablescplookup%28v=exchg.80%29.aspx)プロパティを設定します。 
  
## <a name="use-autodiscover-less-often"></a>自動検出の使用頻度を下げる

自動検出は、アプリケーションで頻繁に使用されるようには設計されていません。自動検出の暗黙的な対象は、構成情報を検出するために自動検出を使用して、その情報を一定期間キャッシュするアプリケーションです。構成情報をキャッシュしていない場合は、自動検出の使用回数を減らすために、カスタム アプリケーションへのキャッシュ機能の追加を検討します。
  
でも既にをキャッシュする場合、構成情報をキャッシュする時間の長さを評価します。 [24 時間ごとの自動検出情報を更新](how-to-refresh-configuration-information-by-using-autodiscover.md)するには、標準が、その時間を延長できる場合があります。 思い付く、」の有効期限"には、有効な構成、ターゲット環境とテストをしてください。
  
## <a name="minimize-requested-data"></a>要求データを最小限に抑える

EWS のマネージ API で、または SOAP を使用して[GetUserSettings 操作 (SOAP)](http://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx)の操作で**AutodiscoverService**クラスを使用する場合は、応答で返されるどのような設定を直接制御があります。 非常に多くの設定を要求することができますが、アプリケーションにそれらのいくつかが必要なだけの可能性があります。 要求するすべての設定では、サーバーの応答を待機しているより多くの時間でより多くの処理が必要です。 要求している設定を評価し、除外する必要がないです。 
  
EWS のマネージ API では、 **ExchangeService.AutodiscoverUrl**メソッドを使用している場合を要求する設定を変更することはできません。 ただし、このメソッドは、既に非常に非効率です。[UserSettingName 列挙型](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=exchg.80%29.aspx)から、 **ExternalEwsUrl**と**InternalEwsUrl**の設定を要求のみです。
  
POX の自動検出サービスは、[特定のプロパティを要求することはできません](autodiscover-for-exchange.md#bk_Options)使用する場合。
  
## <a name="see-also"></a>関連項目


- [Exchange の自動検出](autodiscover-for-exchange.md)
    
- [Exchange SCP のルックアップを使用して自動検出エンドポイントを検索します。](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [自動検出を使用して構成情報を更新します。](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [ExchangeService クラス](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)
    
- [AutodiscoverService クラス](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice%28v=exchg.80%29.aspx)
    

