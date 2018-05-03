---
title: WBSMasks 要素の XML スキーマ
TOCTitle: WBSMasks 要素の XML スキーマ
ms:assetid: 822ec84d-c92a-419d-a0bf-905f5d1da8cc
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968565(v=office.12)
ms:contentKeyID: 16741000
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# WBSMasks 要素の XML スキーマ

次に示すのは、Microsoft Office Project 2007 XML データ交換スキーマ (mspdi\_pj12.xsd) で **WBSMasks** 要素を定義しているセクションです。

完全な Project XML データ交換スキーマは、Project 2007 SDK ダウンロードに含まれています。Project 2007 SDK ダウンロードへのリンクについては、「[Microsoft Office Project 2007 SDK へようこそ](https://msdn.microsoft.com/ja-jp/library/ms512767\(v=office.12\))」を参照してください。

## WBSMasks スキーマ

``` xml
<?xml version="1.0" encoding="utf-8"?>
. . .
<!-- @WBSMask schema -->
<xsd:element name="WBSMasks" minOccurs="0">
  <xsd:annotation>
    <xsd:documentation>The table of entries that define the outline code mask.</xsd:documentation>
  </xsd:annotation>
  <xsd:complexType>
    <xsd:sequence>
      <xsd:element name="VerifyUniqueCodes" type="xsd:boolean" default="false" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation>Whether work breakdown structure (WBS) codes are unique for new tasks.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="GenerateCodes" type="xsd:boolean" default="false" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation>Whether WBS codes are generated for new tasks.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="Prefix" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation>The prefix for all WBS codes.</xsd:documentation>
        </xsd:annotation>
        <xsd:simpleType>
          <xsd:restriction base="xsd:string">
            <xsd:maxLength value="50" />
          </xsd:restriction>
        </xsd:simpleType>
      </xsd:element>
      <xsd:element name="WBSMask" minOccurs="0" maxOccurs="unbounded">
        <xsd:annotation>
          <xsd:documentation>The WBS mask that is applied to all tasks in the project.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="Level" type="xsd:integer">
              <xsd:annotation>
                <xsd:documentation>The level of the mask.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Type">
              <xsd:annotation>
                <xsd:documentation>The type of the node value.  The values are: 0=Numbers, 1=Uppercase Letters, 2=Lowercase Letters, 3=Characters.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="0" />
                  <xsd:enumeration value="1" />
                  <xsd:enumeration value="2" />
                  <xsd:enumeration value="3" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="Length" type="xsd:string">
              <xsd:annotation>
                <xsd:documentation>The maximum length in characters.  This element is omitted when length is "any".</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Separator" type="xsd:string">
              <xsd:annotation>
                <xsd:documentation>The separator character of the node.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
</xsd:element>
```

## 参照

#### リファレンス

[WBSMask 要素](wbsmask-elements-and-xml-structure.md)

