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
description: SmtpAddress 要素では、偽装に使用するアカウントの簡易メール転送プロトコル (SMTP) アドレス、または予定表または連絡先の共有の依頼の簡易メール転送プロトコル (SMTP) 受信者のアドレスを表します。
ms.openlocfilehash: 39588f0892cdcec819a1972547155730be5785f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833511"
---
# <a name="smtpaddress"></a>SmtpAddress

**SmtpAddress**要素では、偽装に使用するアカウントの簡易メール転送プロトコル (SMTP) アドレス、または予定表または連絡先の共有の依頼の簡易メール転送プロトコル (SMTP) 受信者のアドレスを表します。 
  
```xml
<SmtpAddress/>
```

**SmtpAddressType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |ExchangeImpersonation SOAP ヘッダーを使用する際に偽装するアカウントを表します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[InvalidRecipient](invalidrecipient.md) <br/> |予定表の共有または共有メッセージを取引先担当者の無効な受信者を表します。  <br/> |
|[受信者 (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |共有フォルダーへのアクセスを許可する受信者のコレクションを表します。  <br/> |
|[GetSharingFolder](getsharingfolder.md) <br/> |指定した共有フォルダーのローカル フォルダーの識別子を取得する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

SMTP アドレスを表す文字列値は、必要があります。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

