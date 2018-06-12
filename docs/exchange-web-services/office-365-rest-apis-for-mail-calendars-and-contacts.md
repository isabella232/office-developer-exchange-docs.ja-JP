---
title: メール、予定表、および連絡先の Office 365 REST API
manager: sethgros
ms.date: 4/29/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3b2e71a6-5fa5-4008-b243-d3a6e9173b3d
description: メール、予定表、および連絡先にアクセスするのに使用できる Office 365 API に関する情報を Office 365 または Exchange Online で探します。
ms.openlocfilehash: d42d3ff0b68dfbf23d5a4eebb826a6d39a4ac116
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759175"
---
# <a name="office-365-rest-apis-for-mail-calendars-and-contacts"></a>メール、予定表、および連絡先の Office 365 REST API

メール、予定表、および連絡先にアクセスするのに使用できる Office 365 API に関する情報を Office 365 または Exchange Online で探します。
  
Office 365 および Exchange Online は、電子メール、予定表、および連絡先で作業する新しい方法を提供します。メール、予定表、および連絡先の REST API は、Exchange データへのアクセスと操作に関する強力で簡単な方法を提供します。これらの API は、オープン標準に基づいています:認証には OAuth バージョン 2.0、データ抽象化には OData バージョン 4.0 および JSON が該当します。これには以下の利点があります。
  
- これらの API は認証に OAuth を求めるため、アプリケーションがユーザーの資格情報を処理または格納する必要はありません。
    
- OAuth は、ユーザー データへの厳格に範囲指定されたアクセス許可を要求できるようにします。たとえば、アクセス許可を要求して、ユーザーの予定表のみを読み取るようにアプリケーションを設計する場合があります。
    
## <a name="work-with-email-and-mail-folders"></a>電子メールおよびメール フォルダーで作業する

[メール API](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx) を使用して、電子メールの取得、作成、更新、削除、移動、コピー、および送信を行うことができます。また、メール フォルダーの取得、作成、更新、および削除を行うこともできます。 
  
## <a name="work-with-events-calendars-and-calendar-groups"></a>イベント、予定表、および予定表グループで作業する

[予定表 API](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx) を使用して、イベントの取得、作成、更新、および削除を行うことができます。また、予定表グループおよび予定表の取得、作成、更新、および削除を行うこともできます。 
  
## <a name="work-with-contacts-and-contact-folders"></a>連絡先および連絡先フォルダーで作業する

[連絡先 API](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx) を使用して、ユーザーのメールボックス内の連絡先の取得、作成、更新、および削除を行うことができます。また、連絡先フォルダーの取得を行うこともできます。 
  
## <a name="work-with-file-providers"></a>ファイル プロバイダーの操作

[ファイル プロバイダーの REST API](http://msdn.microsoft.com/library/8bab5403-de68-4b49-ab19-9a6470f2a2ce%28Office.15%29.aspx) を使用して、メールボックス、Dropbox などのサポートされているファイル プロバイダーに関する情報を取得、作成、更新、削除することができます。 
  
## <a name="next-steps"></a>次の手順

[Office 365 プラットフォームでの開発](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx)ページに進んで、環境のセットアップおよび API を開始するためのガイダンスを含む、メール、予定表、および連絡先 API に関する情報を取得してください。また、[スタート プロジェクトおよびコード サンプル](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx)を必ず確認して、これらの API の動作を参照してください。 
  
## <a name="see-also"></a>関連項目


- [Office 365 プラットフォーム上での開発](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx)
    
- [Office 365 ASP.NET MVC アプリの構築](http://msdn.microsoft.com/office/office365/howto/Build-your-first-ASPNET-MVC-app%28Office.15%29.aspx)
    
- [メール REST 操作](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx)
    
- [予定表 REST 操作](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx)
    
- [連絡先 REST 操作](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx)
    
- [Office 365 API スタート プロジェクトおよびサンプル コード](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx)
    

