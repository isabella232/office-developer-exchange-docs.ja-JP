---
title: DeploymentId (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b879c134-307e-4645-bb53-55d8ba4fad9c
description: DeploymentId 要素は、Microsoft Exchange Server 2007 のフォレストを一意に識別します。
ms.openlocfilehash: 4f2548709753d8407d02218acecd9233f0ba764f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760011"
---
# <a name="deploymentid-pox"></a>DeploymentId (POX)

**DeploymentId**要素は、Microsoft Exchange Server 2007 のフォレストを一意に識別します。 
  
- [(POX) を自動検出](autodiscover-pox.md)  
- [応答 (POX)](response-pox.md) 
- [ユーザー (POX)](user-pox.md)  
- [DeploymentId (POX)](deploymentid-pox.md)
  
```xml
<DeploymentId/>
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
|[ユーザー (POX)](user-pox.md) <br/> |ユーザー固有の情報を提供します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、Exchange 2007 フォレストでは、GUID の形式を一意に識別します。
  
## <a name="remarks"></a>備考

アンインストールし、Exchange 2007 を再インストールし、同じサーバー名を使用すると、 **DeploymentId**の値を変更します。 
  
## <a name="see-also"></a>関連項目

- [交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

