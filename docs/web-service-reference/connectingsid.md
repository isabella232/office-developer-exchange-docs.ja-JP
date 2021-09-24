---
title: ConnectingSID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConnectingSID
api_type:
- schema
ms.assetid: 56d6aa52-8fa6-4773-9046-44a6f4f5d97c
description: ConnectingSID 要素は、ExchangeImpersonation SOAP ヘッダーを使用するときに偽装するアカウントを表します。
ms.openlocfilehash: 21cfcfc3590ea5a8b8ca5b53dfdb403e108e37f7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515972"
---
# <a name="connectingsid"></a>ConnectingSID

**ConnectingSID** 要素は、ExchangeImpersonation SOAP ヘッダーを使用するときに偽装するアカウントを表します。 
  
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
|[PrincipalName](principalname.md) <br/> |偽装に使用するアカウントのユーザー プリンシパル名 (UPN) を表します。 これは、ユーザー アカウントが存在するドメインの UPN である必要があります。  <br/> |
|[SID](sid.md) <br/> |偽装に使用するアカウントのセキュリティ識別子 (SID) のセキュリティ記述子定義言語 (SDDL) 形式を表します。  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |ユーザー偽装に使用するアカウントのプライマリ簡易メール転送プロトコル (SMTP) Exchangeします。 プライマリ SMTP アドレスが指定されている場合は、ユーザーの SID を取得するために追加の Active Directory ディレクトリ サービス参照のコストがかかります。 SID または UPN が使用可能な場合は、使用することをお勧めします。  <br/> |
|[SmtpAddress](smtpaddress.md) <br/> |偽装に使用するアカウントの簡易メール転送プロトコル (SMTP) Exchangeします。 SMTP アドレスを指定すると、ユーザーの SID を取得するために追加の Active Directory 参照が必要になります。 SID または UPN が使用可能な場合は、使用することをお勧めします。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExchangeImpersonation](exchangeimpersonation.md) <br/> |要求の SOAP ヘッダーで使用されます。 この要素が存在する場合、呼び出し元は **ExchangeImpersonation** 要素内に含まれるアカウントを偽装しようとしている。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/ExchangeImpersonation` <br/> |
   
## <a name="remarks"></a>注釈

呼び出し元アカウントには、クライアント アクセス サーバー上の **ms-exch 偽装** 権限と、偽装するメールボックスを含むメールボックス データベースまたは Active Directory ユーザーまたは連絡先オブジェクトの **ms-exch-MayImpersonate** 権限が必要です。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS でのサーバー間認証](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

