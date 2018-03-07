---
layout: default
title: markdown Tests
---

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="2">area</td>
  </tr>
  <tr>
    <th>テーブルの説明</th><td align="center" colspan="2">地域を区別する情報を管理するテーブル</td>
  </tr>
  <tr>
    <th>カラム名</th><td align="center">area_id</td><td align="center">area_name</td>
  </tr>  
  <tr>
    <th>型名</th><td align="center">serial</td><td align="center">text</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">not null</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">PK</td><td align="center">---</td>
  </tr>  
  <tr>
    <th>カラムの説明</th><td align="center">地域のid</td><td align="center">地域名</td>
  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="2">area_company</td>
  </tr>
  <tr>
    <th>テーブルの説明</th><td align="center" colspan="2">地域内で表示対象のバス会社を管理するテーブル</td>
  </tr>
  <tr>
    <th>カラム名</th><td align="center">area_id</td><td align="center">bus_company_id</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">integer</td><td align="center">integer</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">---</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">PK</td><td align="center">---</td>
  </tr>
  <tr>
    <th>カラムの説明</th><td align="center">地域のid</td><td align="center">バス会社のid</td>
  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="2">bus_company</th>
  </tr>
  <tr>
    <th>テーブルの説明</th><td align="center" colspan="2">バス会社を管理するテーブル</td>
  </tr>
  <tr>
    <th>カラム名</th><td align="center">bus_company_id</td><td align="center">company_name</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">serial</td><td align="center">text</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">---</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">PK</td><td align="center">---</td>
  </tr>
  <tr>
    <th>カラムの説明</th><td align="center">バス会社のid</td><td align="center">会社名</td>
  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="3">bus_course</td>
  </tr>
  <tr>
    <th>テーブルの説明</th><td align="center" colspan="3">路線情報を地図上に線でプロットするための情報を管理するテーブル</td>
  </tr>
  <tr>
    <th>カラム名</th><td align="center">route_id</td><td align="center">ordinal</td><td align="center">latlon</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">integer</td><td align="center">integer</td><td align="center">circle</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">not null</td><td align="center">---</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">複合PK</td><td align="center">複合PK</td><td align="center">---</td>
  </tr>
  <tr>
    <th>カラムの説明</th><td align="center">路線のid</td><td align="center">番号</td><td align="center">緯度・経度</td>
  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="4">bus_stop</td>
  </tr>
  <tr>
    <th>テーブルの説明</th><td align="center" colspan="4">バス停の位置情報を管理するテーブル</td>
  </tr>
  <tr>
    <th>カラム名</th><td align="center">bus_stop_id</td><td align="center">bus_company_id</td><td align="center">bus_stop_name</td><td align="center">latlon</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">serial</td><td align="center">integer</td><td align="center">text</td>
    <td align="center">circle</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">---</td><td align="center">---</td>
    <td align="center">---</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">PK</td><td align="center">FK</td><td align="center">---</td>
    <td align="center">---</td>
  </tr>
  <tr>
    <th>カラムの説明</th><td align="center">バス停のid</td><td align="center">バス会社のid</td><td align="center">バス停の名前
    </th><td align="center">緯度・経度</td>
  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="3">day_type</td>
  </tr>
  <tr>
    <th>テーブルの説明</th><td align="center" colspan="3">ある交番が平日運行か土日祝運行かを管理するテーブル</td>
  </tr>
  <tr>
    <th>カラム名</th><td align="center">day_type_id</td><td align="center">koban_id</td><td align="center">day_type</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">serial</td><td align="center">integer</td><td align="center">text</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">---</td><td align="center">not null</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">PK</td><td align="center">FK</td><td align="center">---</td>
  </tr>
  <tr>
    <th>カラムの説明</th><td align="center">サロゲートキー</td><td align="center">交番のid</td><td align="center">平日・土日祝日</td>
  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="3">device</td>
  </tr>
  <tr>
    <th>テーブルの説明</th><td align="center" colspan="3">端末情報を管理するテーブル</td>
  </tr>
  <tr>
    <th>カラム名</th><td align="center">device_id</td><td align="center">bus_company_id</td><td align="center">code</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">serial</td><td align="center">integer</td><td align="center">text</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">not null</td><td align="center">not null</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">PK</td><td align="center">FK</td><td align="center">---</td>
  </tr>
  <tr>
    <th>カラムの説明</th><td align="center">端末のid</td><td align="center">バス会社のid</td><td align="center">端末を識別するためのコード</td>
  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="5">gps_data</td>
  </tr>
  <tr>
    <th>テーブルの説明</th><td align="center" colspan="5">取得したGPS情報を管理するテーブル</td>
  </tr>
   <tr>
    <th>カラム名</th><td align="center">gps_data_id</td><td align="center">device_id</td><td align="center">task_id</td>
    <td align="center">submit_at</td><td align="center">latlon</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">serial</td><td align="center">integer</td><td align="center">integer</td>
    <td align="center">timestamp without timezone</td><td align="center">circle</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">---</td><td align="center">---</td>
    <td align="center">---</td>
    <td align="center">---</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">PK</td><td align="center">FK</td><td align="center">FK</td><td align="center">---</td>
    <td align="center">---</td>
  </tr>
  <tr>
    <th>カラムの説明</th><td align="center">GPS情報のid</td><td align="center">端末のid</td><td align="center">タスクのid</td><td align="center">gpsを取得した時間</th><td align="center">緯度・経度</td>
  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="3">koban</td>
  </tr>
  <tr>
    <th>テーブルの説明</th><td align="center" colspan="3">バス会社がもつ交番を管理するテーブル</td>
  </tr>
  <tr>
    <th>カラム名</th><td align="center">koban_id</td><td align="center">bus_company_id</td>
    <td align="center">koban_name</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">serial</td><td align="center">integer</td><td align="center">text</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">---</td><td align="center">---</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">PK</td><td align="center">FK</td><td align="center">---</td>
  </tr>
  <tr>
    <th>カラムの説明</th><td align="center">交番のid</td><td align="center">バス会社のid</td>
