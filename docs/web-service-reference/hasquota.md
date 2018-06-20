---
title: HasQuota
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HasQuota
api_type:
- schema
ms.assetid: b6e4fef0-92a9-415f-81ae-0c5ecb7c12ad
description: HasQuota 要素は、管理対象のフォルダーがクォータを持つかどうかを示します。
ms.openlocfilehash: 26f14ee7c9d4de267733bca11f7884d1d391b3dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831807"
---
# <a name="hasquota"></a>HasQuota

**HasQuota**要素は、管理対象のフォルダーがクォータを持つかどうかを示します。 
  
```xml
<HasQuota/>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |管理フォルダーに関する情報が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、ブール値を表します。 **True**の場合は、フォルダーが、クォータを持っていることを示します**false**の値は、フォルダーがクォータを持っていないことを示します。 
  
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

