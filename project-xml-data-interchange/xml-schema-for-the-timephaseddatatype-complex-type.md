﻿---
title: TimephasedDataType 複合型の XML スキーマ
TOCTitle: TimephasedDataType 複合型の XML スキーマ
ms:assetid: f500fe0e-9b75-43ac-8aa5-81b914984b4b
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968734(v=office.12)
ms:contentKeyID: 16750604
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# TimephasedDataType 複合型の XML スキーマ

次のスキーマは、**TimephasedDataType** 複合型を定義する Microsoft Office Project 2007 データ交換スキーマ (mspdi\_pj12.xsd) のセクションを示しています。

完全な Project データ交換スキーマは Project 2007 SDK ダウンロードに収録されています。Project 2007 SDK ダウンロードへのリンクについては、「[Microsoft Office Project 2007 SDK へようこそ](https://msdn.microsoft.com/ja-jp/library/ms512767\(v=office.12\))」を参照してください。

## TimephasedDataType スキーマ

``` xml
<?xml version="1.0" encoding="utf-8"?>
<!-- data type definitions - @TimephasedData schema -->
<xsd:complexType name="TimephasedDataType">
  <xsd:annotation>
    <xsd:documentation>The definition of the timephased data block.</xsd:documentation>
  </xsd:annotation>
  <xsd:sequence>
    <xsd:element name="Type" minOccurs="0">
      <xsd:annotation>
        <xsd:documentation>
          The type of task timephased data. Values are:
          1=Assignment Remaining Work
          2=Assignment Actual Work
          3=Assignment Actual Overtime Work
          4=Assignment Baseline Work
          5=Assignment Baseline Cost
          6=Assignment Actual Cost
          7=Resource Baseline Work
          8=Resource Baseline Cost
          9=Task Baseline Work
          10=Task Baseline Cost
          11=Task Percent Complete
          16=Assignment Baseline 1 Work
          17=Assignment Baseline 1 Cost
          18=Task Baseline 1 Work
          19=Task Baseline 1 Cost
          20=Resource Baseline 1 Work
          21=Resource Baseline 1 Cost
          22=Assignment Baseline 2 Work
          23=Assignment Baseline 2 Cost
          24=Task Baseline 2 Work
          25=Task Baseline 2 Cost
          26=Resource Baseline 2 Work
          27=Resource Baseline 2 Cost
          28=Assignment Baseline 3 Work
          29=Assignment Baseline 3 Cost
          30=Task Baseline 3 Work
          31=Task Baseline 3 Cost
          32=Resource Baseline 3 Work
          33=Resource Baseline 3 Cost
          34=Assignment Baseline 4 Work
          35=Assignment Baseline 4 Cost
          36=Task Baseline 4 Work
          37=Task Baseline 4 Cost
          38=Resource Baseline 4 Work
          39=Resource Baseline 4 Cost
          40=Assignment Baseline 5 Work
          41=Assignment Baseline 5 Cost
          42=Task Baseline 5 Work
          43=Task Baseline 5 Cost
          44=Resource Baseline 5 Work
          45=Resource Baseline 5 Cost
          46=Assignment Baseline 6 Work
          47=Assignment Baseline 6 Cost
          48=Task Baseline 6 Work
          49=Task Baseline 6 Cost
          50=Resource Baseline 6 Work
          51=Resource Baseline 6 Cost
          52=Assignment Baseline 7 Work
          53=Assignment Baseline 7 Cost
          54=Task Baseline 7 Work
          55=Task Baseline 7 Cost
          56=Resource Baseline 7 Work
          57=Resource Baseline 7 Cost
          58=Assignment Baseline 8 Work
          59=Assignment Baseline 8 Cost
          60=Task Baseline 8 Work
          61=Task Baseline 8 Cost
          62=Resource Baseline 8 Work
          63=Resource Baseline 8 Cost
          64=Assignment Baseline 9 Work
          65=Assignment Baseline 9 Cost
          66=Task Baseline 9 Work
          67=Task Baseline 9 Cost
          68=Resource Baseline 9 Work
          69=Resource Baseline 9 Cost
          70=Assignment Baseline 10 Work
          71=Assignment Baseline 10 Cost
          72=Task Baseline 10 Work
          73=Task Baseline 10 Cost
          74=Resource Baseline 10 Work
          75=Resource Baseline 10 Cost
          76=Physical Percent Complete
        </xsd:documentation>
      </xsd:annotation>
      <xsd:simpleType>
        <xsd:restriction base="xsd:integer">
          <xsd:enumeration value="1" />
          <xsd:enumeration value="2" />
          <xsd:enumeration value="3" />
          <xsd:enumeration value="4" />
          <xsd:enumeration value="5" />
          <xsd:enumeration value="6" />
          <xsd:enumeration value="7" />
          <xsd:enumeration value="8" />
          <xsd:enumeration value="9" />
          <xsd:enumeration value="10" />
          <xsd:enumeration value="11" />
          <xsd:enumeration value="16" />
          <xsd:enumeration value="17" />
          <xsd:enumeration value="18" />
          <xsd:enumeration value="19" />
          <xsd:enumeration value="20" />
          <xsd:enumeration value="21" />
          <xsd:enumeration value="22" />
          <xsd:enumeration value="23" />
          <xsd:enumeration value="24" />
          <xsd:enumeration value="25" />
          <xsd:enumeration value="26" />
          <xsd:enumeration value="27" />
          <xsd:enumeration value="28" />
          <xsd:enumeration value="29" />
          <xsd:enumeration value="30" />
          <xsd:enumeration value="31" />
          <xsd:enumeration value="32" />
          <xsd:enumeration value="33" />
          <xsd:enumeration value="34" />
          <xsd:enumeration value="35" />
          <xsd:enumeration value="36" />
          <xsd:enumeration value="37" />
          <xsd:enumeration value="38" />
          <xsd:enumeration value="39" />
          <xsd:enumeration value="40" />
          <xsd:enumeration value="41" />
          <xsd:enumeration value="42" />
          <xsd:enumeration value="43" />
          <xsd:enumeration value="44" />
          <xsd:enumeration value="45" />
          <xsd:enumeration value="46" />
          <xsd:enumeration value="47" />
          <xsd:enumeration value="48" />
          <xsd:enumeration value="49" />
          <xsd:enumeration value="50" />
          <xsd:enumeration value="51" />
          <xsd:enumeration value="52" />
          <xsd:enumeration value="53" />
          <xsd:enumeration value="54" />
          <xsd:enumeration value="55" />
          <xsd:enumeration value="56" />
          <xsd:enumeration value="57" />
          <xsd:enumeration value="58" />
          <xsd:enumeration value="59" />
          <xsd:enumeration value="60" />
          <xsd:enumeration value="61" />
          <xsd:enumeration value="62" />
          <xsd:enumeration value="63" />
          <xsd:enumeration value="64" />
          <xsd:enumeration value="65" />
          <xsd:enumeration value="66" />
          <xsd:enumeration value="67" />
          <xsd:enumeration value="68" />
          <xsd:enumeration value="69" />
          <xsd:enumeration value="70" />
          <xsd:enumeration value="71" />
          <xsd:enumeration value="72" />
          <xsd:enumeration value="73" />
          <xsd:enumeration value="74" />
          <xsd:enumeration value="75" />
          <xsd:enumeration value="76" />
        </xsd:restriction>
      </xsd:simpleType>
    </xsd:element>
    <xsd:element name="UID" type="xsd:integer">
      <xsd:annotation>
        <xsd:documentation>The unique identifier of the timephased data record.</xsd:documentation>
      </xsd:annotation>
    </xsd:element>
    <xsd:element name="Start" type="xsd:dateTime" minOccurs="0">
      <xsd:annotation>
        <xsd:documentation>The start date of the timephased data period.</xsd:documentation>
      </xsd:annotation>
    </xsd:element>
    <xsd:element name="Finish" type="xsd:dateTime" minOccurs="0">
      <xsd:annotation>
        <xsd:documentation>The finish date of the timephased data period.</xsd:documentation>
      </xsd:annotation>
    </xsd:element>
    <xsd:element name="Unit" minOccurs="0">
      <xsd:annotation>
        <xsd:documentation>The time unit of the timephased data period. Values are: 0=m, 1=h, 2=d, 3=w, 5=mo, 8=y.</xsd:documentation>
      </xsd:annotation>
      <xsd:simpleType>
        <xsd:restriction base="xsd:integer">
          <xsd:enumeration value="0" />
          <xsd:enumeration value="1" />
          <xsd:enumeration value="2" />
          <xsd:enumeration value="3" />
          <xsd:enumeration value="5" />
          <xsd:enumeration value="8" />
        </xsd:restriction>
      </xsd:simpleType>
    </xsd:element>
    <xsd:element name="Value" type="xsd:string" minOccurs="0">
      <xsd:annotation>
        <xsd:documentation>The value per unit of time for the timephased data period.</xsd:documentation>
      </xsd:annotation>
    </xsd:element>
  </xsd:sequence>
</xsd:complexType>
```

## 参照

#### その他の技術情報

[TimephasedDataType 要素と XML データ構造](timephaseddatatype-elements-and-xml-structure.md)