　　　　　　　　<td align="center">交番名</td>
　  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="3">platform</td>
  </tr>
  <tr>
    <th>テーブルの説明</th><td align="center" colspan="3">バス停と乗り場を結びつけるテーブル</td>
  </tr>
  <tr>
    <th>カラム名</th><td align="center">platform_id</td><td align="center">platform_name</td>
    <td align="center">latlon</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">serial</td><td align="center">integer</td><td align="center">circle</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">PK</td><td align="center">---</td><td align="center">---</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">PK</td><td align="center">---</td><td align="center">---</td>
  </tr>
  <tr>
    <th>カラムの説明</th><td align="center">乗降場のid</td><td align="center">乗降場の名前</td>
　　　　　　　　<td align="center">経度・緯度</td>
　  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="5">route</td>
  </tr>
  <tr>
    <th>テーブルの説明</th><td align="center" colspan="5">バス会社が運行する路線を管理するテーブル</td>
  </tr>
  <tr>
    <th>カラム名</th><td align="center">route_id</td><td align="center">bus_company_id</td>
    <td align="center">route_name</td>
    <td align="center">by_way_of</td><td align="center">keito_number</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">serial</td><td align="center">integer</td><td align="center">text</td>
    <td align="center">text</td><td align="center">text</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">---</td><td align="center">---</td>
    <td align="center">---</td><td align="center">---</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">PK</td><td align="center">FK</td><td align="center">---</td>
    <td align="center">---</td><td></td>
  </tr>
  <tr>
    <th>カラムの<br>説明</th><td align="center">路線のid</td><td align="center">バス会社のid</td>
　　　　　　　　<td align="center">路線名</td>
　　<td align="center">行き先</td><td align="center">系統番号</td>
  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="3">route_bus_stop</td>
  </tr>
  <tr>
    <th>テーブルの説明</th><td align="center" colspan="3">路線とバス停を紐付けるテーブル</td>
  </tr>
  <tr>
    <th>カラム名</th><td align="center">route_id</td><td align="center">bus_stop_id<td align="center">ordinal</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">integer</td><td align="center">integer</td><td align="center">intger</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">not null</td><td align="center">not null</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">複合PK</td><td align="center">複合PK</td><td align="center">複合PK</td>
  </tr>
  <tr>
    <th>カラムの説明</th><td align="center">路線のid</td><td align="center">バス停のid</td><td align="center">バス会社のid</td>
  </tr>
</table>

<table>
 <tr>
   <th>テーブル名</th><td align="center" colspan="3">route_bus_stop_platform</td>
 </tr>
