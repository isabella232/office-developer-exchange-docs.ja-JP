---
title: OriginalRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- OriginalRecipients
api_type:
- schema
ms.assetid: e4af86a5-85af-4239-8055-e29f0acf77c1
description: OriginalRecipients 要素は、最初のメッセージ受信者の電子メール アドレスの一覧を表します。
ms.openlocfilehash: 38066a14cbac02ead7e56cef3d448509302d545d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546141"
---
# <a name="originalrecipients"></a>OriginalRecipients

**OriginalRecipients** 要素は、最初のメッセージ受信者の電子メール アドレスの一覧を表します。 
  
```XML
<OriginalRecipients>
   <Address/>
</OriginalRecipients>
```

 **ArrayOfEmailAddressesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Address (EmailAddressType)](address-emailaddresstype.md) <br/> |完全に解決された電子メール アドレスが含まれる。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MessageTrackingReport](messagetrackingreport.md) <br/> |[GetMessageTrackingReport](getmessagetrackingreport-operation.md)操作で返される 1 つのメッセージを格納します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

