---
title: TasksFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TasksFolderPermissionLevel
api_type:
- schema
ms.assetid: 0f70b79b-3443-4048-b410-692d4e2464fc
description: TasksFolderPermissionLevel 要素には、既定の Tasks フォルダーのアクセス許可が含まれています。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。
ms.openlocfilehash: 991b13f9a9f95805b13312712b1f6c5941033c46
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543871"
---
# <a name="tasksfolderpermissionlevel"></a>TasksFolderPermissionLevel

**TasksFolderPermissionLevel** 要素には、既定の Tasks フォルダーのアクセス許可が含まれています。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。 
  
```xml
<TasksFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</TasksFolderPermissionLevel>
```

**DelegateFolderPermissionLevelType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DelegatePermissions](delegatepermissions.md) <br/> |ユーザーの代理人アクセス許可レベルの設定が含まれる。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に、アクセス許可レベルを表すテキスト値を示します。
  
**アクセス許可レベルのテキスト値**

|**アクセス許可レベル**|**説明**|
|:-----|:-----|
|なし  <br/> |代理人ユーザーには、タスク フォルダーへのアクセス許可はありません。  <br/> |
|レビュー担当者  <br/> |代理人ユーザーは、タスク フォルダー内のアイテムを読み取りできます。  <br/> |
|Author  <br/> |代理人ユーザーは、タスク フォルダー内のアイテムの読み取りおよび作成を行うことができます。  <br/> |
|エディター  <br/> |代理人ユーザーは、タスク フォルダー内のアイテムの読み取り、作成、および変更を行うことができます。  <br/> |
|Custom  <br/> |代理人ユーザーは、タスク フォルダーへのカスタム アクセス許可を持ちます。  <br/> |
   
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

- [AddDelegate 操作](adddelegate-operation.md)
- [UpdateDelegate 操作](updatedelegate-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)
- [代理人の追加](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

