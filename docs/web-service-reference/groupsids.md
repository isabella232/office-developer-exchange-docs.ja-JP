---
title: GroupSids
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupSids
api_type:
- schema
ms.assetid: ebb00653-83f0-4080-a902-c38df6719800
description: GroupSids 要素は、Active Directory ディレクトリ サービス グループ オブジェクト セキュリティ識別子のコレクションを表します。
ms.openlocfilehash: c24c8ea3c3b7d37f41986997ed924c951b4a48ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831790"
---
# <a name="groupsids"></a>GroupSids

**GroupSids**要素は、Active Directory ディレクトリ サービス グループ オブジェクト セキュリティ識別子のコレクションを表します。 
  
```xml
<GroupSids>
   <GroupIdentifier/>
</GroupSids>
```

 **NonEmptyArrayOfGroupIdentifiersType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[GroupIdentifier](groupidentifier.md) <br/> |1 つのセキュリティ識別子と、アカウントがメンバーである Active Directory オブジェクト グループの属性を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SerializedSecurityContext](serializedsecuritycontext.md) <br/> |Simple Object Access Protocol (SOAP) ヘッダーでサーバーからサーバーへの認証でトークンのシリアル化のために使用されます。 トークンのシリアル化はサポートされていません。  <br/> |
   
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

