---
title: EncryptionMethod (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: bc632c85-ec74-4a00-baec-df5973e032fa
description: EncryptionMethod 要素は、POP、IMAP、および SMTP プロトコルに使用される暗号化方式を表します。
ms.openlocfilehash: 26236d9b08eae1bcabfd9aac59f5b01714ba9841
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530657"
---
# <a name="encryptionmethod-soap"></a>EncryptionMethod (SOAP)

**Encryptionmethod**要素は、POP、IMAP、および SMTP プロトコルに使用される暗号化方式を表します。 
  
```XML
<EncryptionMethod/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ProtocolConnection (SOAP)](protocolconnection-soap.md) <br/> |サーバー Web クライアントのプロトコル接続を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は、POP、IMAP、および SMTP プロトコルに使用される暗号化方法です。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)

