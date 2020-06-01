---
title: SmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SmtpAddress
api_type:
- schema
ms.assetid: 779305a6-ad1e-424e-8a69-4e3bef61d787
description: SmtpAddress 要素は、偽装に使用されるアカウントの簡易メール転送プロトコル (SMTP) アドレス、または予定表または連絡先共有要求の SMTP (Simple Mail Transfer Protocol) 受信者アドレスを表します。
ms.openlocfilehash: 915ff328cc384c1f2884e9fbea8c10c1ebc79288
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466690"
---
# <a name="smtpaddress"></a>SmtpAddress

**Smtpaddress**要素は、偽装に使用されるアカウントの簡易メール転送プロトコル (smtp) アドレス、または予定表または連絡先共有要求の Smtp (Simple Mail transfer protocol) 受信者アドレスを表します。 
  
```xml
<SmtpAddress/>
```

**SmtpAddressType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |ExchangeImpersonation SOAP ヘッダーを使用しているときに偽装するアカウントを表します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[InvalidRecipient](invalidrecipient.md) <br/> |予定表共有または連絡先共有メッセージの無効な受信者を表します。  <br/> |
|[受信者 (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |共有フォルダーへのアクセスが許可される受信者のコレクションを表します。  <br/> |
|[GetSharingFolder](getsharingfolder.md) <br/> |指定された共有フォルダーのローカルフォルダー識別子を取得する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

SMTP アドレスを表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

