---
title: TextBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820
description: TextBody 要素は、テキスト本文を指定します。
ms.openlocfilehash: c0002785fb990a251267218f7a5f232e521db41a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459484"
---
# <a name="textbody"></a>TextBody

**Textbody**要素は、テキスト本文を指定します。 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|BodyTypeType  <br/> |本文の種類を示します。 **Bodytypetype**属性の**テキスト**の値は、本文がプレーンテキスト形式であることを示します。 **Bodytypetype**属性の**html**の値は、本文が HTML 形式であることを示します。 **Bodytypetype**属性は必須です。  <br/> |
|Istrがありません  <br/> |本文の内容が切り捨てられていることを示します。 **Istruncated** attribute のテキスト値が**false**の場合は、本文のコンテンツが切り捨てられていないことを示します。 テキストの本文の長さが[Maximumbodysize](maximumbodysize.md)要素で設定された値よりも長い場合は、正規化された本文が切り捨てられます。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[アイテム](item.md)  | [連絡先](contact.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [DistributionList](distributionlist.md)  | [Calendaritem](calendaritem.md)  | [Postitem](postitem.md)  | [タスク](task.md)
  
## <a name="text-value"></a>テキスト値

**Textbody**要素のテキスト値は、アイテムの本文です。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   

