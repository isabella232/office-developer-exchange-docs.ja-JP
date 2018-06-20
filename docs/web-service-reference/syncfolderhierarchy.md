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
description: SyncFolderHierarchy 要素は、クライアント上のフォルダー階層を同期するための要求を定義します。
ms.openlocfilehash: f72640e5605dd83e92cd323cb00e4d2f64406245
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839634"
---
# <a name="syncfolderhierarchy"></a>SyncFolderHierarchy

**SyncFolderHierarchy**要素は、クライアント上のフォルダー階層を同期するための要求を定義します。 
  
```xml
<SyncFolderHierarchy>
   <FolderShape/>   <SyncFolderId/>
   <SyncState/>
</SyncFolderHierarchy>
```

 **SyncFolderHierarchyType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |[SyncFolderHierarchy](syncfolderhierarchy.md)の応答に含めるフォルダーのプロパティを識別します。  <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |同期する項目を含むフォルダーを表します。 この要素はオプションです。  <br/> |
|[同期状態](syncstate-ex15websvcsotherref.md) <br/> |各成功した要求の後に更新された同期データの base64 でエンコードされたフォームが含まれています。 これを使用して、同期の状態を識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[SyncFolderHierarchy 操作](syncfolderhierarchy-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

