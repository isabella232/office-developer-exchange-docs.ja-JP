---
title: MailboxSearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ef4a4203-61e5-46b8-9fa4-d1a10e785aa2
description: MailboxSearchScope 要素は、メールボックスの検出検索用の検索範囲を指定します。
ms.openlocfilehash: 657e6dfd4eb6c6c0eabb18546e7090c524e28e5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832297"
---
# <a name="mailboxsearchscope"></a>MailboxSearchScope

**MailboxSearchScope**要素は、メールボックスの検出検索用の検索範囲を指定します。 
  
```XML
<MailboxSearchScope>
   <Mailbox/>
   <SearchScope/>
<MailboxSearchScope>
```

**MailboxSearchScopeType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[メールボックス (文字列)](mailbox-string.md) | [SearchScope](searchscope.md)
  
### <a name="parent-elements"></a>親要素

[MailboxSearchScopes](mailboxsearchscopes.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> ||
   

