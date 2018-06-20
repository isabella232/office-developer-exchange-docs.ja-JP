---
title: SearchableMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 339005cd-a3b9-47dd-bc7b-a860b699625b
description: SearchableMailbox 要素は、メールボックスは、GetSearchableMailboxes 要求から返されるを指定します。
ms.openlocfilehash: 0d0981d050fa388e83eaa8408b60d305296c1f36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833284"
---
# <a name="searchablemailbox"></a>SearchableMailbox

**SearchableMailbox**要素は、メールボックスは、 **GetSearchableMailboxes**要求から返されるを指定します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[Guid](guid-ex15websvcsotherref.md) | [PrimarySmtpAddress (文字列)](primarysmtpaddress-string.md) | [IsExternalMailbox](isexternalmailbox.md) | [ExternalEmailAddress](externalemailaddress.md) | [表示名 (文字列)](displayname-string.md) | [IsMembershipGroup](ismembershipgroup.md)  |  [参照 id が](referenceid.md)
  
### <a name="parent-elements"></a>親要素

[SearchableMailboxes](searchablemailboxes.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> ||
   

