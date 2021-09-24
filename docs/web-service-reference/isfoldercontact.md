---
title: IsFolderContact
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsFolderContact
api_type:
- schema
ms.assetid: 8b456255-f4ae-4ca0-845a-13c195f1c867
description: IsFolderContact 要素は、ユーザーがフォルダーの連絡先であるかどうかを示します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。
ms.openlocfilehash: 21f5f55a07b6f5acc6310398a7578154b3428265
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522972"
---
# <a name="isfoldercontact"></a>IsFolderContact

**IsFolderContact** 要素は、ユーザーがフォルダーの連絡先であるかどうかを示します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。 
  
```xml
<IsFolderContact/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アクセス許可](permission.md) <br/> |ユーザーがフォルダーに対して持つアクセスを定義します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[CalendarPermission](calendarpermission.md) <br/> |ユーザーが予定表フォルダーに対して持つアクセスを定義します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

true のテキスト **値は** 、ユーザーが指定したフォルダーの連絡先を示します。 false の **値は** 、ユーザーが指定したフォルダーの連絡先ではないかどうかを示します。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[アクセス許可Folder-Level設定する](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

