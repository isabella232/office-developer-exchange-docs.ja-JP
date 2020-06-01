---
title: RedirectUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c54f310f-8c99-4c37-8e73-ac87722b6229
description: RedirectUrl 要素には、Microsoft Exchange Server 2007 を実行しているコンピューターの URL が含まれています。これにより、クライアントアクセスサーバーの役割がインストールされており、自動検出の設定を取得するために使用する必要があります。
ms.openlocfilehash: 5400b1e7a4bb7ebebc58b6a0f1fc9bf37f5a2e22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468090"
---
# <a name="redirecturl-pox"></a>RedirectUrl (POX)

**Redirecturl**要素には、Microsoft Exchange server 2007 を実行しているコンピューターの URL が含まれています。これにより、クライアントアクセスサーバーの役割がインストールされており、自動検出の設定を取得するために使用する必要があります。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[RedirectUrl (POX)](redirecturl-pox.md)
  
```xml
<RedirectUrl/>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アカウント (POX)](account-pox.md) <br/> |ユーザーのアカウント設定を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

Text 値は、自動検出設定を取得するために使用するクライアントアクセスサーバーの URL を表します。
  
## <a name="remarks"></a>注釈

クライアントアプリケーションは、10回リダイレクトした後にリダイレクトを停止する必要があります。
  
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

