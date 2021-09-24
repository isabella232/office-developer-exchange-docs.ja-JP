---
title: IsDefault (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 7358bb88-c441-4f2c-9647-c030e7303e8a
description: IsDefault 要素は、ドキュメント共有の場所がユーザーの既定の共有場所であるかどうかを示します。
ms.openlocfilehash: cf8547dc017a1470406f312214fa8e532083ef9e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539501"
---
# <a name="isdefault-soap"></a>IsDefault (SOAP)

**IsDefault 要素** は、ドキュメント共有の場所がユーザーの既定の共有場所であるかどうかを示します。 
  
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

**IsDefault** 要素のブール値は、共有場所がユーザーの既定の共有場所であるかどうかを示します。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)


[Exchange 用自動検出 Web サービス リファレンス](autodiscover-web-service-reference-for-exchange.md)
  
[SOAP 自動検出 XML 要素 (2013 Exchange)](soap-autodiscover-xml-elements-for-exchange-2013.md)

