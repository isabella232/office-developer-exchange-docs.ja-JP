---
title: Member
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Member
api_type:
- schema
ms.assetid: af9c5ff8-02a4-41fc-876d-14ac05f1ee77
description: Member 要素は、配布リストのメンバーを表します。
ms.openlocfilehash: e84223b7c41846ca2f174293bff46a8825777a0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457306"
---
# <a name="member"></a>Member

**Member**要素は、配布リストのメンバーを表します。 
  
```xml
<Member Key="">
   <Mailbox/>
   <Status/>
</Member>
```

**MemberType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|キー  <br/> |配布リストのメンバーの一意の識別子を提供します。 この属性は省略可能です。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[メールボックス](mailbox.md) <br/> |配布リストのメンバーの電子メールアドレスを表します。 この要素は省略できます。  <br/> |
|[Status (MemberStatusType)](status-memberstatustype.md) <br/> |配布リストのメンバーの状態に関する情報を提供します。 この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Members (MemberListType)](members-memberlisttype.md) <br/> |配布リストのメンバーの一覧が含まれています。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

