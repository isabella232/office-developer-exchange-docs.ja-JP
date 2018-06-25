---
title: CanModifyPermissions (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9693de1a-0c76-4898-8f4d-a8693fb005b3
description: CanModifyPermissions 要素は、ユーザーが共有ドキュメントへのアクセス許可を変更できるかどうかを示します。
ms.openlocfilehash: 16526cb79eeca591af6e009e67959a1c3b58a5d7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759608"
---
# <a name="canmodifypermissions-soap"></a>CanModifyPermissions (SOAP)

**CanModifyPermissions**要素は、ユーザーが共有ドキュメントへのアクセス許可を変更できるかどうかを示します。 
  
```XML
<CanModifyPermissions /> 
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

**CanModifyPermissions**要素のブール値は、ユーザーが共有の場所へのアクセス許可を変更できるかどうかを示します。 
  
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

