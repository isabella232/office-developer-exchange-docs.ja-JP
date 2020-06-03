---
title: PrincipalName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PrincipalName
api_type:
- schema
ms.assetid: 88c142d4-0bc7-43ea-a997-d7200664d900
description: PrincipalName 要素は、Exchange の偽装に使用されるアカウントのユーザープリンシパル名 (UPN) を表します。
ms.openlocfilehash: 31412c1461264e28bf8d52c957a457e8d1e847ef
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44440191"
---
# <a name="principalname"></a>PrincipalName

**PrincipalName**要素は、Exchange の偽装に使用されるアカウントのユーザープリンシパル名 (UPN) を表します。 
  
```xml
<PrincipalName/>
```

 **PrincipalNameType**
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
   
## <a name="text-value"></a>テキスト値

Text 値は、ユーザーの UPN を表します。 この値は、Active Directory ディレクトリサービスのユーザーオブジェクトに存在します。 これには、次の形式で、ユーザーアカウントが存在するドメインを識別するユーザーログオン名とドメイン名が含まれています `someone@example.com` 。
  
## <a name="remarks"></a>注釈

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

