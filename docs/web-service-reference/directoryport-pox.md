---
title: DirectoryPort (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ab436b54-ceba-4cd9-aeb4-134f9b93986d
description: DirectoryPort 要素は、ネームサービスプロバイダインターフェイス (NSPI) プロトコルが使用されている場合に、ディレクトリへの接続に使用されるポートを指定します。
ms.openlocfilehash: 2ba0a15cea0b4eb9b6069fab384edb3d9747a360
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462088"
---
# <a name="directoryport-pox"></a>DirectoryPort (POX)

**Directoryport**要素は、ネームサービスプロバイダインターフェイス (NSPI) プロトコルが使用されている場合に、ディレクトリへの接続に使用されるポートを指定します。 
  
- [自動検出 (POX)](autodiscover-pox.md) 
- [応答 (POX)](response-pox.md)  
- [アカウント (POX)](account-pox.md)  
- [プロトコル (POX)](protocol-pox.md)  
- [DirectoryPort (POX)](directoryport-pox.md)
  
```xml
<DirectoryPort/>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

Text 値は、Exchange サーバーへのアクセスに使用されるポートを表します。
  
## <a name="remarks"></a>注釈

**Directoryport**要素は、 [Type (POX)](type-pox.md)要素が EXCH または EXPR と等しい場合にのみ使用されます。 
  
## <a name="see-also"></a>関連項目

- [Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

