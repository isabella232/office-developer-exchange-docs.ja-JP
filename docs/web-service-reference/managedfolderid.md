---
title: ManagedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ManagedFolderId
api_type:
- schema
ms.assetid: 3efb7abb-0e91-4d8a-9fa2-3dec8bd17c30
description: ManagedFolderId 要素には、管理フォルダーのフォルダー ID が含まれています。
ms.openlocfilehash: acdb69f82678633baff12c46494c39015c36d233
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832340"
---
# <a name="managedfolderid"></a>ManagedFolderId

**ManagedFolderId**要素には、管理フォルダーのフォルダー ID が含まれています。 
  
```xml
<ManagedFolderId/>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |管理フォルダーに関する情報が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、この要素の必要があります。
  
## <a name="remarks"></a>備考

**Guid**プロパティによって取得されるのと同じでは識別子の値を**ManagedFolderId** `Get-ManagedFolder` Microsoft Windows Powershell コマンドです。 また、Active Directory ディレクトリ サービスの管理対象フォルダーの**objectGUID**属性の値です。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[CreateManagedFolder 操作](createmanagedfolder-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[フォルダーを削除します。](http://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)
  
[管理フォルダーを追加します。](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

