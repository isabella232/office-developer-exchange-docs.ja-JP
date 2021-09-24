---
title: SearchableMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 339005cd-a3b9-47dd-bc7b-a860b699625b
description: SearchableMailbox 要素は、GetSearchableMailboxes 要求から返されるメールボックスを指定します。
ms.openlocfilehash: 75d5680de8b0776b1ecf441ff71266ee74c4aa66
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524428"
---
# <a name="searchablemailbox"></a>SearchableMailbox

**SearchableMailbox 要素** は **、GetSearchableMailboxes** 要求から返されるメールボックスを指定します。 
  
```XML
<SearchableMailbox>
   <Guid/>
   <PrimarySmtpAddress/>
   <IsExternalMailbox/>
   <ExternalEmailAddress/>
   <DisplayName/>
   <IsMembershipGroup/>
   <ReferenceId/>
</SearchableMailbox>
```

 **SearchableMailboxType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[Guid](guid-ex15websvcsotherref.md)  | [PrimarySmtpAddress (string)](primarysmtpaddress-string.md)  | [IsExternalMailbox](isexternalmailbox.md)  | [ExternalEmailAddress](externalemailaddress.md)  | [DisplayName (string)](displayname-string.md)  | [IsMembershipGroup](ismembershipgroup.md)  | [ReferenceId](referenceid.md)
  
### <a name="parent-elements"></a>親要素

[SearchableMailboxes](searchablemailboxes.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> ||
   

