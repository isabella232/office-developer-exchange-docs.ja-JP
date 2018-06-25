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
description: 文字列要素は、項目、連絡先、タスク、および会話で使用される文字列を表します。
ms.openlocfilehash: 66260c7ebcb56049a78c5eddbe057dfa8d61f193
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833607"
---
# <a name="string"></a>String

**文字列**要素は、項目、連絡先、タスク、および会話で使用される文字列を表します。 
  
```XML
<String/>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Categories](categories-ex15websvcsotherref.md) <br/> |メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションが含まれています。  <br/> |
|[Children](children.md) <br/> |連絡先の子供の名前が含まれています。  <br/> |
|[Companies](companies.md) <br/> |連絡先またはタスクに関連付けられている企業のコレクションを表します。  <br/> |
|[連絡先](contacts-ex15websvcsotherref.md) <br/> |タスクに関連付けられている連絡先の一覧が含まれています。  <br/> |
|[GlobalCategories](globalcategories.md) <br/> |メールボックス内のすべての会話項目のカテゴリの一覧が含まれています。  <br/> |
|[GlobalUniqueRecipients](globaluniquerecipients.md) <br/> |メールボックス間で集計する対話の受信者のリストが含まれています。  <br/> |
|[GlobalUniqueSenders](globaluniquesenders.md) <br/> |メールボックス内のアイテムの会話のすべての送信者の一覧が含まれています。  <br/> |
|[GlobalUniqueUnreadSenders](globaluniqueunreadsenders.md) <br/> |現在この会話で、メールボックス内のすべてのフォルダー間でメッセージを送信したすべての人のリストが含まれています。  <br/> |
|[ItemClasses](itemclasses.md) <br/> |項目のクラスに適用する条件または例外の順序で受信したメッセージにスタンプする必要がありますの一覧が含まれています。  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |適用する場合の条件または例外の順序で受信したメッセージにスタンプする必要がありますメッセージの分類の一覧が含まれています。  <br/> |
|[UniqueRecipients](uniquerecipients.md) <br/> |会話の受信者の一覧が含まれています。 この要素は、読み取り専用です。  <br/> |
|[UniqueSenders](uniquesenders.md) <br/> |会話項目を現在のフォルダー内のすべての送信者の一覧が含まれています。 この要素は、読み取り専用です。  <br/> |
|[UniqueUnreadSenders](uniqueunreadsenders.md) <br/> |現在この会話を [現在のフォルダーにメッセージを送信したすべての人のリストが含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は、連絡先、会社、会話、またはタスクに関連付けられている連絡先の一意の受信者の子カテゴリを表す文字列です。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [FindConversation 操作](findconversation-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

