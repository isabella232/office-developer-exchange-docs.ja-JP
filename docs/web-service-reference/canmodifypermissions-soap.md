---
title: CanModifyPermissions (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 9693de1a-0c76-4898-8f4d-a8693fb005b3
description: CanModifyPermissions 要素は、ユーザーがドキュメント共有場所へのアクセス許可を変更できるかどうかを示します。
ms.openlocfilehash: 5aa11ff62fc5c82d263eb03707d7514b87c94be0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515986"
---
# <a name="canmodifypermissions-soap"></a>CanModifyPermissions (SOAP)

**CanModifyPermissions 要素** は、ユーザーがドキュメント共有場所へのアクセス許可を変更できるかどうかを示します。 
  
```XML
<CanModifyPermissions /> 
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

**CanModifyPermissions** 要素のブール値は、ユーザーが共有場所へのアクセス許可を変更できるかどうかを示します。 
  
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

