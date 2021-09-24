---
title: Exchange 2013 トランスポート パイプライン内のメッセージの読み取りおよび変更
manager: sethgros
ms.date: 09/17/2021
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b53ed47a-3d01-4c4e-ad32-fb0532872aad
description: Exchange 2013 のカスタム トランスポート エージェントでメッセージを読み取り、書き込み、および変更するために使用できる .NET Framework クラスの詳細について説明します。
ms.openlocfilehash: 5bf4406f7ca82512bb55388e0865e0d343cae66e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537237"
---
# <a name="reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline"></a>Exchange 2013 トランスポート パイプライン内のメッセージの読み取りおよび変更

Exchange 2013 のカスタム トランスポート エージェントでメッセージを読み取り、書き込み、および変更するために使用できる .NET Framework クラスの詳細について説明します。
  
**製品:** Exchange Server 2013
  
- メッセージの読み取り、書き込み、または変更に使用するクラス
- Encoders 名前空間
- iCalendar 名前空間
- MIME 名前空間
- TextConverters 名前空間
- Tnef 名前空間
- vCard 名前空間
  
メッセージがトランスポート パイプラインを通過するときに、トランスポート エージェントはメッセージの内容を読み取ったり、書き込んだり、別のデータ形式に変換したりできます。たとえば、MIME データを読み取ったり書き込んだりできます。また、uuencode 形式や Quoted-printable (qp) 形式の着信メッセージを識別して、そのメッセージを組織で使用している標準に変換することも、着信メッセージに関連付けられている予定表または連絡先情報を読み取って保存することもできます。  
  
さらに、セキュリティ上の問題を引き起こすコンテンツを識別し、それらを含むコンテンツやメッセージを移動または削除する (たとえば、HTML メッセージのリンクを削除するなど) こともできます。
  
この記事では、メッセージの読み取り、書き込み、および変更に使用できる .NET Framework のクラスに関する情報を提供します。
  
> [!CAUTION]
> コンテンツ変換 API の多くのプロパティとパラメーターには、パフォーマンスの問題 (サービス拒否攻撃を含む) を引き起こすほど大きな値が使用できます。トランスポート エージェントでコンテンツ変換 API を使用する場合は、エージェントのリソース消費量に制限をかけるため、読み取り時や書き込み時にプロパティ値とパラメーター値でサポートするサイズに制限を実装する必要があります。 

<a name="Namespaces"> </a>

## <a name="classes-used-to-read-write-or-modify-messages"></a>メッセージの読み取り、書き込み、または変更に使用するクラス

次の表に、電子メール メッセージの読み取り、書き込み、および変更に使用できる .NET Framework のクラスを示します。
  
**.NET Framework のメッセージ処理の名前空間**

