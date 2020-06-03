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
description: DeploymentId 要素は、Microsoft Exchange Server 2007 フォレストを一意に識別します。
ms.openlocfilehash: 4986a3404763e88fb3e84d52a5d30d54c810f93a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467922"
---
# <a name="deploymentid-pox"></a>DeploymentId (POX)

**DeploymentId**要素は、Microsoft Exchange Server 2007 フォレストを一意に識別します。 
  
- [自動検出 (POX)](autodiscover-pox.md)  
- [応答 (POX)](response-pox.md) 
- [ユーザー (POX)](user-pox.md)  
- [DeploymentId (POX)](deploymentid-pox.md)
  
```xml
<DeploymentId/>
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
|[ユーザー (POX)](user-pox.md) <br/> |ユーザー固有の情報を提供します。  <br/> |
   
## <a name="text-value"></a>テキスト値

Text 値は、Exchange 2007 フォレストを GUID 形式で一意に識別します。
  
## <a name="remarks"></a>注釈

Exchange 2007 をアンインストールしてから再インストールし、同じサーバー名を使用すると、 **DeploymentId**値が変更されます。 
  
## <a name="see-also"></a>関連項目

- [Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

