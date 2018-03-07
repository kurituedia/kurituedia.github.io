---
layout: default
title: markdown Tests
---

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
