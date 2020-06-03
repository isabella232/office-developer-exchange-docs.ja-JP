---
title: 非 Pxcb Ammailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1034b013-ef34-4e72-99b3-38bff475b3e8
description: 非検出応答からサイトメールボックスを削除することにより、クライアントからサイトメールボックスのピン留めを解除する要求が、非 Pxcb Ammailbox 要素に含まれています。
ms.openlocfilehash: a6b01bfa9c5908765ff04ef7f5edbef0b99a9be2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467243"
---
# <a name="unpinteammailbox"></a>非 Pxcb Ammailbox

非**検出**応答からサイトメールボックスを削除することにより、クライアントからサイトメールボックスのピン留めを解除する要求が、非**Pxcb ammailbox**要素に含まれています。 
  
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
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> ||
   

