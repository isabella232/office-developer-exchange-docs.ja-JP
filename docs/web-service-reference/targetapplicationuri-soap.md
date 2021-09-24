---
title: TargetApplicationUri (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: e13c0edd-2ab1-49bb-a993-54a8db2dfbb9
description: TargetApplicationUri 要素は、ターゲット アプリケーション URI を定義します。 TargetApplicationUri 要素は内部でのみ使用できます。 この要素は、クライアントでは使用されません。
ms.openlocfilehash: 3bed26b697fc3638782de5abd53a68fd04f031e6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522573"
---
# <a name="targetapplicationuri-soap"></a>TargetApplicationUri (SOAP)

**TargetApplicationUri 要素** は、ターゲット アプリケーション URI を定義します。 **TargetApplicationUri 要素** は内部でのみ使用できます。 この要素は、クライアントでは使用されません。 
  
```XML
<TargetApplicationUri/>
```

 **anyURI**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |1 つの組織の組織関係の一覧を表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は、外部組織のターゲット URI を定義します。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

