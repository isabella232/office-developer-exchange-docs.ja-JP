---
title: Exchange での EWS の電子情報開示
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3128419f-dd5f-46d2-bb0d-0940738d0bb6
description: Exchange の EWS の電子情報開示について説明します。
ms.openlocfilehash: 48e3fdb3a2f21f7dcfcb7eed21b586e099b249a3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456095"
---
# <a name="ediscovery-in-ews-in-exchange"></a>Exchange での EWS の電子情報開示

Exchange の EWS の電子情報開示について説明します。
  
電子情報開示は、外部アプリケーションが Exchange データのクエリを実行できるようにするフェデレーション クエリ Web サービスです。
  
証拠開示は、主なデータの識別や保持、データの選別や確認、法廷でのデータの生成を含むいくつかのフェーズから構成されます。電子情報開示のクエリは、Exchange と SharePoint にまたがる単一の証拠開示ワークフローを提供することで、証拠開示プロセスを容易にします。
  
## <a name="ediscovery-operations"></a>電子情報開示の操作

EWS で公開されている電子情報開示機能は、Exchange Online、Office 365 の一部としての Exchange Online、Exchange 2013 以降のバージョンの Exchange で導入された操作によって利用できます。 
  
**表 1. 電子情報開示のための新しい操作**

|**操作名**|**説明**|
|:-----|:-----|
|[GetDiscoverySearchConfiguration](https://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |インプレース ホールド、保存された探索検索、探索検索が有効になっているメールボックスの構成情報を取得します。  <br/> |
|[GetHoldOnMailboxes](https://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |クエリ ベースの保持 ([SetHoldOnMailboxes 操作](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx)を使用して設定される) の状態を取得します。  <br/> |
|[GetNonIndexableItemDetails](https://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |インデックスを作成できないアイテムの詳細を取得します。これには、アイテム識別子、エラー コード、エラーの説明、アイテムのインデックス作成をしようとしたタイミング、ファイルに関する追加情報が含まれますが、これに限定されません。  <br/> |
|[GetNonIndexableItemStatistics](https://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |メールボックス内にある、インデックスを作成できないアイテムの数を取得します。  <br/> |
|[GetSearchableMailboxes](https://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |クライアントが検索または電子情報開示を実行するアクセス許可を持つメールボックスの一覧を取得します。  <br/> |
|[SearchMailboxes](https://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |特定のメールボックス内にある、クエリ キーワードに一致するアイテムを検索します。  <br/> |
|[SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |アイテムにクエリベースの保持を設定します。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)
    
- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)
    

