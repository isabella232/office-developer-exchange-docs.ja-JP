---
title: SyncFolderHierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: 55df4d01-e48e-4263-a851-78a66ad1093a
description: SyncFolderHierarchy 要素は、クライアント上のフォルダー階層を同期する要求を定義します。
ms.openlocfilehash: 68b607dbf603e955f74dfaccadd3ce6c4c9fb6ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466648"
---
# <a name="syncfolderhierarchy"></a>SyncFolderHierarchy

**Syncfolderhierarchy**要素は、クライアント上のフォルダー階層を同期する要求を定義します。 
  
```xml
<SyncFolderHierarchy>
   <FolderShape/>   <SyncFolderId/>
   <SyncState/>
</SyncFolderHierarchy>
```

 **SyncFolderHierarchyType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |[Syncfolderhierarchy](syncfolderhierarchy.md)応答に含めるフォルダーのプロパティを識別します。  <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |同期するアイテムを含むフォルダを表します。 この要素は省略できます。  <br/> |
|[SyncState](syncstate-ex15websvcsotherref.md) <br/> |要求が成功するたびに更新される同期データの base64 でエンコードされた形式が含まれます。 これは、同期状態を識別するために使用されます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[SyncFolderHierarchy 操作](syncfolderhierarchy-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

