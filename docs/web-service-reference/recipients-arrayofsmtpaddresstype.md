---
title: Recipients (ArrayOfSmtpAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Recipients
api_type:
- schema
ms.assetid: cf68417d-85cf-49e0-857a-f987d3675344
description: Recipients 要素は、メッセージの受信者の配列を指定します。
ms.openlocfilehash: 20083c001df5097ded2033bed881ec3a39f98789
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534495"
---
# <a name="recipients-arrayofsmtpaddresstype"></a>Recipients (ArrayOfSmtpAddressType)

**Recipients 要素** は、メッセージの受信者の配列を指定します。 
  
```xml
<Recipients>   <SmtpAddress/></Recipients>
```

 **ArrayOfSmtpAddressType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SmtpAddress](smtpaddress.md) <br/> |予定表または連絡先共有要求の簡易メール転送プロトコル (SMTP) 受信者アドレスを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetSharingMetadata](getsharingmetadata.md) <br/> |共有の招待を識別する不透明な認証トークンを取得する要求を定義します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetSharingMetadata 操作](getsharingmetadata-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

