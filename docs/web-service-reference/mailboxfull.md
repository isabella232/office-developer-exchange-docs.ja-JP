---
title: MailboxFull
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxFull
api_type:
- schema
ms.assetid: 38b28c9b-9da2-4d6a-9cda-9c393986575b
description: MailboxFull 要素は、受信者のメールボックスがいっぱいになっているかどうかを示します。
ms.openlocfilehash: f336f1eda122bb170aafb22a028e3faf84f4d782
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465976"
---
# <a name="mailboxfull"></a>MailboxFull

**MailboxFull**要素は、受信者のメールボックスがいっぱいになっているかどうかを示します。 
  
```XML
<MailboxFull>true | false</MailboxFull>
```

**Boolean**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[メールヒント](mailtips.md) <br/> |さまざまな種類のメールヒントの値を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素は、 **true**または**false**のいずれかになります。 値**true**は、メールボックスが容量に達したことを示します。値が**false**の場合は、容量に達していないことを示します。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

