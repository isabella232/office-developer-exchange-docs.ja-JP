---
title: GroupIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupIdentifier
api_type:
- schema
ms.assetid: bdc6fc1e-4979-42da-a35b-e3017988c7d3
description: GroupIdentifier 要素は、アカウントがメンバーである Active Directory ディレクトリサービスオブジェクトグループの単一のセキュリティ識別子と属性を表します。
ms.openlocfilehash: 8b427b9228cc5e66f46f70389acf2fa4bcd283b3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530804"
---
# <a name="groupidentifier"></a>GroupIdentifier

**GroupIdentifier**要素は、アカウントがメンバーである Active Directory ディレクトリサービスオブジェクトグループの単一のセキュリティ識別子と属性を表します。 
  
```xml
<GroupIdentifier>
   <SecurityIdentifier/>
</GroupIdentifier>
```

 **SidAndAttributesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**属性** <br/> |グループの属性が含まれます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SecurityIdentifier](securityidentifier.md) <br/> |グループを表すセキュリティ識別子 ([SID](sid.md)) のセキュリティ記述子定義言語 (SDDL) 形式を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GroupSids](groupsids.md) <br/> |トークンのシリアル化のためのアカウントトークンを構成する Active Directory グループオブジェクトのセキュリティ識別子のコレクションを表します。 トークンのシリアル化はサポートされていません。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

