---
title: UserMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 1d47141c-3c3f-45b8-90c5-33a44adb34b2
description: UserMailbox 要素は、ユーザー メールボックスを識別します。
ms.openlocfilehash: c2a66b23de5e4b312f60019f0b4ecfb4088b3da2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542618"
---
# <a name="usermailbox"></a>UserMailbox

**UserMailbox 要素は**、ユーザー メールボックスを識別します。 
  
```XML
<UserMailbox Id="" IsArchive=""/>
```

 **UserMailboxType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |Id 属性のテキスト **値** は、メールボックスの識別子です。  <br/> |
|IsArchive  <br/> |**IsArchive 属性のテキスト値は**、メールボックスがアーカイブ メールボックスであるかどうかを示します。 **IsArchive** 属性 **のテキスト値が true** の場合は、メールボックスがアーカイブ メールボックスです。 **IsArchive** **属性の** 値 false は、メールボックスがプライマリ メールボックスかどうかを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[メールボックス (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md)  | [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |true  <br/> |
   

