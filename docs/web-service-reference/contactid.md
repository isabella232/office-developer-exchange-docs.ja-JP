---
title: ContactId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 86f66275-1e39-48ed-bd89-ac3bffc465a7
description: ContactId 要素は、連絡先を一意に識別します。
ms.openlocfilehash: 6b00d2f83c31905b5901a9d0dec2994c23fcb21d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533901"
---
# <a name="contactid"></a>ContactId

**ContactId 要素は**、連絡先を一意に識別します。 
  
```XML
<ContactId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |Id 属性のテキスト **値** は、連絡先アイテムの識別子です。  <br/> |
|ChangeKey  <br/> |ChangeKey 属性の **テキスト値** は、連絡先アイテムの変更キーです。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[AddImContactToGroup](addimcontacttogroup.md)  | [RemoveContactFromImList](removecontactfromimlist.md)  | [RemoveImContactFromGroup](removeimcontactfromgroup.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

