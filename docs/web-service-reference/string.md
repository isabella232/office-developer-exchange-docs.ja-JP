---
title: String
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- String
api_type:
- schema
ms.assetid: e6e362b1-4526-49e1-b283-1c4bc4295874
description: String 要素は、アイテム、連絡先、タスク、会話で使用される文字列を表します。
ms.openlocfilehash: dd85cae34ddf829f00660c8b87feb9331505183c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509295"
---
# <a name="string"></a>String

**String 要素** は、アイテム、連絡先、タスク、会話で使用される文字列を表します。 
  
```XML
<String/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Categories](categories-ex15websvcsotherref.md) <br/> |メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを格納します。  <br/> |
|[Children](children.md) <br/> |連絡先の子の名前が含まれる。  <br/> |
|[Companies](companies.md) <br/> |連絡先またはタスクに関連付けられている会社のコレクションを表します。  <br/> |
|[連絡先](contacts-ex15websvcsotherref.md) <br/> |タスクに関連付けられている連絡先の一覧を含む。  <br/> |
|[GlobalCategories](globalcategories.md) <br/> |メールボックス内のすべての会話アイテムのカテゴリ リストが含まれます。  <br/> |
|[GlobalUniqueRecipients](globaluniquerecipients.md) <br/> |メールボックス全体で集計された会話の受信者リストを格納します。  <br/> |
|[GlobalUniqueSenders](globaluniquesenders.md) <br/> |メールボックス内の会話アイテムのすべての送信者の一覧が含まれます。  <br/> |
|[GlobalUniqueUnreadSenders](globaluniqueunreadsenders.md) <br/> |メールボックス内のすべてのフォルダーで、この会話で現在未読のメッセージを送信したすべてのユーザーの一覧が含まれます。  <br/> |
|[ItemClasses](itemclasses.md) <br/> |条件または例外を適用するために受信メッセージにスタンプする必要があるアイテム クラスの一覧が含まれます。  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |条件または例外を適用するために受信メッセージにスタンプする必要があるメッセージ分類の一覧が含まれます。  <br/> |
|[UniqueRecipients](uniquerecipients.md) <br/> |会話の受信者の一覧を格納します。 この要素は読み取り専用です。  <br/> |
|[UniqueSenders](uniquesenders.md) <br/> |現在のフォルダー内の会話アイテムのすべての送信者の一覧が含まれます。 この要素は読み取り専用です。  <br/> |
|[UniqueUnreadSenders](uniqueunreadsenders.md) <br/> |現在のフォルダー内のこの会話で現在未読のメッセージを送信したすべてのユーザーの一覧が含まれます。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は、カテゴリ、連絡先の子、会社、会話の一意の受信者、またはタスクに関連付けられている連絡先を表す文字列です。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web Services をホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[FindConversation 操作](findconversation-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

