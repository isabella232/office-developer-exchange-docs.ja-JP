---
title: UnpinTeamMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 1034b013-ef34-4e72-99b3-38bff475b3e8
description: UnpinTeamMailbox 要素には、自動検出応答からサイト メールボックスを削除して、クライアントからサイト メールボックスのピン留めを解除する要求が含まれている。
ms.openlocfilehash: 520d201f8ba618d085ef5b190184fceaf66b4170
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541827"
---
# <a name="unpinteammailbox"></a>UnpinTeamMailbox

**UnpinTeamMailbox** 要素には、自動検出応答からサイト メールボックスを削除して、クライアントからサイト メールボックスのピン留めを解除する要求 **が含** まれている。 
  
```XML
<UnpinTeamMailbox>
   <EmailAddress/>
</UnpinTeamMailbox>
```

 **UnpinTeamMailboxRequestType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md)
  
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
|検証ファイル  <br/> |messages.xsd  <br/> |
|空の場合  <br/> ||
   

