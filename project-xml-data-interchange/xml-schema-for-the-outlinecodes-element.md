﻿---
title: OutlineCodes 要素の XML スキーマ
TOCTitle: OutlineCodes 要素の XML スキーマ
ms:assetid: 8db24ef2-eeee-43be-a998-9aaf90f7e5d9
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968584(v=office.12)
ms:contentKeyID: 16741971
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# OutlineCodes 要素の XML スキーマ

次に示すのは、Microsoft Office Project 2007 XML データ交換スキーマ (mspdi\_pj12.xsd) で **OutlineCodes** 要素を定義しているセクションです。

完全な Project XML データ交換スキーマは、Project 2007 SDK ダウンロードに含まれています。Project 2007 SDK ダウンロードへのリンクについては、「[Microsoft Office Project 2007 SDK へようこそ](https://msdn.microsoft.com/ja-jp/library/ms512767\(v=office.12\))」を参照してください。

## OutlineCodes のスキーマ

``` xml
<?xml version="1.0"?>
. . .
<!-- @OutlineCode schema -->
<xsd:element name="OutlineCodes" minOccurs="0">
  <xsd:annotation>
    <xsd:documentation>The collection of outline code definitions associated with the project.  These codes can be associated only with this project, or can be common among several projects (enterprise codes).</xsd:documentation>
  </xsd:annotation>
  <xsd:complexType>
    <xsd:sequence>
      <xsd:element name="OutlineCode" minOccurs="0" maxOccurs="unbounded">
        <xsd:annotation>
          <xsd:documentation>The individual outline codes.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <!-- #New Project 2007 element definition -->
            <xsd:element name="Guid" type="xsd:string">
              <xsd:annotation>
                <xsd:documentation>The GUID of the outline code.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <!-- #End new Project 2007 element definition -->
            <xsd:element name="FieldID" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Coresponds to the field number of outline code.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="FieldName" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The name of the custom outline code.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Alias" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The alias of the custom outline code.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="PhoneticAlias" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The phonetic pronunciation of the alias of the custom outline code.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Values" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The values of the table associated with this outline code.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence minOccurs="0" maxOccurs="unbounded">
                  <xsd:element name="Value">
                    <xsd:annotation>
                      <xsd:documentation>The individual values.</xsd:documentation>
                    </xsd:annotation>
                    <xsd:complexType>
                      <xsd:all>
                        <xsd:element name="ValueID" type="xsd:integer" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The unique ID of the outline code value across the project.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <!-- #New Project 2007 element definitions -->
                        <xsd:element name="FieldGUID" type="xsd:string">
                          <xsd:annotation>
                            <xsd:documentation>The GUID of the outline code value.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="Type">
                          <xsd:annotation>
                            <xsd:documentation>The outline code type. Values are: 4=Date, 6=Duration, 9=Cost, 15=Number, 17=Flag, 21=Text, 27=Finish date.</xsd:documentation>
                          </xsd:annotation>
                          <xsd:simpleType>
                            <xsd:restriction base="xsd:integer">
                              <xsd:enumeration value="4" />
                              <xsd:enumeration value="6" />
                              <xsd:enumeration value="9" />
                              <xsd:enumeration value="15" />
                              <xsd:enumeration value="17" />
                              <xsd:enumeration value="21" />
                              <xsd:enumeration value="27" />
                            </xsd:restriction>
                          </xsd:simpleType>
                        </xsd:element>
                        <!-- #End new Project 2007 element definitions -->
                        <xsd:element name="ParentValueID" type="xsd:integer" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The value of the parent node of the outline code.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="Value" type="xsd:string" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The actual value.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="Description" type="xsd:string" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>A description of this value.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                      </xsd:all>
                    </xsd:complexType>
                  </xsd:element>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
            <xsd:element name="Enterprise" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Indicates whether the custom outline code is an enterprise custom outline code.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="EnterpriseOutlineCodeAlias" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>A reference to another custom field for which this is an alias.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ResourceSubstitutionEnabled" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the custom outline code can be used by the Resource Substitution Wizard in Microsoft Office Project.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="LeafOnly" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether or not values specified in this outline code field must be leaf values.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="AllLevelsRequired" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>New codes must have all levels present.  Not available for enterprise codes.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="OnlyTableValuesAllowed" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether values specified must come from values table.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Masks" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The table of entries that define the outline code mask.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="Mask" minOccurs="0" maxOccurs="unbounded">
                    <xsd:annotation>
                      <xsd:documentation>The four elements of the mask constitute the format in which the outline code must appear.</xsd:documentation>
                    </xsd:annotation>
                    <xsd:complexType>
                      <xsd:sequence>
                        <xsd:element name="Level" type="xsd:integer" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The level of the mask.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="Type" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The type of mask. Values are: 0=Numbers, 1=Upper Case Letters, 2=Lower Case Letters, 3=Characters.</xsd:documentation>
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
                        <xsd:element name="Length" type="xsd:integer" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The maximum length in characters of the outline code values.  If length is any, the value is zero.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="Separator" type="xsd:string" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The separator value of the code values.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                      </xsd:sequence>
                    </xsd:complexType>
                  </xsd:element>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
</xsd:element>
```

## 参照

#### その他の技術情報

[OutlineCode 要素と XML データ構造](outlinecode-elements-and-xml-structure.md)

