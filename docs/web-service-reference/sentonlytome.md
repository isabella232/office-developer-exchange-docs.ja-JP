---
title: SentOnlyToMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentOnlyToMe
api_type:
- schema
ms.assetid: b6d4dea5-812d-4b29-917d-071ebd7ddd92
description: SentOnlyToMe 要素は、メールボックスの所有者が ToRecipients プロパティを適用する場合の条件または例外の順序で受信メッセージの 1 つだけにするかどうかを示します。
ms.openlocfilehash: 91c31069652a35dc7a38ad6b6e1512cc07d67a98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833353"
---
# <a name="sentonlytome"></a>SentOnlyToMe

**SentOnlyToMe**要素は、メールボックスの所有者が**ToRecipients**プロパティを適用する場合の条件または例外の順序で受信メッセージの 1 つだけにするかどうかを示します。 
  
```XML
<SentOnlyToMe/>true | false</SentOnlyToMe>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[条件](conditions.md) <br/> |条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。  <br/> |
|[Exceptions](exceptions.md) <br/> |受信トレイ ルールの使用可能なルールの例外条件をすべてを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**True**の場合、テキスト値は、メールボックスの所有者は**ToRecipients**プロパティを適用する場合の条件または例外の順序で受信メッセージの 1 つのみである必要があることを示します。 **False**の値では、メールボックスの所有者では、 **ToRecipients**プロパティを適用する場合の条件または例外の順序で受信メッセージの 1 つにしかならないということを示します。 
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