　　<tr>
  <th>テーブルの説明</th><td align="center" colspan="3">路線ごとのバス停と乗り場を結びつけるテーブル</td>
 </tr>
 <tr>
  <th>カラム名</th><td align="center">route_id</td><td align="center">bus_stop_id</td><td align="center">platform_id</td>
 </tr>
  <tr>
    <th>型名</th><td align="center">integer</td><td align="center">integer</td><td align="center">integer</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">not null</td><td align="center">not null</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">複合PK</td><td align="center">複合PK</td><td align="center">複合PK</td>
  </tr>
  <tr>
  <th>カラムの説明</th><td align="center">路線のid</td><td align="center">バス停のid</td><td align="center">乗り場のid</td>
 </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="4">signage</td>
  </tr>
   <tr>
    <th>テーブルの説明</th><td align="center" colspan="4">サイネージの設置場所と表示タイプを管理するテーブル</td>
  </tr>
 <tr>
    <th>カラム名</th><td align="center">signage_id</td><td align="center">spot</td>
    <td align="center">display_type</td><td align="center">delay_checking_minute</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">serial</td><td align="center">text</td><td align="center">text</td><td align="center">integer</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">---</td><td align="center">---</td><td align="center">---</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">PK</td><td align="center">---</td><td align="center">---</td><td align="center">---</td>
  </tr>
  <tr>
    <th>カラムの説明</th><td align="center">サイネージのid</td><td align="center">設置場所</td>
    <td>表示形式</td><td align="center">遅れ余裕時間</td>
  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="3">signage_item</td>
  </tr>
   <tr>
    <th>テーブルの説明</th><td align="center" colspan="3">サイネージ設置場所とバス停を結びつけるテーブル</td>
  </tr>
 <tr>
    <th>カラム名</th><td align="center">signage_item_id</td><td align="center">signage_id</td><td align="center">bus_stop_id</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">serial</td><td align="center">integer</td><td align="center">integer</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">---</td><td align="center">---</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">PK</td><td align="center">FK</td><td align="center">FK</td>
  </tr>
 <tr>
    <th>カラムの説明</th><td align="center">サロゲートキー</td><td align="center">サイネージのid</td><td align="center">バス停のid</td>
  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="5">signage_tmp</td>
  </tr>
   <tr>
    <th>テーブルの説明</th><td align="center" colspan="5">交番で管理していないがサイネージに表示したい運行情報を管理するテーブル</td>
  </tr>
 <tr>
    <th>カラム名</th><td align="center">signage_tmp_id</td><td align="center">route_id</td><td align="center">bus_stop_id</td>
    <td align="center">departure_time</td>
    <td align="center">day_type</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">serial</td><td align="center">integer</td><td align="center">integer</td><td align="center">time without time zone</td><td align="center">text</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">---</td><td align="center">---</td><td align="center">---</td><td align="center">---</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">PK</td><td align="center">FK</td><td align="center">FK</td><td align="center">---</td><td align="center">---</td>
  </tr>
 <tr>
    <th >カラムの説明</th><td align="center">サロゲートキー</td><td align="center">路線のid</td><td align="center">バス停のid</td>
    <td align="center">出発時間</td><td align="center">平日か休日</td>
  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="4">special_term</td>
  </tr>
   <tr>
    <th>テーブルの説明</th><td align="center" colspan="4">特別運行期間を管理するテーブル</td>
  </tr>
 <tr>
    <th>カラム名</th><td align="center">special_term_id</td><td align="center">bus_company_id</td><td align="center">begin_at</td>
    <td align="center">end_at</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">serial</td><td align="center">integer</td><td align="center">integer</td><td align="center">time without time zone</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">not null</td><td align="center">---</td><td align="center">---</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">PK</td><td align="center">FK</td><td align="center">---</td><td align="center">---</td>
  </tr>
 <tr>
    <th>カラムの説明</th><td align="center">特別運行id</td><td align="center">バス会社id</td><td align="center">開始時間</td>
    <td align="center">終了時間</td>
  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="2">special_term_operation</td>
  </tr>
   <tr>
    <th>テーブルの説明</th><td align="center" colspan="2">特別運行期間の交番運行を管理するテーブル</td>
  </tr>
 <tr>
    <th>カラム名</th><td align="center">special_term_id</td><td align="center">koban_id</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">integer</td><td align="center">integer</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">not null</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">複合PK</td><td align="center">複合PK</td>
  </tr>
 <tr>
    <th>カラムの説明</th><td align="center">特別運行id</td><td align="center">交番id</td>
  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="2">special_term_tmp</td>
  </tr>
   <tr>
    <th>テーブルの説明</th><td align="center" colspan="2">交番で管理していないが特別運行期間中にサイネージに表示したい運行情報を管理するテーブル</td>
  </tr>
 <tr>
    <th>カラム名</th><td align="center">special_term_id</td><td align="center">signage_tmp_id</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">integer</td><td align="center">integer</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">not null</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">複合PK</td><td align="center">複合PK</td>
  </tr>
 <tr>
    <th>カラムの説明</th><td align="center">特別運行id</td><td align="center">外部キー</td>
  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="3">task</td>
  </tr>
   <tr>
    <th>テーブルの説明</th><td align="center" colspan="3">交番内の各運行路線を一つのタスクとして管理するテーブル</td>
  </tr>
 <tr>
    <th>カラム名</th><td align="center">task_id</td><td align="center">koban_id</td><td align="center">route_id</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">serial</td><td align="center">integer</td><td align="center">integer</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">---</td><td align="center">---</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">PK</td><td align="center">FK</td><td align="center">FK</td>
  </tr>
 <tr>
    <th>カラムの説明</th><td align="center">タスクのid</td><td align="center">交番のid</td><td align="center">路線のid</td>
  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="8">task_delay</td>
  </tr>
   <tr>
    <th>テーブルの説明</th><td align="center" colspan="8">バス停基準でタスクごとの遅れ情報を記録するテーブル</td>
  </tr>
 <tr>
    <th width="100px">カラム名</th><td align="center">task_id</td><td align="center">bus_stop_id</td><td align="center">device_id</td>
    <td align="center">submit_in</td><td align="center">departure_time</td><td align="center">collide_at</td>
    <td align="center">distance</td><td align="center">gps_data_id</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">integer</td><td align="center">integer</td><td align="center">integer</td><td align="center">date</td><td align="center">time without time zone</td><td align="center">time without time zone</td><td align="center">double precision</td><td align="center">bigint</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">not null</td><td align="center">not null</td><td align="center">not null</td><td align="center">not null</td><td align="center">not null</td><td align="center">not null</td><td align="center">not null</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">複合PK</td><td align="center">複合PK</td><td align="center">複合PK</td><td align="center">複合PK</td><td align="center">複合PK</td><td align="center">FK</td><td align="center">---</td><td align="center">---</td>
  </tr>
 <tr>
    <th>カラムの説明</th><td align="center">タスクのid</td><td align="center">バス停のid</td><td align="center">端末のid</td>
    <td align="center">日付</td><td align="center">出発時間</td><td align="center">バス停を通った時間</td>
    <td align="center">バス停との距離</td><td align="center">GPSデータのid</td>
  </tr>
