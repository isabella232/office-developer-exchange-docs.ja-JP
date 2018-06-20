---
title: ExternalAccessAllowed (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 967df8c0-ee95-4202-b037-0c4b9fbbf5ee
description: ExternalAccessAllowed 要素は、場所を共有するドキュメントは、外部の接続からに使用できるかどうかを示します。
ms.openlocfilehash: 7d2a4027fe6de0c24191272d65605310af6a16bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760434"
---
# <a name="externalaccessallowed-soap"></a>ExternalAccessAllowed (SOAP)

**ExternalAccessAllowed**要素は、場所を共有するドキュメントは、外部の接続からに使用できるかどうかを示します。 
  
```XML
<ExternalAccessAllowed /> 
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DocumentSharingLocation (SOAP)](documentsharinglocation-soap.md) <br/> |場所を共有するドキュメントの場所およびメタデータの情報を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**ExternalAccessAllowed**要素のブール値は、共有の場所は外部の接続からに使用できるかどうかを示します。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)


[Exchange の自動検出 web サービスの参照](autodiscover-web-service-reference-for-exchange.md)
  
[Exchange 2013 の自動検出の XML 要素を SOAP](soap-autodiscover-xml-elements-for-exchange-2013.md)

