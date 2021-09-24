---
title: Guid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 49dcf69f-bf8d-4be6-a24c-03bbd13f4fe5
description: Guid 要素は、メールボックスのグローバル一意識別子を指定します。
ms.openlocfilehash: 093364e26d5c65127c1f23214e1d3d0aa85c95c2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519535"
---
# <a name="guid"></a>Guid

**Guid 要素** は、メールボックスのグローバル一意識別子を指定します。 
  
```XML
<Guid></Guid>
```

 **GuidType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SearchableMailbox](searchablemailbox.md) <br/> |**GetSearchableMailboxes** 要求から返されるメールボックスを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

Guid 要素のテキスト **値** は、メールボックスを一意に識別する GUID 値です。 
  
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

