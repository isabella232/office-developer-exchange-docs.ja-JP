---
title: InvalidRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipient
api_type:
- schema
ms.assetid: 9e2d3433-22d7-444b-9883-e5649297d8fe
description: InvalidRecipient 要素には、無効な受信者の SMTP アドレスと、受信者が無効である理由に関する情報が含まれています。
ms.openlocfilehash: f301b31c1054625151ce90e41fca5e3efc21f473
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526551"
---
# <a name="invalidrecipient"></a>InvalidRecipient

**Invalidrecipient**要素には、無効な受信者の SMTP アドレスと、受信者が無効である理由に関する情報が含まれています。 
  
```XML
<InvalidRecipient>
   <SmtpAddress/>
   <ResponseCode/>
   <MessageText/>
</InvalidRecipient>

```

 **Invalid受信者の種類**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SmtpAddress](smtpaddress.md) <br/> |無効な受信者の SMTP アドレスを含みます。 この要素は必須です。  <br/> |
|[応答 Secmode (Invalid受信者応答 Secodetype)](responsecode-invalidrecipientresponsecodetype.md) <br/> |要求で発生した特定のエラーを識別するエラーコードを提供します。 この要素は必須です。  <br/> |
|[MessageText](messagetext.md) <br/> |応答の状態を説明するテキストを提供します。 この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[InvalidRecipients](invalidrecipients.md) <br/> |無効なフォルダー共有要求の受信者を表します。  <br/> |
   
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



[GetSharingMetadata 操作](getsharingmetadata-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

