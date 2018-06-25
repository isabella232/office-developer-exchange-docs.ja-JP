---
title: RemoveImContactFromGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a62b0640-9800-45a6-a297-2105ff36881e
description: RemoveImContactFromGroup 要素は、インスタント メッセージ、インスタント メッセージング グループから連絡先を削除する要求を定義します。
ms.openlocfilehash: 402cbd6929428d410ce5701b0c1afa901703bc29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833094"
---
# <a name="removeimcontactfromgroup"></a>RemoveImContactFromGroup

**RemoveImContactFromGroup**要素は、インスタント メッセージ、インスタント メッセージング グループから連絡先を削除する要求を定義します。 
  
```XML
<RemoveImContactFromGroup>
   <ContactId/>
   <GroupId/>
</RemoveImContactFromGroup>
```

 **RemoveImContactFromGroupType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[ContactId](contactid.md) | [グループ Id](groupid.md)
  
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> ||
   

