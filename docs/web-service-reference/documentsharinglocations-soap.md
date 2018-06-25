---
title: DocumentSharingLocations (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 394f6015-721b-4800-9286-039d430f09b3
description: DocumentSharingLocations 要素には、場所と場所を共有するドキュメントのメタデータ情報の一覧が含まれています。
ms.openlocfilehash: 72d1ae9f01ad45441b4e255f2fb6353be2dc8d28
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760144"
---
# <a name="documentsharinglocations-soap"></a>DocumentSharingLocations (SOAP)

**DocumentSharingLocations**要素には、場所と場所を共有するドキュメントのメタデータ情報の一覧が含まれています。 
  
```XML
<DocumentSharingLocations>
   <DocumentSharingLocation />
</DocumentSharingLocations>
```

 **DocumentSharingLocations**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[DocumentSharingLocation (SOAP)](documentsharinglocation-soap.md) <br/> |場所と場所を共有するドキュメントのメタデータが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DocumentSharingLocationCollectionSetting (SOAP)](documentsharinglocationcollectionsetting-soap.md) <br/> |共有の場所およびメタデータ ドキュメントのコレクションに設定されているユーザーを表します。  <br/> |
   
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
- [Exchange の自動検出 web サービスの参照](autodiscover-web-service-reference-for-exchange.md)
- [Exchange 2013 の自動検出の XML 要素を SOAP](soap-autodiscover-xml-elements-for-exchange-2013.md)

