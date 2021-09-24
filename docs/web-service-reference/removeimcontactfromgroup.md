---
title: RemoveImContactFromGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: a62b0640-9800-45a6-a297-2105ff36881e
description: RemoveImContactFromGroup 要素は、インスタント メッセージング グループからインスタント メッセージング連絡先を削除する要求を定義します。
ms.openlocfilehash: 426129f6bb26b43374fcb706531af04aea3c1e20
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512409"
---
# <a name="removeimcontactfromgroup"></a>RemoveImContactFromGroup

**RemoveImContactFromGroup** 要素は、インスタント メッセージング グループからインスタント メッセージング連絡先を削除する要求を定義します。 
  
```XML
<RemoveImContactFromGroup>
   <ContactId/>
   <GroupId/>
</RemoveImContactFromGroup>
```

 **RemoveImContactFromGroupType**
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
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> ||
   

