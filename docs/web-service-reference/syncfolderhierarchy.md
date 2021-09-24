---
title: SyncFolderHierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: 55df4d01-e48e-4263-a851-78a66ad1093a
description: SyncFolderHierarchy 要素は、クライアント上のフォルダー階層を同期する要求を定義します。
ms.openlocfilehash: ebe8ecd613fee02275326be6377544959f85afb5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531515"
---
# <a name="syncfolderhierarchy"></a>SyncFolderHierarchy

**SyncFolderHierarchy 要素** は、クライアント上のフォルダー階層を同期する要求を定義します。 
  
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
|[FolderShape](foldershape.md) <br/> |[SyncFolderHierarchy](syncfolderhierarchy.md)応答に含めるフォルダー プロパティを識別します。  <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |同期するアイテムを含むフォルダーを表します。 この要素は省略できます。  <br/> |
|[SyncState](syncstate-ex15websvcsotherref.md) <br/> |要求が成功した後に更新される同期データの base64 エンコード形式が含まれる。 これは、同期状態を識別するために使用されます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[SyncFolderHierarchy 操作](syncfolderhierarchy-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

