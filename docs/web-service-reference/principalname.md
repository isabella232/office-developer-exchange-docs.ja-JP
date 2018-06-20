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
description: PrincipalName 要素は、Exchange の偽装に使用するアカウントのユーザー プリンシパル名 (UPN) を表します。
ms.openlocfilehash: d8557ce0435a11a5602372517db1f576028a9c97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832882"
---
# <a name="principalname"></a>PrincipalName

**PrincipalName**要素は、Exchange の偽装に使用するアカウントのユーザー プリンシパル名 (UPN) を表します。 
  
```xml
<PrincipalName/>
```

 **PrincipalNameType**
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
   
## <a name="text-value"></a>テキスト値

テキスト値は、ユーザーの UPN を表します。 この値は、Active Directory ディレクトリ サービス内のユーザー オブジェクトに存在します。 ユーザー ログオン名とユーザー アカウントが次の形式で、配置されているドメインを識別するドメイン名が含まれます: `someone@example.com`。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[EWS でのサーバーからサーバーへの承認](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

