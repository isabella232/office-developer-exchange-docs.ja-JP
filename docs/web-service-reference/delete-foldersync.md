---
title: (集合的) を削除します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- schema
ms.assetid: c4397d91-43ef-40a9-a80e-d31501a33caa
description: ローカル クライアント ストアで削除するのには 1 つのフォルダーを識別する要素を削除します。
ms.openlocfilehash: 5cad36c6fcff782195fdb285e2d3c4f3c5ec0f1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/15/2018
ms.locfileid: "19759957"
---
# <a name="delete-foldersync"></a>(集合的) を削除します。

要素の**削除**は、ローカル クライアント ストアで削除するのには 1 つのフォルダーを識別します。 
  
- [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)  
- [ResponseMessages](responsemessages.md)  
- [SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)  
- [(階層) の変更](changes-hierarchy.md)  
- [(集合的) を削除します。](delete-foldersync.md)
  
```xml
<Delete>
   <FolderId/>
</Delete>
```

**SyncFolderHierarchyDeleteType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[フォルダー Id](folderid.md) <br/> |フォルダーの識別子と変更キーが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[(階層) の変更](changes-hierarchy.md) <br/> |クライアント上のフォルダーや Microsoft Exchange Server 2007 を実行しているコンピューター上のフォルダー間の相違点の種類を表すの種類の変更の順序付けされた配列が含まれています。  <br/> |
   
## <a name="remarks"></a>Remarks

EWS 仮想ディレクトリのクライアント アクセス サーバーの役割がインストールされている Exchange 2007 コンピューターには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [SyncFolderHierarchy 操作](syncfolderhierarchy-operation.md)
- 
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

