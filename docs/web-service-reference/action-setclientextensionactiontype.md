---
title: アクション (SetClientExtensionActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c5624a87-3436-40ce-8d6b-cc01eecab64d
description: Action 要素には、アプリケーションに対して、Exchange server が実行するアクションが含まれています。
ms.openlocfilehash: a231cedfa6e4759dabfcbecfbe9a9b851f834247
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759273"
---
# <a name="action-setclientextensionactiontype"></a>アクション (SetClientExtensionActionType)

**Action**要素には、アプリケーションに対して、Exchange server が実行するアクションが含まれています。 
  
```XML
<Action ActionId="" ExtensionId="">
   <ClientExtension/>
</Action>
```

 **SetClientExtensionActionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ActionId  <br/> |アクションの識別子を指定します。 この属性は、必要があります。  <br/> |
|ExtensionId  <br/> |拡張機能の識別子を指定します。 この属性は、省略可能です。  <br/> |
   
#### <a name="actionid"></a>ActionId

|**値**|**説明**|
|:-----|:-----|
|構成します。  <br/> |構成の操作を示します。  <br/> |
|インストール  <br/> |インストール アクションを示します。  <br/> |
|アンインストール  <br/> |アンインストール アクションを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ClientExtension](clientextension.md) <br/> |アプリケーションのユーザーおよび構成情報が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アクション (ArrayOfSetClientExtensionActionsType)](actions-arrayofsetclientextensionactionstype.md) <br/> |**アクション**要素の配列を指定します。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

