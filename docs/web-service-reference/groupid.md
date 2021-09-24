---
title: GroupId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 656d9b9a-8a65-4a75-8466-5b0d96512dab
description: GroupId 要素は、グループを一意に識別します。
ms.openlocfilehash: c0261153a0c64a2e54c053597bd3fdc1466480da
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539669"
---
# <a name="groupid"></a>GroupId

**GroupId 要素は**、グループを一意に識別します。 
  
```XML
<GroupId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |Id 属性のテキスト **値** は、グループの識別子です。  <br/> |
|ChangeKey  <br/> |ChangeKey 属性の **テキスト値** は、グループの変更キーです。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[AddNewImContactToGroup](addnewimcontacttogroup.md)  | [AddNewTelUriContactToGroup](addnewteluricontacttogroup.md)  | [AddImContactToGroup](addimcontacttogroup.md)  | [RemoveContactFromImList](removecontactfromimlist.md)  | [RemoveImContactFromGroup](removeimcontactfromgroup.md)  | [RemoveImGroup](removeimgroup.md)  | [RemoveDistributionGroupFromImList](removedistributiongroupfromimlist.md)  | [SetImGroup](setimgroup.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空の場合  <br/> ||
   

