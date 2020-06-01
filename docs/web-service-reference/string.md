---
title: String
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- String
api_type:
- schema
ms.assetid: e6e362b1-4526-49e1-b283-1c4bc4295874
description: String 要素は、アイテム、連絡先、タスク、会話で使用される文字列を表します。
ms.openlocfilehash: fbb4219d35c4acdc2c80b21b73e6479a2ef317f7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463105"
---
# <a name="string"></a>String

**String**要素は、アイテム、連絡先、タスク、会話で使用される文字列を表します。 
  
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
|[Categories](categories-ex15websvcsotherref.md) <br/> |メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションが含まれています。  <br/> |
|[Children](children.md) <br/> |連絡先の子の名前を含みます。  <br/> |
|[Companies](companies.md) <br/> |連絡先またはタスクに関連付けられている会社のコレクションを表します。  <br/> |
|[連絡先](contacts-ex15websvcsotherref.md) <br/> |タスクに関連付けられている連絡先の一覧が含まれています。  <br/> |
|[GlobalCategories](globalcategories.md) <br/> |メールボックス内のすべての会話アイテムのカテゴリリストが保存されています。  <br/> |
|[GlobalUniqueRecipients](globaluniquerecipients.md) <br/> |メールボックス全体で集約された会話の受信者の一覧が含まれています。  <br/> |
|[GlobalUniqueSenders](globaluniquesenders.md) <br/> |メールボックス内のスレッドアイテムのすべての送信者の一覧が含まれています。  <br/> |
|[GlobalUniqueUnreadSenders](globaluniqueunreadsenders.md) <br/> |メールボックス内のすべてのフォルダーにわたって、この会話で現在未読のメッセージを送信したすべてのユーザーの一覧が含まれています。  <br/> |
|[ItemClasses](itemclasses.md) <br/> |条件または例外を適用するために、受信メッセージにスタンプする必要があるアイテムクラスのリストが含まれています。  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |条件または例外を適用するために、受信メッセージにスタンプする必要があるメッセージ分類の一覧が含まれています。  <br/> |
|[UniqueRecipients](uniquerecipients.md) <br/> |会話の受信者のリストが含まれます。 この要素は値の取得のみ可能です。  <br/> |
|[UniqueSenders](uniquesenders.md) <br/> |現在のフォルダー内のスレッドアイテムのすべての送信者の一覧が含まれています。 この要素は値の取得のみ可能です。  <br/> |
|[UniqueUnreadSenders](uniqueunreadsenders.md) <br/> |現在のフォルダーで、この会話で現在未読のメッセージを送信したすべてのユーザーの一覧が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は、カテゴリ、連絡先の子、会社、スレッドの一意の受信者、またはタスクに関連付けられている連絡先を表す文字列です。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[FindConversation 操作](findconversation-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