|**.NET Framework 名前空間**|**Classes**|
|:-----|:-----|
|[Microsoft。Exchange。Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |メモリ内エンコードとデコードのクラス、関連する列挙に含まれるエンコーダーまたはデコーダー クラスのいずれかを受け入れるエンコーダー ストリーム クラス、エンコーダーとデコーダーの ByteEncoder 基本クラスと[ByteEncoderException](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoderException.aspx)例外クラスが含まれます。 [](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoder.aspx)  <br/> |
|[Microsoft。Exchange。Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |予定表の情報が含まれているデータ ストリームの読み書きを可能にする型が含まれています。これには、予定表のリーダーとライター、例外オブジェクト、定期的なアイテム オブジェクト、および予定表アイテムに関するプロパティ情報を返す際に役立つ構造体と列挙体が含まれます。  <br/> |
|[Microsoft。Exchange。Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |MIME データの作成、読み取り、書き込み、走査、エンコード、およびデコードに使用できるクラス、構造体、列挙体およびデリゲートが含まれています。これには、MIME データ ストリームへの順方向専用の読み取り書き込みアクセスが可能になるストリーム ベースのリーダーとライターと、MIME ドキュメントに使用可能な DOM ベースのメソッドとクラスが含まれています。  <br/> |
|[Microsoft。Exchange。Data.TextConverters](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |データ ストリームの読み書きと、特定のデータ形式間での変換 (HTML からリッチ テキスト形式 (RTF) への変換など) の実行を可能にするクラス、構造体、列挙体、およびデリゲートが含まれています。テキスト コンバーターを使用すると、ドキュメント ストリームの形式を相互に変換できるようになり、セキュリティ上のリスクを招く可能性のあるドキュメントの要素を選択的に削除することもできるようになります。   <br/> |
|[Microsoft。Exchange。Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |Transport Neutral Encapsulation Format (TNEF) の読み取りと書き込みが容易になる順方向専用のストリーム リーダーとライター、例外クラス、および構造体と列挙体が含まれています。  <br/> |
|[Microsoft。Exchange。Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |vCard 形式の連絡先データの読み取りと書き込みが容易になる順方向専用のストリーム リーダーとライター、例外クラス、および構造体と列挙体が含まれています。  <br/> |
   
## <a name="encoders-namespace"></a>Encoders 名前空間
<a name="Encoders"> </a>

Encoders 名前空間には、メモリ内エンコードおよびデコードに対応するクラスが含まれています。 これらは [ByteEncoder 基本クラスから](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoder.aspx) 継承します。 各クラスでは、Base64、BinHex、Quoted-printable (qp)、および Unix-to-Unix (Uu) のエンコードとデコードを行います。 メモリ内エンコードおよびデコードに使用されるクラスを次に示します。 
  
- [Base64Encoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.Base64Encoder.aspx)
    
- [Base64Decoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.Base64Decoder.aspx)
    
- [BinHexEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.BinHexEncoder.aspx)
    
- [BinHexDecoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.BinHexDecoder.aspx)
    
- [QPEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.QPEncoder.aspx)
    
- [QPDecoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.QPDecoder.aspx)
    
- [UUEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.UUEncoder.aspx)
    
- [UUDecoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.UUDecoder.aspx)
    
エンコーダーとデコーダーは [、ByteEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoder.aspx) 基本クラスから継承し、エラー処理に [ByteEncoderException](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoderException.aspx) 例外クラスを使用します。 
  
さらに、名前空間には [MacBinaryHeader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.MacBinaryHeader.aspx) クラスが含まれています。このクラスは MacBinary エンコード されたファイルを識別し、関連付けられたファイル ヘッダーを読み取ります。 
  
最後に [、EncoderStream](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.EncoderStream.aspx) クラスは、メモリ内オブジェクトの代わりにデータ ストリームに対して変換を実行します。 このクラスは、エンコーダーまたはデコーダー クラスのいずれかを受け入れ、関連付けられた EncoderStreamAccess 列挙に従って読み取りまたは書 [き込みを行](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.EncoderStreamAccess.aspx) います。 
  
## <a name="icalendar-namespace"></a>iCalendar 名前空間
<a name="iCalendar"> </a>

iCalendar 名前空間には、iCalendar データに対応した順方向専用のリーダーおよびライターと、iCalendar ストリームの作成、アクセス、および変更をサポートする構造体とクラスが用意されています。
  
[CalendarReader クラスと](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.aspx) [CalendarWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarWriter.aspx)クラスは、iCalendar ストリーム データの読み取りおよび書き込みに使用されます。 
  
CalendarReader は、読み取り [可能な Stream](https://msdn.microsoft.com/library/System.IO.Stream.aspx) をコンストラクターの引数として受け取ります。 次に [、ReadFirstChildComponent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ReadFirstChildComponent.aspx)メソッド [、ReadNextSiblingComponent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ReadNextSiblingComponent.aspx)メソッド、 [および ReadNextComponent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ReadNextComponent.aspx) メソッドを使用して、データ ストリーム内の iCalendar コンポーネントに順次アクセスできます。 [ComplianceMode](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ComplianceMode.aspx)プロパティに設定した値に基づいて、iCalendar ストリームのエラーによって例外がスローされるか[、ComplianceStatus](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ComplianceStatus.aspx)プロパティが Compliance 以外の値に設定されます。 [](https://msdn.microsoft.com/library/microsoft.exchange.data.contenttypes.icalendar.calendarcompliancestatus.aspx) このプロパティを確認することで、受信 iCalendar データの問題を検出できます。 
  
[CalendarWriter クラス](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarWriter.aspx)は、書き込み[可能な Stream](https://msdn.microsoft.com/library/System.IO.Stream.aspx)をコンストラクターの引数として受け取ります。 
  
## <a name="mime-namespace"></a>MIME 名前空間
<a name="MIME"> </a>

MIME 名前空間には、MIME ドキュメントの作成、アクセス、および変更を可能にするクラスが用意されています。ストリーム ベースのメソッドまたは DOM ベースのメソッドのどちらかを使用して、MIME ドキュメントを操作できます。
  
### <a name="mimedocument-class-and-the-mime-dom"></a>MimeDocument クラスと MIME DOM

[MimeDocument クラスを使用](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.aspx)すると、MIME ドキュメントへの DOM アクセスが有効です。 この型のオブジェクトは、DOM 全体をロードできるメモリ容量があり、メッセージのヘッダーとコンテンツへのランダム アクセスが必要なときに使用します。 
  
GetLoadStream メソッドまたは Load メソッドを [使用して、MimeDocument](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.aspx) オブジェクト [に](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.GetLoadStream.aspx) データ [を](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.Load.aspx) 読み込む。 その後、DOM 階層を辿って MIME データを作成、変更、または削除します。 MIME データを変更した後は、WriteTo メソッドのいずれかを使用してストリームに [書き](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeNode.WriteTo.aspx) 込みます。 
  
次の図は [、MimeDocument](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.aspx) オブジェクト内のデータの構造を示しています。 
  
**図 1.MimeDocument オブジェクトの構造**

![MIME DOM のアーキテクチャ](media/MimeDomArchitecture.gif)
  
### <a name="mimereader-and-mimewriter-classes-and-stream-based-mime-parsing"></a>MimeReader クラスおよび MimeWriter クラスとストリーム ベースの MIME 解析

[MimeReader クラスと](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.aspx) [MimeWriter クラスを使用すると](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeWriter.aspx)、MIME ストリームへの転送専用アクセスが有効になります。 これらのクラスは、MIME データを変更する必要がなく、読み取りまたは書き込みが完了しているデータが必要になる場合に使用します。 たとえば、定義済みの形式に合ったメッセージを印刷する場合は [、MimeWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeWriter.aspx) クラスが最適な場合があります。 
  
[MimeDocument クラスは](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.aspx)DOM をカプセル化します。 [MimeReader クラスと](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.aspx) [MimeWriter クラスは](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeWriter.aspx)、状態コンピューターを表します。 それらの状態は、受信した入力と呼び出したメソッドによって変化します。 図 2 ~ 5 は [、MimeReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.aspx) オブジェクトに対して、各状態から呼び出すのに有効なメソッドと結果の状態を示す簡略化された状態遷移図です。 
  
これらの図を使用する場合は、ある状態から次の状態への矢印に従い、状態の変化を起こすメソッドの呼び出しや戻り値に注目します。 たとえば、最初の図では、自作の MimeReader に属するストリームの開始点を想定しています。 パーツ ヘッダーの状態を取得するには、その順序で [ReadNextPart](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.ReadNextPart.aspx) または [ReadFirstChildPart](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.ReadFirstChildPart.aspx)のいずれかを呼び出します。 ヘッダーが存在する場合 (MIME が整形式の場合) は、Part Headers 状態に移行します。 それ以外の場合は、例外がスローされます。 
  
**図 2.MimeReader オブジェクトの簡略化された状態遷移図**

![MimeReader 状態図](media/MimeReader_StateDiagram_01.gif)
  
> [!NOTE]
> 図 3、4 および 5 では、それぞれ前の図に示した状態を詳しく説明しています。 
  
**図 3.図 2 からのパーツ ヘッダーの状態の拡張**

!["Part Headers" 状態の拡張](media/MimeReader_StateDiagram_02.gif)
  
**図 4.ヘッダーでパラメーターが検出された場合の図 3 からのヘッダー状態の拡張**

![ヘッダーでパラメーターが検出された場合の 'パーツ ヘッダー' 状態の拡張](media/MimeReader_StateDiagram_03.gif)
  
> [!NOTE]
> 図 5 で表される状態は、アドレス グループが検出された場合 [、GroupRecipientReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeAddressReader.GroupRecipientReader.aspx) プロパティを使用してグループ内のアドレスを読み取るという点で再帰的です。 
  
**図 5.アドレスまたはアドレス グループが検出された場合の図 3 からのヘッダー状態の拡張**

![住所またはグループに対する "Header" 状態の拡張](media/MimeReader_StateDiagram_04.gif)
  
図 6 と図 7 は、MimeWriter オブジェクトの簡略化された状態遷移 [図を示](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeWriter.aspx) しています。 
  
> [!NOTE]
> 図 7 では、図 6 に示した Part Headers 状態を詳しく説明しています。 
  
**図 6.MimeWriter オブジェクトの簡略化された状態遷移図**

![MimeWriter 用の状態遷移図](media/MimeWriter_TopLevel.gif)
  
**図 7.図 6 からのパーツ ヘッダーの状態の拡張**

![MimeWriter 用の状態遷移図拡張機能](media/MimeWriter_Diagram_Expansion.gif)
  
## <a name="textconverters-namespace"></a>TextConverters 名前空間
<a name="TextConverters"> </a>

TextConverters 名前空間には、電子メール メッセージの内容の変換をサポートする型が含まれます。 これらの種類では、コード ページ変換を実行し、セキュリティで保護されていない HTML を削除し、電子メール メッセージのボディで他の変換を実行できます。 [Microsoft.Exchange。Data.TextConverters](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx)名前空間には[、TextConverter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextConverter.aspx)抽象クラスから派生する次のクラスが含まれます。 
  
- [EnrichedToHtml](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.EnrichedToHtml.aspx)
    
- [EnrichedToText](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.EnrichedToText.aspx)
    
- [HtmlToEnriched](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlToEnriched.aspx)
    
- [HtmlToHtml](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlToHtml.aspx)
    
- [HtmlToRtf](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlToRtf.aspx)
    
- [HtmlToText](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlToText.aspx)
    
- [RtfCompressedToRtf](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfCompressedToRtf.aspx)
    
- [RtfToHtml](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfToHtml.aspx)
    
- [RtfToRtf](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfToRtf.aspx)
    
- [RtfToRtfCompressed](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfToRtfCompressed.aspx)
    
- [RtfToText](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfToText.aspx)
    
- [TextToHtml](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextToHtml.aspx)
    
- [TextToRtf](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextToRtf.aspx)
    
- [TextToText](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextToText.aspx)
    
これらのテキスト コンバーターを使用すると、ドキュメント ストリームの形式を変更したり、HTML ドキュメントから安全でない要素を削除したりできます。 これらのクラスは、単一の呼び出しを [使用して、TextConverter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextConverter.aspx) 基本クラスの Convert メソッドの 1 つを使用して変換を実行するために単独で使用するか、変換された読み取りまたは書き込みを実行するコンバーターのコンストラクターに渡すことができます。 
  
基底クラスから継承した機能は、元のドキュメントと変換後の出力を保存するための十分な領域がある場合や、変換の結果を保存する必要がある場合の変換を実行する際に役立ちます。**Convert** メソッドは、入力と出力のストリーム、テキスト リーダー、またはテキスト ライターを受け取り、入力のコンテンツを関連付けられた出力に変換します。 
  
この名前空間には、次に示すテキスト リーダー、ライター、およびストリームのクラスも含まれています。
  
- [ConverterReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.ConverterReader.aspx) — **System.IO.TextReader から派生します**。 
    
- [ConverterWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.ConverterWriter.aspx) — **System.IO.TextWriter から派生します**。 
    
- [ConverterStream](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.ConverterStream.aspx) — **System.IO.Stream から派生します**。 
    
これらは、元のデータや変換後の出力を保存する領域がない場合、ストリームからの入力を受信する場合やストリームに出力を送信する場合、または出力の用途がインデックスの作成や検索のみで変換の結果を保存する必要のない場合の変換を実行するために使用します。
  
## <a name="tnef-namespace"></a>Tnef 名前空間
<a name="TNEF"> </a>

Tnef 名前空間には、TNEF データについて順方向専用のストリーム ベースの読み取りおよび書き込みを可能にするクラスと型が含まれています。TNEF とは、MAPI を解釈できないクライアントのために、MAPI のプロパティをカプセル化することを目的として使用されるデータ形式のことです。
  
[TnefReader クラスと](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.aspx) [TnefWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefWriter.aspx)クラスは[、Microsoft.Exchange のコア機能を提供します。Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx)名前空間。 
  
[TnefReader クラスは](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.aspx)、コンストラクターの引数として読み取り可能なストリームを受け取ります。 次に [、ReadNextAttribute](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.ReadNextAttribute.aspx) メソッドを使用して、TNEF ストリーム内の属性を順番に読み取ります。 属性を読み取った後は[、TnefPropertyReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefPropertyReader.aspx)を取得して現在のプロパティを読み取るだけでなく[、TnefReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.aspx)オブジェクトの読み取り専用プロパティを使用して属性に関する情報にアクセスできます。 [ReadAttributeRawValue](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.ReadAttributeRawValue.aspx)メソッドを使用して、現在の属性に直接アクセスすることもできます。 
  
[TnefWriter クラス](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefWriter.aspx)は、書き込み[可能な Stream](https://msdn.microsoft.com/library/System.IO.Stream.aspx)をコンストラクターの引数として受け取ります。 [TnefWriter クラスは](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefWriter.aspx)、このストリームにデータを書き込む複数の方法を提供します。 
  
## <a name="vcard-namespace"></a>vCard 名前空間
<a name="vCard"> </a>

vCard 名前空間には、vCard データ形式で電子メール メッセージに含まれている連絡先情報を読み書きするために使用するクラス、構造体、および列挙体が含まれています。この名前空間には、電子メール メッセージに関連付けられた vCard データの読み取りを可能にする連絡先リーダーとライター、例外クラス、プロパティ リーダー、パラメーター リーダー、およびサポート用列挙体が含まれています。
  
## <a name="see-also"></a>関連項目

- [Exchange のトランスポート エージェント](transport-agents-in-exchange-2013.md)  
- [Exchange 2013 におけるトランスポート エージェントの概念](transport-agent-concepts-in-exchange-2013.md) 
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)
- [MIME メディアの種類](http://www.iana.org/assignments/media-types)
    

