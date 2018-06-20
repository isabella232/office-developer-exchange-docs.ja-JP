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
description: RedirectUrl 要素には、クライアント アクセス サーバーの役割がインストールされている自動検出の設定を取得するために使用する必要があります Microsoft Exchange Server 2007 を実行しているコンピューターの URL が含まれています。
ms.openlocfilehash: 3b634f1a3a3d44b6aae1a826a005149200641dcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833027"
---
# <a name="redirecturl-pox"></a>RedirectUrl (POX)

**RedirectUrl**要素には、クライアント アクセス サーバーの役割がインストールされている自動検出の設定を取得するために使用する必要があります Microsoft Exchange Server 2007 を実行しているコンピューターの URL が含まれています。 
  
[(POX) を自動検出](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[RedirectUrl (POX)](redirecturl-pox.md)
  
```xml
<RedirectUrl/>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アカウント (POX)](account-pox.md) <br/> |ユーザーのアカウントの設定を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、自動検出の設定を取得するために使用する必要がありますクライアント アクセス サーバーの URL を表します。
  
## <a name="remarks"></a>備考

クライアント アプリケーションでは、10 リダイレクト後のリダイレクトを停止する必要があります。
  
## <a name="see-also"></a>関連項目



[交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

