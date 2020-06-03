---
title: DocumentSharingLocationCollectionSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0e3346f9-7a55-4e87-b121-9b1ee7f227f4
description: DocumentSharingLocationCollectionSetting 要素は、ドキュメント共有の場所とメタデータのコレクションであるユーザー設定を表します。
ms.openlocfilehash: 2a52f639a1f1bf638aacc78666c58aed1fae0fa0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457054"
---
# <a name="documentsharinglocationcollectionsetting-soap"></a>DocumentSharingLocationCollectionSetting (SOAP)

**Documentsharinglocationcollectionsetting**要素は、ドキュメント共有の場所とメタデータのコレクションであるユーザー設定を表します。 
  
[DocumentSharingLocationCollectionSetting (SOAP)](documentsharinglocationcollectionsetting-soap.md)
  
```XML
<DocumentSharingLocationCollectionSetting>
    <DocumentSharingLocations />
</DocumentSharingLocationCollectionSetting>
```

 **DocumentSharingLocationCollectionSetting**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[DocumentSharingLocations (SOAP)](documentsharinglocations-soap.md) <br/> |ドキュメント共有の場所のリストの場所とメタデータを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[UserSettings (SOAP)](usersettings-soap.md) <br/> |ユーザー設定のコレクションを表します。  <br/> |
   
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
- [Exchange 用自動検出 Web サービス リファレンス](autodiscover-web-service-reference-for-exchange.md)
- [Exchange 2013 の SOAP 自動検出 XML 要素](soap-autodiscover-xml-elements-for-exchange-2013.md)

