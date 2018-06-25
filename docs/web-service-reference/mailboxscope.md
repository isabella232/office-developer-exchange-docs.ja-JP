---
title: MailboxScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: MailboxScope 要素は、検索、または会話をフェッチする必要があります、プライマリ メールボックス、アーカイブ メールボックス、または両方のプライマリ、メールボックスをアーカイブするかどうかを識別します。
ms.openlocfilehash: 89c9776079d686b114d6b744150f1c6df3711eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832293"
---
# <a name="mailboxscope"></a>MailboxScope

**MailboxScope**要素は、検索、または会話をフェッチする必要があります、プライマリ メールボックス、アーカイブ メールボックス、または両方のプライマリ、メールボックスをアーカイブするかどうかを識別します。 
  
```XML
<MailboxScope> PrimaryOnly | ArchiveOnly | All </MailboxScope>
```

**MailboxSearchLocationType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[FindConversation](findconversation.md) | [GetConversationItems](getconversationitems.md) | [(ConversationType) の会話](conversation-conversationtype.md)
  
## <a name="text-value"></a>テキスト値

**MailboxScope**要素のテキスト値は、検索のスコープをまたはいずれかのプライマリ メールボックス間での会話でアーカイブ メールボックス、または両方のプライマリおよびアーカイブ メールボックス アイテムを取得します。 **PrimaryOnly**のテキスト値は、ユーザーのプライマリ メールボックスを対象とする範囲を示します。 **ArchiveOnly**のテキスト値は、ユーザーのアーカイブ メールボックスを対象とする範囲を示します。 **すべて**のテキスト値は、プライマリ メールボックスとアーカイブ メールボックスの両方を対象とする範囲を示します。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

