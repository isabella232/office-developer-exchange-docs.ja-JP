---
title: RedirectUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: c54f310f-8c99-4c37-8e73-ac87722b6229
description: RedirectUrl 要素には、自動検出設定を取得するために使用する必要があるクライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの URL が含まれる。
ms.openlocfilehash: d515f3f79f2370dc496614bab0a3f77300ad4e30
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513529"
---
# <a name="redirecturl-pox"></a>RedirectUrl (POX)

**RedirectUrl** 要素には、自動検出設定の取得に使用するクライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの URL が含まれる。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
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
|[Account (POX)](account-pox.md) <br/> |ユーザーのアカウント設定を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、自動検出設定を取得するために使用する必要があるクライアント アクセス サーバーの URL を表します。
  
## <a name="remarks"></a>注釈

クライアント アプリケーションは、10 回のリダイレクト後にリダイレクトを停止する必要があります。
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

