---
title: SecurityIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SecurityIdentifier
api_type:
- schema
ms.assetid: f7656729-f2c9-41cc-b1ec-60f480fc4dab
description: SecurityIdentifier 要素は、セキュリティ識別子 (SID) のセキュリティ記述子定義言語 (SDDL) 形式を表します。
ms.openlocfilehash: c18d7d4505c618792497c32c7499eab9ac82989e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833314"
---
# <a name="securityidentifier"></a>SecurityIdentifier

**SecurityIdentifier**要素は、セキュリティ識別子 ( [SID](sid.md)) のセキュリティ記述子定義言語 (SDDL) 形式を表します。
  
```xml
<SecurityIdentifier/>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GroupIdentifier](groupidentifier.md) <br/> |1 つのセキュリティ識別子と、アカウントがメンバーである Active Directory オブジェクト グループの属性を表します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/SerializedSecurityContext/GroupSids/GroupIdentifier[i]` <br/> |
|[RestrictedGroupIdentifier](restrictedgroupidentifier.md) <br/> |グループのセキュリティ識別子とユーザーのトークン内の制限されたグループの属性を表します。  <br/> |
   
## <a name="remarks"></a>備考

Simple Object Access Protocol (SOAP) ヘッダーには、この要素を使用します。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

