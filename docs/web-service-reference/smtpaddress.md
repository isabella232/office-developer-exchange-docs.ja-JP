---
title: SmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SmtpAddress
api_type:
- schema
ms.assetid: 779305a6-ad1e-424e-8a69-4e3bef61d787
description: SmtpAddress 要素は、偽装に使用するアカウントの簡易メール転送プロトコル (SMTP) アドレス、または予定表または連絡先共有要求の SMTP (簡易メール転送プロトコル) 受信者アドレスを表します。
ms.openlocfilehash: c10e18ce77a1002a9c7a94718e8e9a2bd3877d8d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539088"
---
# <a name="smtpaddress"></a>SmtpAddress

**SmtpAddress** 要素は、偽装に使用するアカウントの簡易メール転送プロトコル (SMTP) アドレス、または予定表または連絡先共有要求の SMTP (簡易メール転送プロトコル) 受信者アドレスを表します。 
  
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
|[ConnectingSID](connectingsid.md) <br/> |ExchangeImpersonation SOAP ヘッダーを使用している場合に偽装するアカウントを表します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[InvalidRecipient](invalidrecipient.md) <br/> |予定表共有メッセージまたは連絡先共有メッセージの無効な受信者を表します。  <br/> |
|[Recipients (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |共有フォルダーへのアクセスを許可する受信者のコレクションを表します。  <br/> |
|[GetSharingFolder](getsharingfolder.md) <br/> |指定した共有フォルダーのローカル フォルダー識別子を取得する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

SMTP アドレスを表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

