---
title: SharingFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingFolderId
api_type:
- schema
ms.assetid: 5ad37ceb-2922-4420-9051-c29d0d57c420
description: SharingFolderId 要素は、共有の関係では、ローカル フォルダーの識別子を表します。
ms.openlocfilehash: e0eb1fbd7155040508daf253f5eb4b1352d7426d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833485"
---
# <a name="sharingfolderid"></a>SharingFolderId

**SharingFolderId**要素は、共有の関係では、ローカル フォルダーの識別子を表します。 
  
```xml
<SharingFolderId Id="" ChangeKey="" />
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |Exchange ストア内のフォルダーを識別する文字列が含まれています。 この属性は、必要があります。  <br/> |
|ChangeKey  <br/> |Id 属性によって識別されるフォルダーのバージョンを識別する文字列が含まれています。 この属性は、省略可能です。 フォルダーの正しいバージョンを使用するかどうかを確認するには、この属性を使用します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RefreshSharingFolder](refreshsharingfolder.md) <br/> |指定したローカル フォルダーを更新する要求を定義します。  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |[GetSharingFolder 操作](getsharingfolder-operation.md)要求に対する応答を定義します。  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[GetSharingFolder の操作](getsharingfolder-operation.md)を要求します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

