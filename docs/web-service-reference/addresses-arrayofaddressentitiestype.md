---
title: アドレス (ArrayOfAddressEntitiesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0c1f3fd3-1b78-46ee-8dd4-b2aff51e767e
description: アドレス要素は、AddressEntity 要素の配列を指定します。
ms.openlocfilehash: b6fbcc54a016e698bccbe075fd340c0c784f121a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759298"
---
# <a name="addresses-arrayofaddressentitiestype"></a>アドレス (ArrayOfAddressEntitiesType)

**アドレス**要素は、 **AddressEntity**要素の配列を指定します。 
  
```XML
<Addresses>
   <AddressEntity/>
</Addresses>
```

 **ArrayOfAddressEntitiesType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[AddressEntity](addressentity.md) <br/> |アドレスの 1 つのエンティティを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[EntityExtractionResult](entityextractionresult.md) <br/> |項目の**EntityExtractionResult**プロパティを指定します。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

