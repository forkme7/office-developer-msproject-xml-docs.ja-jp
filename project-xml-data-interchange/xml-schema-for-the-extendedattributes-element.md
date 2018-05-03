﻿---
title: ExtendedAttributes 要素の XML スキーマ
TOCTitle: ExtendedAttributes 要素の XML スキーマ
ms:assetid: db014a14-2934-4f15-8766-0ab0dd0add22
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968705(v=office.12)
ms:contentKeyID: 16748547
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# ExtendedAttributes 要素の XML スキーマ

次に示すのは、Microsoft Office Project 2007 XML データ交換スキーマ (mspdi\_pj12.xsd) で **ExtendedAttributes** 要素を定義しているセクションです。

完全な Project データ交換スキーマは Project 2007 SDK ダウンロードに収録されています。Project 2007 SDK ダウンロードへのリンクについては、「[Microsoft Office Project 2007 SDK へようこそ](https://msdn.microsoft.com/ja-jp/library/ms512767\(v=office.12\))」を参照してください。

## ExtendedAttributes スキーマ

``` xml
<?xml version="1.0" encoding="utf-8"?>
. . .
<!-- @ExtendedAttribute schema -->
<xsd:element name="ExtendedAttributes" minOccurs="0">
  <xsd:annotation>
    <xsd:documentation>The collection of extended attribute (custom field) definitions associated with the project.</xsd:documentation>
  </xsd:annotation>
  <xsd:complexType>
    <xsd:sequence>
      <xsd:element name="ExtendedAttribute" minOccurs="0" maxOccurs="unbounded">
        <xsd:annotation>
          <xsd:documentation>Each of the individual entries in the extended attributes definition collection.  There are no limits to the number of children that may appear, but Project only understands Flag1-Flag10, etc.  There must be at least one ExtendedAttribute in each ExtendedAttributes collection.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="FieldID" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>This corresponds to the PID of the custom field.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="FieldName" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The name of the custom field.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="CFType" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The custom field type. Values are: 0=Cost, 1=Date, 2=Duration, 3=Finish, 4=Flag, 5=Number, 6=Start, 7=Text.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="0" />
                  <xsd:enumeration value="1" />
                  <xsd:enumeration value="2" />
                  <xsd:enumeration value="3" />
                  <xsd:enumeration value="4" />
                  <xsd:enumeration value="5" />
                  <xsd:enumeration value="6" />
                  <xsd:enumeration value="7" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="Guid" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The GUID of the custom field.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ElemType" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies whether the extended attribute is associated with a task, a resource, or an assignment. Values are: 20=Task, 21=Resource, 22=Calendar, 23=Assignment.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="20" />
                  <xsd:enumeration value="21" />
                  <xsd:enumeration value="22" />
                  <xsd:enumeration value="23" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="MaxMultiValues" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies the maximum number of values you can set in a picklist.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="UserDef" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies whether the custom field is user-defined.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Alias" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The alias of the custom field.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="50" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="SecondaryPID" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The secondary PID of the custom field.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="AutoRollDown" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies whether automatic rolldown to assignments is enabled.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="DefaultGuid" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies the GUID of the default lookup table entry.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Ltuid" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The GUID of the lookup table associated with the custom field.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="PhoneticAlias" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The phonetic pronunciation of the alias of the custom field.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="50" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="RollupType" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>How rollups are calculated. Values are: 0=Maximum (OR for flag fields), 1=Minimum (AND for flag fields), 2=Count all, 3=Sum, 4=Average, 5=Average First Sublevel, 6=Count First Sublevel, 7=Count Nonsummaries.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="0" />
                  <xsd:enumeration value="1" />
                  <xsd:enumeration value="2" />
                  <xsd:enumeration value="3" />
                  <xsd:enumeration value="4" />
                  <xsd:enumeration value="5" />
                  <xsd:enumeration value="6" />
                  <xsd:enumeration value="7" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="CalculationType" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether rollups are calculated for task and group summary rows. Values are: 0=None, 1=Rollup, 2=Calculation.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="0" />
                  <xsd:enumeration value="1" />
                  <xsd:enumeration value="2" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="Formula" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The formula that Microsoft Project uses to populate the custom task field.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RestrictValues" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>If RestrictValues=True then only values in the list are allowed in the file.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ValuelistSortOrder" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>How value lists are sorted. Values are: 0=Descending, 1=Ascending.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="0" />
                  <xsd:enumeration value="1" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="AppendNewValues" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>If AppendNewValues=True then any new values added in a project are automatically appended to the list.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Default" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>This points to the default value in the list.  Not present if no default is set.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ValueList" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>When values of extended attributes are specified as properties of elements in the schema, they can be specified either by values or by references to the values contained in this list.  Applications can assume ordering of the list by ordering specified here.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="Value" maxOccurs="unbounded">
                    <xsd:annotation>
                      <xsd:documentation>The values that make up the value list.</xsd:documentation>
                    </xsd:annotation>
                    <xsd:complexType>
                      <xsd:all>
                        <xsd:element name="ID" type="xsd:integer">
                          <xsd:annotation>
                            <xsd:documentation>Unique ID of value across the project.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="Value" type="xsd:string" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The actual value.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="Description" type="xsd:string" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The description of the value in the list.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="Phonetic" type="xsd:string" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>Phonetic information for custom field names.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                      </xsd:all>
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

[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[XML のユーザー設定フィールド データ](custom-field-data-in-xml.md)

