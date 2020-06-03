---
title: PrimarySmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PrimarySmtpAddress
api_type:
- schema
ms.assetid: eee79904-9412-4e61-b9b8-aff0ce25fade
description: PrimarySmtpAddress 要素は、サーバー間の認証または代理人アクセスに使用されるアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。
ms.openlocfilehash: eea995b3e546d7e94e65cf9b230b639a781c4928
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467964"
---
# <a name="primarysmtpaddress"></a>PrimarySmtpAddress

**Primarysmtpaddress**要素は、サーバー間の認証または代理人アクセスに使用されるアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。 
  
```xml
<PrimarySmtpAddress/>
```

 **PrimarySmtpAddressType**
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
|[SerializedSecurityContext](serializedsecuritycontext.md) <br/> |サーバー間認証のトークンシリアル化のために SOAP ヘッダーで使用されます。  <br/> |
|[UserId](userid.md) <br/> |代理ユーザーまたはフォルダーのアクセス許可を持つユーザーを識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

SMTP アドレスを表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

Exchange Web サービスでは、メールボックスのプライマリ SMTP アドレスによってメールボックスが識別される必要があります。 プロキシまたは代替アドレスは受け付けられません。
  
この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[EWS でのサーバー間認証](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)
  
[代理人アクセスを使用する](https://msdn.microsoft.com/library/dfd6b4a3-8fd3-47ba-83c0-52465cb5f3f3%28Office.15%29.aspx)

