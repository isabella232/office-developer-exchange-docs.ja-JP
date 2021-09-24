---
title: MailboxScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: MailboxScope 要素は、会話の検索またはフェッチをプライマリ メールボックス、アーカイブ メールボックス、またはプライマリ メールボックスとアーカイブ メールボックスの両方にまたがるべきかどうかを識別します。
ms.openlocfilehash: 705c72ae2aefbb16599f392eb712d080668490b0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522881"
---
# <a name="mailboxscope"></a>MailboxScope

**MailboxScope 要素** は、会話の検索またはフェッチをプライマリ メールボックス、アーカイブ メールボックス、またはプライマリ メールボックスとアーカイブ メールボックスの両方にまたがるべきかどうかを識別します。 
  
```XML
<MailboxScope> PrimaryOnly | ArchiveOnly | All </MailboxScope>
```

**MailboxSearchLocationType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[FindConversation](findconversation.md)  | [GetConversationItems](getconversationitems.md)  | [Conversation (ConversationType)](conversation-conversationtype.md)
  
## <a name="text-value"></a>テキスト値

**MailboxScope** 要素のテキスト値は、プライマリ メールボックス、アーカイブ メールボックス、またはプライマリ メールボックスとアーカイブ メールボックスの両方で会話内のアイテムを検索または取得するスコープです。 **PrimaryOnly のテキスト値は**、ユーザーのプライマリ メールボックスを対象とするスコープを示します。 **ArchiveOnly のテキスト値は**、ユーザーのアーカイブ メールボックスを対象とするスコープを示します。 All のテキスト **値は** 、プライマリ メールボックスとアーカイブ メールボックスの両方を対象とするスコープを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

