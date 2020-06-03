---
title: メール、カレンダー、連絡先用の Microsoft Graph の Outlook API
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
ms.assetid: 3b2e71a6-5fa5-4008-b243-d3a6e9173b3d
description: Office 365 または Exchange Online において、メール、予定表、連絡先へのアクセスに使用できる Microsoft Graph API の詳細です。
localization_priority: Priority
ms.openlocfilehash: 7ca77596afb59ffab76001abd495de7328d2dd29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463868"
---
# <a name="microsoft-graph-rest-apis-for-mail-calendars-and-contacts"></a>メール、予定表、連絡先用の Microsoft Graph の REST API

Office 365、Exchange Online、またはハイブリッド展開の Exchange Server のメール、予定表、連絡先へのアクセスに使用できる Microsoft Graph Api についての情報を参照してください。

ハイブリッド展開の Office 365、Exchange Online、および Exchange Server は、電子メール、予定表、連絡先を操作するための新しい方法を提供します。 Microsoft Graph のメール、予定表、連絡先用の REST API は、Exchange データにアクセスして操作する強力で簡単な方法を提供します。 これらの API は、認証用の OAuth バージョン 2.0、データ抽象化用の OData バージョン 4.0 および JSON など、オープンな標準に基づいています。 これには以下の利点があります。

- これらの API は認証に OAuth を求めるため、アプリケーションがユーザーの資格情報を処理または格納する必要はありません。

- OAuth は、ユーザー データへの厳格に範囲指定されたアクセス許可を要求できるようにします。たとえば、アクセス許可を要求して、ユーザーの予定表のみを読み取るようにアプリケーションを設計する場合があります。

## <a name="work-with-email-and-mail-folders"></a>電子メールおよびメール フォルダーで作業する

[メール API](https://developer.microsoft.com/graph/docs/concepts/outlook-mail-concept-overview) を使用して、電子メールの取得、作成、更新、削除、移動、コピー、および送信を行うことができます。また、メール フォルダーの取得、作成、更新、および削除を行うこともできます。 
  
## <a name="work-with-events-calendars-and-calendar-groups"></a>イベント、予定表、および予定表グループで作業する

[予定表 API](https://developer.microsoft.com/graph/docs/concepts/outlook-calendar-concept-overview) を使用して、イベントの取得、作成、更新、および削除を行うことができます。また、予定表グループおよび予定表の取得、作成、更新、および削除を行うこともできます。 
  
## <a name="work-with-contacts-and-contact-folders"></a>連絡先および連絡先フォルダーで作業する

[連絡先 API](https://developer.microsoft.com/graph/docs/concepts/outlook-contacts-concept-overview) を使用して、ユーザーのメールボックス内の連絡先の取得、作成、更新、および削除を行うことができます。また、連絡先フォルダーの取得を行うこともできます。 
  
## <a name="next-steps"></a>次のステップ

[「Microsoft Graph ドキュメント」](https://developer.microsoft.com/graph/docs/concepts/overview)のページにマウス ポインターを合わせて、環境設定および API 使用開始にあたってのガイダンスを含む、メール、予定表、連絡先の API のより詳細な情報を取得します。 

また、[「Microsoft Graph のクイック スタート」](https://developer.microsoft.com/graph/quick-start)と[コード サンプル](https://developer.microsoft.com/office/gallery/?filterBy=Samples,Microsoft%20Graph)を必ず確認し、これらの API の動作をご覧ください。 
  
## <a name="see-also"></a>関連項目

- [Microsoft Graph のドキュメント](https://developer.microsoft.com/graph/docs/concepts/overview)   
- [REST API のオンプレミスの要件](https://blogs.technet.microsoft.com/exchange/2016/09/26/on-premises-architectural-requirements-for-the-rest-api)   

