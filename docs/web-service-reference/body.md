---
title: 本文
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7851ea9b-9f87-4adc-a26f-7a27df4a9bca
description: Body 要素は、アイテムの本文を指定します。
ms.openlocfilehash: c565c5701ae5bc210cf0a9dc694108752860e24b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529491"
---
# <a name="body"></a>本文

**Body**要素は、アイテムの本文を指定します。 
  
```XML
<Body> BodyType="" IsTruncated="" </Body>
```

 **BodyType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|BodyType  <br/> |本文の種類を指定します。  <br/> |
|Istrがありません  <br/> |本文が切り捨てられるかどうかを示すブール値。  <br/> |
   
#### <a name="bodytype"></a>BodyType

|**値**|**説明**|
|:-----|:-----|
|HTML  <br/> |本文が HTML 形式であることを示します。  <br/> |
|テキスト  <br/> |本文がテキストにあることを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange ストア内の連絡先アイテムを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[Item](item.md) <br/> |Exchange ストア内の汎用アイテムを表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Microsoft Exchange の電子メールメッセージを表します。  <br/> |
|[PostItem](postitem.md) <br/> |Exchange ストア内の投稿アイテムを表します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**Body**要素のテキスト値は、アイテムの本文の内容です。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

