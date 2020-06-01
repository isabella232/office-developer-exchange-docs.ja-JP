---
title: IsFolderVisible
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsFolderVisible
api_type:
- schema
ms.assetid: dd611fb5-9424-4ff9-bb27-c882c73c0c74
description: IsFolderVisible 要素は、ユーザーがフォルダーを表示できるかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 7efe7eef3c10027c38a3dad2dd3ec1d8684c322a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459301"
---
# <a name="isfoldervisible"></a>IsFolderVisible

**Isfoldervisible**要素は、ユーザーがフォルダーを表示できるかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
```xml
<IsFolderVisible/>
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
|[アクセス許可](permission.md) <br/> |ユーザーがフォルダーに対して持つアクセス許可を定義します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[CalendarPermission](calendarpermission.md) <br/> |ユーザーが予定表フォルダーに対して持っているアクセス権を定義します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値が**true の場合**は、ユーザーがフォルダーを表示できることを示します。 値が**false**の場合は、ユーザーがフォルダーを表示できないことを示します。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[フォルダーレベルのアクセス許可を設定する](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

