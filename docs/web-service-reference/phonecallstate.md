---
title: PhoneCallState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallState
api_type:
- schema
ms.assetid: ac009eb3-6334-49ce-82be-48fe83577f9c
description: PhoneCallState 要素は、電話の呼び出しの現在の状態を指定します。
ms.openlocfilehash: 184a7400810711442e565d1ef37094bd63b00914
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832761"
---
# <a name="phonecallstate"></a>PhoneCallState

**PhoneCallState**要素は、電話の呼び出しの現在の状態を指定します。 
  
```xml
<PhoneCallState>Idle or Connecting or Alerted or Connected or Disconnected or Incoming or Transferring or Forwarding</PhoneCallState>
```

 **PhoneCallStateType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[PhoneCallInformation](phonecallinformation.md) <br/> |電話の状態情報を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表は、 **PhoneCallState**要素の値を一覧します。 
  
**PhoneCallState 要素の値**

|**値**|**説明**|
|:-----|:-----|
|アイドル  <br/> |最初の呼び出しの状態です。  <br/> |
|Connecting  <br/> |システムがこの呼び出しをダイヤルします。  <br/> |
|警告を表示  <br/> |状態の警告では、呼び出し (電話が鳴って)。  <br/> |
|Connected  <br/> |呼び出しは、接続されている状態です。  <br/> |
|Disconnected  <br/> |呼び出しは切断されます。  <br/> |
|受信  <br/> |呼び出しのバインドが解除されます。  <br/> |
|転送します。  <br/> |呼び出しが別の宛先に転送されます。  <br/> |
|転送  <br/> |呼び出しを別の宛先に転送されているが。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの/ews/ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

