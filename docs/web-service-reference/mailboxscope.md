---
title: MailboxScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: MailboxScope 要素は、会話の検索またはフェッチがプライマリメールボックス、アーカイブメールボックス、またはプライマリメールボックスとアーカイブメールボックスのいずれかにまたがる必要があるかどうかを識別します。
ms.openlocfilehash: 92823c06d4fe186917c3cfb532eda821bd6a95a7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455374"
---
# <a name="mailboxscope"></a>MailboxScope

**MailboxScope**要素は、会話の検索またはフェッチがプライマリメールボックス、アーカイブメールボックス、またはプライマリメールボックスとアーカイブメールボックスのいずれかにまたがる必要があるかどうかを識別します。 
  
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

[Findconversation](findconversation.md)  | [GetConversationItems](getconversationitems.md)  | [会話 (ConversationType)](conversation-conversationtype.md)
  
## <a name="text-value"></a>テキスト値

**MailboxScope**要素のテキスト値は、プライマリメールボックス、アーカイブメールボックス、またはプライマリメールボックスとアーカイブメールボックスの両方で、会話内のアイテムを検索または取得するためのスコープです。 Text 値が**Primaryonly**の場合は、ユーザーのプライマリメールボックスを対象とするスコープを示します。 アーカイブのテキスト値は、ユーザーのアーカイブメールボックスを対象とするスコープ**のみ**を示します。 Text 値は、プライマリメールボックスとアーカイブメールボックスの両方をターゲットとするスコープ**を示します**。 
  
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
   

