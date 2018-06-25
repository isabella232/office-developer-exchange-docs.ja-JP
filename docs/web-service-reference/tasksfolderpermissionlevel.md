---
title: TasksFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TasksFolderPermissionLevel
api_type:
- schema
ms.assetid: 0f70b79b-3443-4048-b410-692d4e2464fc
description: TasksFolderPermissionLevel 要素には、既定の仕事フォルダーのアクセス許可が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 49807896f9175bafbef106c41d1c9dff8f6178c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839649"
---
# <a name="tasksfolderpermissionlevel"></a>TasksFolderPermissionLevel

**TasksFolderPermissionLevel**要素には、既定の仕事フォルダーのアクセス許可が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
```xml
<TasksFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</TasksFolderPermissionLevel>
```

**DelegateFolderPermissionLevelType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DelegatePermissions](delegatepermissions.md) <br/> |ユーザーの代理人のアクセス許可レベルの設定が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

アクセス許可レベルを表す文字列値を次の表に一覧します。
  
**アクセス許可レベルのテキスト値**

|**アクセス許可レベル**|**説明**|
|:-----|:-----|
|なし  <br/> |[仕事] フォルダーには、代理ユーザーのアクセス許可がありません。  <br/> |
|Reviewer  <br/> |代理ユーザーは、[仕事] フォルダー内のアイテムを読み取ることができます。  <br/> |
|作成者  <br/> |代理ユーザーは、読み取りし、[仕事] フォルダーにアイテムを作成できます。  <br/> |
|Editor  <br/> |代理ユーザーは読み取り、作成、および [仕事] フォルダー内の項目を変更します。  <br/> |
|カスタム  <br/> |代理ユーザーは、[仕事] フォルダーにカスタム アクセス許可を持ちます。  <br/> |
   
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

- [AddDelegate 操作](adddelegate-operation.md)
- [UpdateDelegate 操作](updatedelegate-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)
- [デリゲートを追加します。](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