</table>


<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="4">task_detail</td>
  </tr>
   <tr>
    <th>テーブルの説明</th><td align="center" colspan="4">タスク内の各バス停の発車時刻を管理するテーブル</td>
  </tr>
 <tr>
    <th>カラム名</th><td align="center">task_detail_id</td><td align="center">task_id</td><td align="center">bus_stop_id</td>
    <td align="center">departure_time</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">serial</td><td align="center">integer</td><td align="center">integer</td><td align="center">time without time zone</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">not null</td><td align="center">not null</td><td align="center">---</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">PK</td><td align="center">FK</td><td align="center">FK</td><td align="center">---</td>
  </tr>
 <tr>
    <th>カラムの説明</th><td align="center">発車時刻のid</td><td align="center">タスクのid</td><td align="center">バス停のid</td>
    <td align="center">出発時間</td>
  </tr>
</table>

<table>
  <tr>
    <th>テーブル名</th><td align="center" colspan="4">user_browsing_log</td>
  </tr>
   <tr>
    <th>テーブルの説明</th><td align="center" colspan="4">ユーザ側の利用履歴を管理するテーブル</td>
  </tr>
 <tr>
    <th>カラム名</th><td align="center">session_id</td><td align="center">browsing_at</td><td align="center">event_type</td>
    <td align="center">param</td>
  </tr>
  <tr>
    <th>型名</th><td align="center">text</td><td align="center">timestamp without time zone</td><td align="center">text</td><td align="center">jsonb</td>
  </tr>
  <tr>
    <th>制約</th><td align="center">not null</td><td align="center">not null</td><td align="center">not null</td><td align="center">not null</td>
  </tr>
  <tr>
    <th>PK/FK</th><td align="center">複合PK</td><td align="center">複合PK</td><td align="center">---</td><td align="center">---</td>
  </tr>
 <tr>
    <th>カラムの説明</th><td align="center">セッション</td><td align="center">閲覧した時間</td><td align="center">イベントの種類</td>
    <td align="center">ユーザの操作ログ</td>
  </tr>
</table>
