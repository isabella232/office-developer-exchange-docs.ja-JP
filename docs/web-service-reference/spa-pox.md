---
title: SPA (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: fba018d5-0c65-4e1b-9767-d1ce8b356278
description: SPA 要素は、セキュリティで保護されたパスワード認証 (SPA) が必要かどうかを示します。
ms.openlocfilehash: cf57b3a6046b1b9b030b7cae81381189eee92c1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467642"
---
# <a name="spa-pox"></a>SPA (POX)

**Spa**要素は、セキュリティで保護されたパスワード認証 (SPA) が必要かどうかを示します。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
[SPA (POX)](spa-pox.md)
  
```xml
<SPA/>
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
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

Text 値は、SPA が必要かどうかを示します。 テキスト値が**の**場合は、SPA が必要です。
  
## <a name="remarks"></a>注釈

この要素が存在しない場合、既定値は **[オン**] に設定されます。
  
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

