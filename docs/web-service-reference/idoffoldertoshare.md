---
title: IdOfFolderToShare
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IdOfFolderToShare
api_type:
- schema
ms.assetid: 199d1839-f061-4070-a977-874b0c08e5be
description: IdOfFolderToShare 要素は、共有されるサーバー上のフォルダーの識別子を表します。
ms.openlocfilehash: 93a4740d9adefbb35aae071f0a6bfcb4b2021b4d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457628"
---
# <a name="idoffoldertoshare"></a>IdOfFolderToShare

**IdOfFolderToShare**要素は、共有されるサーバー上のフォルダーの識別子を表します。 
  
```
<IdOfFolderToShare Id="" ChangeKey="" />
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |Exchange ストア内のフォルダーを識別する文字列を格納します。 この属性は必須です。  <br/> |
|ChangeKey  <br/> |Id 属性によって識別されるフォルダーのバージョンを識別する文字列を格納します。 この属性は省略可能です。 この属性を使用して、適切なバージョンのフォルダーが使用されていることを確認します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetSharingMetadata](getsharingmetadata.md) <br/> |共有への招待を識別する非透過の認証トークンを取得する要求を定義します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetSharingMetadata 操作](getsharingmetadata-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

