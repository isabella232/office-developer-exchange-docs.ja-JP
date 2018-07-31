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
description: ConnectingSID 要素は、ExchangeImpersonation SOAP ヘッダーを使用する際に偽装するアカウントを表します。
ms.openlocfilehash: a30f11721506989a84f52dd04c328974f4483956
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354338"
---
# <a name="connectingsid"></a>ConnectingSID

**ConnectingSID**要素は、ExchangeImpersonation SOAP ヘッダーを使用する際に偽装するアカウントを表します。 
  
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

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[PrincipalName](principalname.md) <br/> |偽装のために使用するアカウントのユーザー プリンシパル名 (UPN) を表します。 UPN ドメイン ユーザー アカウントが存在する可能性があります。  <br/> |
|[SID](sid.md) <br/> |偽装に使用するアカウントのセキュリティ識別子 (SID) のセキュリティ記述子定義言語 (SDDL) 形式を表します。  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Exchange 偽装のために使用するアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。 プライマリ SMTP アドレスが指定されている場合、ユーザーの SID を取得するために Active Directory ディレクトリ サービスの参照は、追加のコストがかかります。 可能な場合、SID または UPN を使用することをお勧めします。  <br/> |
|[SmtpAddress](smtpaddress.md) <br/> |Exchange 偽装のために使用するアカウントの簡易メール転送プロトコル (SMTP) アドレスを表します。 SMTP アドレスが指定されている場合、ユーザーの SID を取得するために、追加の Active Directory 検索のコストがかかります。 可能な場合、SID または UPN を使用することをお勧めします。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExchangeImpersonation](exchangeimpersonation.md) <br/> |要求の SOAP ヘッダーで使用されます。 この要素が存在する場合、呼び出し元が**ExchangeImpersonation**要素内に含まれているアカウントを偽装するとしています。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/ExchangeImpersonation` <br/> |
   
## <a name="remarks"></a>注釈

呼び出し元のアカウントが必要でクライアント アクセス サーバーと**ms-exch-MayImpersonate** **ms の偽装 exch**上かを偽装するメールボックスを含むメールボックス データベースまたは Active Directory のユーザーまたは連絡先オブジェクトです。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS でのサーバーからサーバーへの承認](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

