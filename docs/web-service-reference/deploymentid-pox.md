---
title: DeploymentId (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: b879c134-307e-4645-bb53-55d8ba4fad9c
description: DeploymentId 要素は、2007 フォレストMicrosoft Exchange Server一意に識別します。
ms.openlocfilehash: 37d66eadb38f02e75a35d0516b36aff07dfdafa6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545357"
---
# <a name="deploymentid-pox"></a>DeploymentId (POX)

**DeploymentId 要素は**、2007 フォレストMicrosoft Exchange Server一意に識別します。 
  
- [AutoDiscover (POX)](autodiscover-pox.md)  
- [Response (POX)](response-pox.md) 
- [User (POX)](user-pox.md)  
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
|[User (POX)](user-pox.md) <br/> |ユーザー固有の情報を提供します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、GUID 形式Exchange 2007 フォレストを一意に識別します。
  
## <a name="remarks"></a>注釈

2007 をアンインストールしてから再インストールExchange同じサーバー名を使用すると **、DeploymentId** の値が変更されます。 
  
## <a name="see-also"></a>関連項目

- [POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

