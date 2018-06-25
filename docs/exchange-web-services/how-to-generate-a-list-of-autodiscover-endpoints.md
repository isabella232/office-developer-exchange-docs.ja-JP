---
title: 自動検出エンドポイントの一覧を生成します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 82394d3c-9fc7-4b3c-b48d-1fe983c198f7
description: 自動検出エンドポイントの優先順位を付けた一覧を生成する方法について説明します。
ms.openlocfilehash: ccecacc9c8beef464727efbc9d1fced7a81f9b7c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758958"
---
# <a name="generate-a-list-of-autodiscover-endpoints"></a>自動検出エンドポイントの一覧を生成します。

自動検出エンドポイントの優先順位を付けた一覧を生成する方法について説明します。
  
[自動検出プロセス](autodiscover-for-exchange.md)の最初のタスクでは、実行するアプリケーションの自動検出エンドポイントの一覧を生成します。 これらのエンドポイントの自動検出は、 [SCP のルックアップ](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)に由来することができます。 またはユーザーの電子メール アドレスから派生させることができます。 最後に、エンドポイントの数が多い場合終了できます。 優先順位を整理する方法を見てみましょう。 
  
## <a name="start-with-scp-lookup"></a>SCP 参照から始める
<a name="bk_StartWithScp"> </a>

[SCP の検索](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)からの自動検出エンドポイントの一覧で最上位の優先順位が必要です。 管理者は、これらのエンドポイントを使用して起動するので、最も近いまたは最も効率的な自動検出エンドポイントに、クライアントをルーティングする SCP オブジェクトを構成できます。 SCP 検索プロセスは、独自の優先順位付けがあるため、SCP 検索の結果既に優先度付けは、次のように。 
  
1. クライアント コンピューターが属する Active Directory サイトを対象とする SCP オブジェクトからの自動検出エンドポイント。
    
2. Active Directory サイトのいずれをも対象としない SCP オブジェクトからの自動検出エンドポイント。
    
3. クライアント コンピューターが属するサイトとは別の Active Directory サイトを対象とする SCP オブジェクトからの自動検出エンドポイント。
    
SCP 検索プロセスの結果を作成したら、ユーザーの電子メール アドレスから派生するエンドポイントを追加できます。 これらは、SCP の結果が存在しないか、SCP 検索から返されたエンドポイントは不十分な場合に既定のエンドポイント、およびフォールバックのセットとして使用できます。
  
## <a name="add-endpoints-derived-from-the-users-email-address"></a>ユーザーのメール アドレスから派生したエンドポイントを追加する
<a name="bk_AddDerivedEndpoints"> </a>

SCP 参照が動作しない場合、または SCP 参照によって返されたエンドポイントが正常な応答を返さない場合、ユーザーのメール アドレスから既定の自動検出エンドポイントのセットを得ることができます。これらのエンドポイントは SCP 参照からのどのエンドポイントよりも優先度は低くなりますが、SCP 参照が失敗する場合に必要になる可能性があります。
  
### <a name="to-derive-autodiscover-endpoints"></a>自動検出エンドポイントを取得する方法

1. ユーザーのメール アドレスからドメイン名を抽出します。たとえば、ユーザーのメール アドレスが Sadie.Daniels@contoso.com である場合、ドメイン名は contoso.com になります。
    
2. ファイル拡張子を持たないエンドポイント URL を、次の形式で作成します。
    
  - "https://" + ドメイン + "/autodiscover/autodiscover"
    
  - "https://autodiscover." + ドメイン +「自動検出/自動検出」
    
SCP 検索とユーザーの電子メール アドレスの両方から派生するエンドポイントの Url のリストをコンパイルした後は、 [SOAP の自動検出 web サービス](http://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx)または POX の[のどちらを使用しているかどうかに応じて、これらの Url でファイル名の拡張子を変更する必要があります。自動検出 web サービス](http://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx)。
  
## <a name="add-or-replace-file-name-extensions-in-endpoint-urls"></a>エンドポイント URL のファイル名拡張子を追加または置き換える
<a name="bk_FileExtensions"> </a>

自動検出サービスにアクセスするには、SOAP 自動検出 Web サービスまたは POX 自動検出 Web サービスを使用します。各サービスでは、類似したエンドポイント URL (ファイル名拡張子だけが異なる) が使用されます。SOAP 自動検出 Web サービスでは ".svc" ファイル名拡張子が使用され、POX 自動検出 Web サービスでは ".xml" ファイル名拡張子が使用されます。
  
既定では、SCP 参照から返された自動検出エンドポイント URL は POX URL です。ただし、SOAP 自動検出を使用している場合は、ファイル名拡張子を ".xml" から ".svc" に変更するだけで、SOAP 要求を試行できます。
  
派生した自動検出エンドポイント URL の場合、ファイル拡張子は省略されています。URL を試用する前に、使用中の自動検出 Web サービスに適切なファイル拡張子を追加します。
  
## <a name="example-generating-a-list-of-autodiscover-endpoints"></a>例:自動検出エンドポイントの一覧を生成する
<a name="bk_Example"> </a>

例を見てみましょう。Sadie Daniels (Sadie.Daniels@contoso.com) は、Exchange Web サービス (EWS) アプリケーションを初めて使用しています。アプリケーションでは、アプリケーション自体を構成するのに自動検出を使用します。Sadie のコンピューターは、contoso.com ドメインに参加し、Redmond Active Directory サイトにあります。アプリケーションでは、図 1 に示すように自動検出エンドポイントの一覧が生成されます。
  
**自動検出エンドポイントの図 1: サンプルの一覧**

![導出されたエンドポイントよりも高い優先順位を持つエンドポイントとして SCP ルックアップ から取得された、Autodiscover エンドポイントのサンプル リスト。](media/Ex15_Autodiscover_GenerateList_Example.png)
  
この例の EWS アプリケーションでは SOAP 自動検出 Web サービスが使用されるため、SCP 結果のファイル名拡張子を ".svc" に変更してから SOAP 要求を送信します。
  
## <a name="next-steps"></a>次の手順
<a name="bk_NextSteps"> </a>

自動検出エンドポイントの一覧を生成した後は、[これらのエンドポイントへの要求を送信](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)してください。
  
## <a name="see-also"></a>関連項目


- [Exchange の自動検出](autodiscover-for-exchange.md)
    
- [Exchange SCP のルックアップを使用して自動検出エンドポイントを検索します。](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [自動検出のエラー メッセージの処理](handling-autodiscover-error-messages.md)
    

