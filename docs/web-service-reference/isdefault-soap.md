---
title: IsDefault (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 7358bb88-c441-4f2c-9647-c030e7303e8a
description: IsDefault 要素は、ドキュメント共有の場所がユーザーの既定の共有場所であるかどうかを示します。
ms.openlocfilehash: dbf419d591bc0d693204df51d8259c2a9fe13c50
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466074"
---
# <a name="isdefault-soap"></a>IsDefault (SOAP)

**IsDefault**要素は、ドキュメント共有の場所がユーザーの既定の共有場所であるかどうかを示します。 
  
```XML
<IsDefault /> 
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DocumentSharingLocation (SOAP)](documentsharinglocation-soap.md) <br/> |ドキュメント共有場所の場所とメタデータ情報を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**IsDefault**要素のブール値は、共有の場所がユーザーの既定の共有場所であるかどうかを示します。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)


[Exchange 用自動検出 Web サービス リファレンス](autodiscover-web-service-reference-for-exchange.md)
  
[Exchange 2013 の SOAP 自動検出 XML 要素](soap-autodiscover-xml-elements-for-exchange-2013.md)

