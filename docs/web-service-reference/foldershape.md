---
title: FolderShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderShape
api_type:
- schema
ms.assetid: 244f4f46-a33d-4764-92e3-1bddb4dc6a49
description: FolderShape 要素は、GetFolder、FindFolder、または SyncFolderHierarchy の応答に含めるフォルダーのプロパティを識別します。
ms.openlocfilehash: 8ebdd70ef13ee9f0cce9020b9212576cba782be4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760582"
---
# <a name="foldershape"></a>FolderShape

**FolderShape**要素は、 [GetFolder](getfolder.md)、 [FindFolder](findfolder.md)、または[SyncFolderHierarchy](syncfolderhierarchy.md)の応答に含めるフォルダーのプロパティを識別します。 
  
```xml
<FolderShape>
   <BaseShape/>
   <AdditionalProperties/>
</FolderShape>
```

 **FolderResponseShapeType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[BaseShape](baseshape.md) <br/> |応答で返されるプロパティの基本構成を識別します。  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |応答で返される追加プロパティを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |メールボックス内のフォルダーを識別するための要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/FindFolder` <br/> |
|[GetFolder](getfolder.md) <br/> |Exchange ストアからフォルダーを取得する要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/GetFolder` <br/> |
|[SyncFolderHierarchy](syncfolderhierarchy.md) <br/> |クライアント上のフォルダー階層を同期するための要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/SyncFolderHierarchy` <br/> |
   
## <a name="remarks"></a>備考

**FolderShape**要素は、 [FindFolder](findfolder.md)要素の必須の子要素です。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="example"></a>例

要求の次の例では、[受信トレイ] フォルダーの最初のレベルにあるすべてのフォルダーを検索する方法を示します。
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[FindFolder](findfolder.md)

