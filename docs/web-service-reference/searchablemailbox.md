---
title: SearchableMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 339005cd-a3b9-47dd-bc7b-a860b699625b
description: SearchableMailbox 要素は、GetSearchableMailboxes 要求から返されるメールボックスを指定します。
ms.openlocfilehash: f790d9a707f10f64a776b2fc35255c233ad854b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467453"
---
# <a name="searchablemailbox"></a>SearchableMailbox

**SearchableMailbox**要素は、 **Getsearchablemailboxes**要求から返されるメールボックスを指定します。 
  
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

[Guid](guid-ex15websvcsotherref.md)  | [Primarysmtpaddress (文字列)](primarysmtpaddress-string.md)  | [IsExternalMailbox](isexternalmailbox.md)  | [ExternalEmailAddress](externalemailaddress.md)  | [DisplayName (文字列)](displayname-string.md)  | [Isメンバーシップグループ](ismembershipgroup.md)  | [ReferenceId](referenceid.md)
  
### <a name="parent-elements"></a>親要素

[SearchableMailboxes](searchablemailboxes.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   

