---
title: SyncFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SyncFolderId
api_type:
- schema
ms.assetid: 3645fa03-236d-4e5f-b8b9-5d98f7f35fa2
description: SyncFolderId 要素は、同期するアイテムを含むフォルダーを表します。
ms.openlocfilehash: 018d35ebdcb5afb3de2f1415bc792ecfbd910ffd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517547"
---
# <a name="syncfolderid"></a>SyncFolderId

**SyncFolderId 要素** は、同期するアイテムを含むフォルダーを表します。 
  
```xml
<SyncFolderId>
   <FolderId/>
</SyncFolderId>
```

```xml
<SyncFolderId>
   <DistinguishedFolderId/> 
</SyncFolderId>
```

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |フォルダーの識別子と変更キーを格納します。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |名前で参照できる MicrosoftExchange Server 2007 フォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SyncFolderHierarchy](syncfolderhierarchy.md) <br/> |フォルダー ストア内のフォルダー階層を同期する要求をExchangeします。  <br/> |
|[SyncFolderItems](syncfolderitems.md) <br/> |ストア フォルダー内のアイテムを同期する要求Exchange定義します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [SyncFolderItems 操作](syncfolderitems-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

