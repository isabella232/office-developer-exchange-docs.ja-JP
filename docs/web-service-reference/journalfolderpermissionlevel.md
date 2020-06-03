---
title: JournalFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- JournalFolderPermissionLevel
api_type:
- schema
ms.assetid: 564525fa-cd95-4c1a-9d6c-3806be664579
description: JournalFolderPermissionLevel 要素には、既定の履歴フォルダーのアクセス許可が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 5c0f30932eb3fbbeef1a8e34611deeb1ffef402c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529050"
---
# <a name="journalfolderpermissionlevel"></a>JournalFolderPermissionLevel

**JournalFolderPermissionLevel**要素には、既定の履歴フォルダーのアクセス許可が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
```xml
<JournalFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</JournalFolderPermissionLevel>
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
|[DelegatePermissions](delegatepermissions.md) <br/> |ユーザーの代理アクセス許可レベルの設定が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に、アクセス許可レベルを表すテキスト値の一覧を示します。
  
**アクセス許可レベルのテキスト値**

|**アクセス許可レベル**|**説明**|
|:-----|:-----|
|なし  <br/> |代理人ユーザーには、履歴フォルダーへのアクセス許可がありません。  <br/> |
|レビュー担当者  <br/> |代理人のユーザーは、履歴フォルダーのアイテムを読み取ることができます。  <br/> |
|設定元  <br/> |代理人のユーザーは、履歴フォルダーのアイテムの読み取りと作成を行うことができます。  <br/> |
|エディター  <br/> |代理人のユーザーは、履歴フォルダーのアイテムの読み取り、作成、および変更を行うことができます。  <br/> |
|Custom  <br/> |代理人ユーザーには、ジャーナルフォルダーに対する独自のアクセス許可があります。  <br/> |
   
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



[AddDelegate 操作](adddelegate-operation.md)
  
[UpdateDelegate 操作](updatedelegate-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[代理人の追加](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

