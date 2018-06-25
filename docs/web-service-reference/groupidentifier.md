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
description: GroupIdentifier 要素は、1 つのセキュリティ識別子と、アカウントがメンバーとして含まれている Active Directory ディレクトリ サービス オブジェクト グループの属性を表します。
ms.openlocfilehash: d73d72979762238ca09496cfbd6636b4ff44a969
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831767"
---
# <a name="groupidentifier"></a>GroupIdentifier

**GroupIdentifier**要素は、1 つのセキュリティ識別子と、アカウントがメンバーとして含まれている Active Directory ディレクトリ サービス オブジェクト グループの属性を表します。 
  
```xml
<GroupIdentifier>
   <SecurityIdentifier/>
</GroupIdentifier>
```

 **SidAndAttributesType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Attributes** <br/> |グループの属性が含まれています。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[SecurityIdentifier](securityidentifier.md) <br/> |グループを表すセキュリティ識別子 ([SID](sid.md)) のセキュリティ記述子定義言語 (SDDL) 形式を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GroupSids](groupsids.md) <br/> |アカウント トークンのトークンのシリアル化を構成する Active Directory グループ オブジェクト セキュリティ識別子のコレクションを表します。 トークンのシリアル化はサポートされていません。  <br/> |
   
## <a name="remarks"></a>備考

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

