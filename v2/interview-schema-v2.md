# Objects
* [`JSON schema for a person`](#reference-person)
* [`JSON schema for interviews`](#reference-json-schema-for-interviews) (root object)




---------------------------------------
<a name="reference-media"></a>
## JSON schema for a media file and references

Record of the media used for interview

**`JSON schema for a media file and references` Properties**

|   |Type|Description|Required|
|---|---|---|---|
|**kind**|`string`|Kind of media used for the interview.

The "n\a" value is used for interviews that were not recorded and where a paper transcript may exist that needs to be manually added.| &#10003; Yes|
|**format**|`string`|Format of the media recorded for interview (where applicable)| &#10003; Yes|
|**url**|`string`|URL of the media file (where applicable)| &#10003; Yes|
|**duration**|`number`|Duration of the media file| &#10003; Yes|
|**duration_unit**|`string`|| &#10003; Yes|

Additional properties are allowed.

### media.kind

Kind of media used for the interview.

The "n\a" value is used for interviews that were not recorded and where a paper transcript may exist that needs to be manually added.

* **Type**: `string`
* **Required**:  &#10003; Yes
* **Allowed values**:
    * `"audio"`
    * `"video"`
    * `"n/a"`

### media.format

Format of the media recorded for interview (where applicable)

* **Type**: `string`
* **Required**:  &#10003; Yes

### media.url

URL of the media file (where applicable)

* **Type**: `string`
* **Required**:  &#10003; Yes

### media.duration

Duration of the media file

* **Type**: `number`
* **Required**:  &#10003; Yes

### media.duration_unit

* **Type**: `string`
* **Required**:  &#10003; Yes




---------------------------------------
<a name="reference-person"></a>
## JSON schema for a person

**`JSON schema for a person` Properties**

|   |Type|Description|Required|
|---|---|---|---|
|**name**|`string`|Name of the person| &#10003; Yes|
|**email**|`string`|Email of the person|No|

Additional properties are allowed.

### person.name

Name of the person

* **Type**: `string`
* **Required**:  &#10003; Yes

### person.email

Email of the person

* **Type**: `string`
* **Required**: No




---------------------------------------
<a name="reference-json-schema-for-interviews"></a>
## JSON schema for interviews

JSON schema for interviews

Additional properties are allowed.


