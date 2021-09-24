---
title: EmailAddresses (ArrayOfEmailAddressEntitiesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 2fc4a8e8-5377-4059-8fb4-3fdabfd30fe3
description: EmailAddresses 要素は、電子メール アドレス エンティティの配列を指定します。
ms.openlocfilehash: acb784e89bbc4cc6618bf5bad6e5cf0c7274bdfb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531015"
---
# <a name="emailaddresses-arrayofemailaddressentitiestype"></a>EmailAddresses (ArrayOfEmailAddressEntitiesType)

**EmailAddresses 要素** は、電子メール アドレス エンティティの配列を指定します。 
  
```XML
<EmailAddresses>
    <EmailAddressEntity></EmailAddressEntity>
</EmailAddresses>
```

 **ArrayOfEmailAddressEntitiesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[EmailAddressEntity](emailaddressentity.md) <br/> |1 つの電子メール アドレス エンティティを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[EntityExtractionResult](entityextractionresult.md) <br/> |アイテムの **EntityExtractionResult** プロパティを指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

