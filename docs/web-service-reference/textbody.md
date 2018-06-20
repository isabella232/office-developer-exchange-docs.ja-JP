---
title: TextBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820
description: TextBody 要素は、テキストの本文を指定します。
ms.openlocfilehash: 78b18b27891d571605d2eeeeffb5c252cc790c11
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839664"
---
# <a name="textbody"></a>TextBody

**TextBody**要素は、テキストの本文を指定します。 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|BodyTypeType  <br/> |本文の種類を示します。 **BodyTypeType**属性の**テキスト**の値は、プレーン テキスト形式の本文であることを示します。 **BodyTypeType**属性の値を**HTML**の本文が HTML フォーム内でことを示します。 **BodyTypeType**属性が必要です。  <br/> |
|IsTruncated  <br/> |本文の内容が切り詰められたことを示します。 テキスト値が**false**の**IsTruncated**属性のでは、本文の内容は切り捨てられましたしないことを示します。 テキスト本文の長さは、 [MaximumBodySize](maximumbodysize.md)要素で設定された値より長い場合、正規化された本文は切り捨てられます。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[項目](item.md) | [連絡先](contact.md) | [メッセージ](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [カレンダー項目](calendaritem.md) | [PostItem](postitem.md) | [タスク](task.md)
  
## <a name="text-value"></a>テキスト値

**TextBody**要素のテキスト値は、項目のテキストの本文です。 
  
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
   

