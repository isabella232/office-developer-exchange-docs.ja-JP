---
title: AddImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65554e4c-c0d9-485e-9f01-ed1baa8280ab
description: AddImContactToGroup 要素は、既存のインスタントメッセージングの連絡先をインスタントメッセージンググループに追加する要求を定義します。
ms.openlocfilehash: b86b1cb69a1ebc7034e5a27047c14efbab7236ea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459666"
---
# <a name="addimcontacttogroup"></a>AddImContactToGroup

**Addimcontacttogroup**要素は、既存のインスタントメッセージングの連絡先をインスタントメッセージンググループに追加する要求を定義します。 
  
```XML
<AddImContactToGroup>
   <ContactId/>
   <GroupId/>
</AddImContactToGroup>
```

 **AddImContactToGroupType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[ContactId](contactid.md)  | [GroupId](groupid.md)
  
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

