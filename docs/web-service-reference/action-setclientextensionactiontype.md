---
title: Action (SetClientExtensionActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c5624a87-3436-40ce-8d6b-cc01eecab64d
description: Action 要素には、Exchange サーバーがアプリに対して実行するアクションが含まれています。
ms.openlocfilehash: 29579e26377edacb5fb0bb8406144eeb116b8d15
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529687"
---
# <a name="action-setclientextensionactiontype"></a>Action (SetClientExtensionActionType)

**Action**要素には、Exchange サーバーがアプリに対して実行するアクションが含まれています。 
  
```XML
<Action ActionId="" ExtensionId="">
   <ClientExtension/>
</Action>
```

 **SetClientExtensionActionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ActionId  <br/> |アクションの id を指定します。 この属性は必須です。  <br/> |
|ExtensionId  <br/> |拡張機能の識別子を指定します。 この属性は省略可能です。  <br/> |
   
#### <a name="actionid"></a>ActionId

|**値**|**説明**|
|:-----|:-----|
|Configure  <br/> |構成操作を示します。  <br/> |
|Install  <br/> |インストールアクションを示します。  <br/> |
|Uninstall  <br/> |アンインストールアクションを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ClientExtension](clientextension.md) <br/> |アプリに関するユーザーおよび構成情報が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Actions (ArrayOfSetClientExtensionActionsType)](actions-arrayofsetclientextensionactionstype.md) <br/> |**Action**要素の配列を指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

