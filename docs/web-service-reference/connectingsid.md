---
title: ConnectingSID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectingSID
api_type:
- schema
ms.assetid: 56d6aa52-8fa6-4773-9046-44a6f4f5d97c
description: ConnectingSID 要素は、ExchangeImpersonation SOAP ヘッダーを使用しているときに偽装するアカウントを表します。
ms.openlocfilehash: f4edf63f129fc769f4a2d710a505b40da4057fab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459280"
---
# <a name="connectingsid"></a>ConnectingSID

**ConnectingSID**要素は、EXCHANGEIMPERSONATION SOAP ヘッダーを使用しているときに偽装するアカウントを表します。 
  
- [ExchangeImpersonation](exchangeimpersonation.md) 
- [ConnectingSID](connectingsid.md)
  
```xml
<ConnectingSID>
   <PrincipalName/>
</ConnectingSID>
```

```xml
<ConnectingSID>
   <SmtpAddress/>
</ConnectingSID>
```

```xml
<ConnectingSID>
    <SID/> 
</ConnectingSID>
```

```xml
<ConnectingSID>
   <PrimarySmtpAddress/>
</ConnectingSID>
```

**ConnectingSIDType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[PrincipalName](principalname.md) <br/> |偽装に使用するアカウントのユーザープリンシパル名 (UPN) を表します。 これは、ユーザーアカウントが存在するドメインの UPN である必要があります。  <br/> |
|[SID](sid.md) <br/> |偽装に使用するアカウントのセキュリティ識別子 (SID) のセキュリティ記述子定義言語 (SDDL) 形式を表します。  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Exchange の偽装に使用するアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。 プライマリ SMTP アドレスが指定されている場合は、ユーザーの SID を取得するために、さらに Active Directory ディレクトリサービス参照にコストがかかります。 使用可能な場合は、SID または UPN を使用することをお勧めします。  <br/> |
|[SmtpAddress](smtpaddress.md) <br/> |Exchange 偽装に使用するアカウントの簡易メール転送プロトコル (SMTP) アドレスを表します。 SMTP アドレスが指定されている場合は、ユーザーの SID を取得するために、さらに Active Directory 参照にコストがかかります。 使用可能な場合は、SID または UPN を使用することをお勧めします。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExchangeImpersonation](exchangeimpersonation.md) <br/> |要求の SOAP ヘッダーで使用されます。 この要素が存在する場合、発信者は**Exchangeimpersonation**要素内に含まれるアカウントを偽装しようとしています。  <br/> この要素の XPath 式を次に示します。  <br/>  `/ExchangeImpersonation` <br/> |
   
## <a name="remarks"></a>注釈

呼び出し元のアカウントには、偽装するメールボックスを含むメールボックスデータベース、または Active Directory ユーザーまたは連絡先オブジェクトのいずれかで、クライアントアクセスサーバーおよび**exch-** **exch**権限が必要です。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS でのサーバー間認証](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

