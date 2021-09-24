---
title: Action (SetClientExtensionActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c5624a87-3436-40ce-8d6b-cc01eecab64d
description: Action 要素には、サーバーがアプリで実行Exchangeアクションが含まれる。
ms.openlocfilehash: a0f5c2743ef976db2faddbb7509a8a015ef4dd8f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510380"
---
# <a name="action-setclientextensionactiontype"></a>Action (SetClientExtensionActionType)

**Action 要素** には、サーバーがアプリで実行Exchangeアクションが含まれる。 
  
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
|ActionId  <br/> |アクションの識別子を指定します。 この属性は必須です。  <br/> |
|ExtensionId  <br/> |拡張機能の識別子を指定します。 この属性は省略可能です。  <br/> |
   
#### <a name="actionid"></a>ActionId

|**値**|**説明**|
|:-----|:-----|
|Configure  <br/> |構成アクションを示します。  <br/> |
|Install  <br/> |インストール アクションを示します。  <br/> |
|アンインストール  <br/> |アンインストール アクションを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ClientExtension](clientextension.md) <br/> |アプリに関するユーザー情報と構成情報が含まれる。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Actions (ArrayOfSetClientExtensionActionsType)](actions-arrayofsetclientextensionactionstype.md) <br/> |Action 要素の配列 **を指定** します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

