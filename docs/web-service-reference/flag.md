---
title: Flag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7b47bc74-a60d-4308-8674-5d52444a1753
description: Flag 要素は、メールボックス アイテムのフラグを指定します。
ms.openlocfilehash: dffc550dc4235c2121b6641f3a6eac30594f75b3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513697"
---
# <a name="flag"></a>Flag

**Flag 要素** は、メールボックス アイテムのフラグを指定します。 
  
```XML
<Flag>
    <FlagStatus/>
    <StartDate/>
    <DueDate/>
    <CompleteDate/>
</Flag>
```

 **FlagType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FlagStatus](flagstatus.md) <br/> |現在のフォルダー内のアイテムの集計フラグの状態を格納します。  <br/> |
|[StartDate](startdate.md) <br/> |アイテムの開始日を表します。  <br/> |
|[DueDate](duedate.md) <br/> |アイテムの期限が設定されている日付を表します。  <br/> |
|[CompleteDate](completedate.md) <br/> |アイテムが完了した日付を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |1 つの会話に適用する 1 つのアクションが含まれる。  <br/> |
|[項目](item.md) <br/> |ストア内の汎用アイテムをExchangeします。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

