---
title: Exchange の自動検出を使用するときにパフォーマンスを向上させる
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: e65ff6b2-3810-43ad-9728-27308891b193
description: カスタム アプリケーションで自動検出プロセスのパフォーマンスを向上させる方法について説明します。
ms.openlocfilehash: c0920f71c230f63658dfa8d29b34ca75bb796db0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520998"
---
# <a name="improving-performance-when-using-autodiscover-for-exchange"></a>Exchange の自動検出を使用するときにパフォーマンスを向上させる

カスタム アプリケーションで自動検出プロセスのパフォーマンスを向上させる方法について説明します。
  
自動検出が優れている理由はいくつもあります。 ユーザーの操作なしに、Exchange に接続するようにカスタム アプリケーションを構成できることは、特に優れています。 この記事の読者は自動検出が優秀であることと、これを使用することの理由をすべて理解しているはずなので、ここではその説明を省きます。 その代わりに、潜在的な短所であるパフォーマンスについて説明します。
  
自動検出は本質的に遅いプロセスではありません。ただし、本質的に高速なプロセスでもありません。[自動検出プロセス](autodiscover-for-exchange.md)には、多くのネットワーク アクティビティが伴われ、それが多くの遅延の可能性を招くことになります。自動検出プロセスには 3 つのフェーズがあります。すべてのフェーズが潜在的にパフォーマンスに影響を与えます。 
  
- 自動検出エンドポイント候補のプールを定義する: ドメインに参加しているコンピューター上で実行中のアプリケーションの場合は、Active Directory ドメイン サービス (AD DS) との通信が必要になる [SCP 参照](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)を伴うことがあります。
    
- 各候補を試してみる: これには、候補のエンドポイントごとの HTTP 要求/応答が必要になります。
    
- その他の候補を試してみる: 自動検出エンドポイント候補のプールに含まれる候補から成果が得られなかったときには、認証されていない GET 要求 (HTTP 要求/応答) と DNS の参照を実行することになります。
    
一見したところでは、それほど大量ではないようです。ただし、自動検出エンドポイント候補のプールが複数の URL であり、プール内で最後の URL まで機能するエンドポイントが見つからないというシナリオではどうなるでしょう。遅延が顕著に現れるようになります。そこで、何ができるかを考えてみましょう。
  
## <a name="consider-the-need-for-scp-lookup"></a>SCP 参照の必要性について検討する

SCP オブジェクトが存在していて適切に構成されている場合は、それによって自動検出プロセスを高速化できます。それ以外の状況では、速度を低下させることがあります。目的の環境内で SCP が使用されていない場合は、自動検出プロセスの SCP 参照の部分をすべて省略して時間を短縮します。
  
これは、EWS マネージ API によって簡単に実施できます。単に [ExchangeService.AutodiscoverUrl](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) メソッドを呼び出す前に [ExchangeService.EnableScpLookup](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.enablescplookup%28v=exchg.80%29.aspx) プロパティを **false** に設定するだけです。 [AutodiscoverService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice%28v=exchg.80%29.aspx) クラスを使用している場合は、そのクラスのメソッドを呼び出す前に、[AutodiscoverService.EnableScpLookup](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.enablescplookup%28v=exchg.80%29.aspx) プロパティを **false** に設定します。 
  
## <a name="use-autodiscover-less-often"></a>自動検出の使用頻度を下げる

自動検出は、アプリケーションで頻繁に使用されるようには設計されていません。自動検出の暗黙的な対象は、構成情報を検出するために自動検出を使用して、その情報を一定期間キャッシュするアプリケーションです。構成情報をキャッシュしていない場合は、自動検出の使用回数を減らすために、カスタム アプリケーションへのキャッシュ機能の追加を検討します。
  
既にキャッシュしている場合でも、構成情報のキャッシュ期間を査定します。標準では、[24 時間ごとに自動検出の情報を更新](how-to-refresh-configuration-information-by-using-autodiscover.md)しますが、この時間は延長してもかまいません。対象の環境でテストして、目的どおりに動作する構成の "有効時間" を導き出す必要があります。
  
## <a name="minimize-requested-data"></a>要求データを最小限に抑える

EWS マネージ API の **AutodiscoverService** クラスを使用している場合や、SOAP で [GetUserSettings 操作 (SOAP)](https://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx) を使用している場合は、応答で返される設定の内容を直接制御できます。多数の設定を要求できますが、アプリケーションに必要な設定は、そのうちのわずかなものである可能性があります。要求した設定ごとにサーバー上での処理が増えるため、応答の待機時間が長引くようになります。要求している設定を査定して、不要なものを省きます。 
  
EWS マネージ API の **ExchangeService.AutodiscoverUrl** メソッドを使用している場合は、要求する設定を変更することはできません。 ただし、このメソッドはすでに非常に効率的なものになっています。このメソッドは、[UserSettingName enumeration](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=exchg.80%29.aspx) 列挙体の **ExternalEwsUrl** と **InternalEwsUrl** の設定のみを要求します。
  
POX 自動検出サービスを使用している場合は、[特定のプロパティを要求できません ](autodiscover-for-exchange.md#bk_Options)。
  
## <a name="see-also"></a>関連項目


- [Exchange の自動検出](autodiscover-for-exchange.md)
    
- [Exchange の SCP 参照を使用して自動検出エンドポイントを見つける](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [自動検出を使用して構成情報を更新する](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [ExchangeService クラス](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)
    
- [AutodiscoverService クラス](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice%28v=exchg.80%29.aspx)
    

