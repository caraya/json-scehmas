# Objects

* [`JSON schema for a person`](#reference-person)
* [`JSON schema for interviews`](#reference-json-schema-for-interviews) (root object)

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

**`JSON schema for interviews` Properties**

|   |Type|Description|Required|
|---|---|---|---|
|**$schema**|`string`||No|
|**id**|`string`|Unique identifier for the block|No|
|**title**|`string`|Title of the interview|No|
|**type**|`string`|Type of interview|No, default: `"interview"`|
|**date**|`string`|Date of the interview|No|
|**location**|`string`|Location of the interview|No|
|**interviewers**|`person` `[1-5]`|Interviewer(s) of the interview|No|
|**interviewees**|`person` `[1-5]`|Subject(s) of the interview|No|
|**audio**|`object`||No|
|**transcript**|`object`||No|

Additional properties are allowed.

### JSON schema for interviews.$schema

* **Type**: `string`
* **Required**: No

### JSON schema for interviews.id

Unique identifier for the block

* **Type**: `string`
* **Required**: No

### JSON schema for interviews.title

Title of the interview

* **Type**: `string`
* **Required**: No

### JSON schema for interviews.type

Type of interview

* **Type**: `string`
* **Required**: No, default: `"interview"`
* **Allowed values**:
  * `"interview"`
  * `"interview-one-on-one"`
  * `"interview-group"`
  * `"interview-one-on-one-video"`
  * `"interview-group-video"`
  * `"interview-one-on-one-audio"`
  * `"interview-group-audio"`

### JSON schema for interviews.date

Date of the interview

* **Type**: `string`
* **Required**: No
* **Format**: date

### JSON schema for interviews.location

Location of the interview

* **Type**: `string`
* **Required**: No

### JSON schema for interviews.interviewers

Interviewer(s) of the interview

* **Type**: `person` `[1-5]`
* **Required**: No

### JSON schema for interviews.interviewees

Subject(s) of the interview

* **Type**: `person` `[1-5]`
* **Required**: No

### JSON schema for interviews.audio

* **Type**: `object`
* **Required**: No

### JSON schema for interviews.transcript

* **Type**: `object`
* **Required**: No
