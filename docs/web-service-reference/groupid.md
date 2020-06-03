---
title: GroupId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 656d9b9a-8a65-4a75-8466-5b0d96512dab
description: GroupId 要素は、グループを一意に識別します。
ms.openlocfilehash: 3b8de4d0fef95e2caff4db0d90bb303830022d36
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530093"
---
# <a name="groupid"></a>GroupId

**GroupId**要素は、グループを一意に識別します。 
  
```XML
<GroupId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |**Id**属性のテキスト値は、グループの識別子です。  <br/> |
|ChangeKey  <br/> |**Changekey**属性のテキスト値は、グループの変更キーです。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[AddNewImContactToGroup](addnewimcontacttogroup.md)  | [AddNewTelUriContactToGroup](addnewteluricontacttogroup.md)  | [Addimcontacttogroup](addimcontacttogroup.md)  | [RemoveContactFromImList](removecontactfromimlist.md)  | [Removeimcontactfromgroup](removeimcontactfromgroup.md)  | [Removeimgroup](removeimgroup.md)  | [RemoveDistributionGroupFromImList](removedistributiongroupfromimlist.md)  | [Setimgroup](setimgroup.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> ||
   

