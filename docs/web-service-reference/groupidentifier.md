---
title: GroupIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GroupIdentifier
api_type:
- schema
ms.assetid: bdc6fc1e-4979-42da-a35b-e3017988c7d3
description: GroupIdentifier 要素は、アカウントがメンバーである Active Directory ディレクトリ サービス オブジェクト グループの 1 つのセキュリティ識別子と属性を表します。
ms.openlocfilehash: c96d0ca673d9b488266f08abbbd6546aaeb9f5a9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533160"
---
# <a name="groupidentifier"></a>GroupIdentifier

**GroupIdentifier 要素** は、アカウントがメンバーである Active Directory ディレクトリ サービス オブジェクト グループの 1 つのセキュリティ識別子と属性を表します。 
  
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
|**属性** <br/> |グループ属性を含む。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SecurityIdentifier](securityidentifier.md) <br/> |グループを表すセキュリティ識別子 (SID) のセキュリティ記述子定義言語[(SDDL)](sid.md)形式を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GroupSids](groupsids.md) <br/> |トークンのシリアル化のアカウント トークンを構成する Active Directory グループ オブジェクト のセキュリティ識別子のコレクションを表します。 トークンのシリアル化はサポートされていません。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

