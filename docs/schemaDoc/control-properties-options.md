# Options Schema

```txt
https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options
```

Gives multiple options to configure the element

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                     |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :----------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [control.schema.json\*](../schemas/control.schema.json "open original schema") |

## options Type

`object` ([Options](control-properties-options.md))

# options Properties

| Property                                  | Type      | Required | Nullable       | Defined by                                                                                                                                                                                      |
| :---------------------------------------- | :-------- | :------- | :------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [label](#label)                           | `boolean` | Optional | cannot be null | [Control](control-properties-options-properties-label.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/label")                           |
| [multi](#multi)                           | Merged    | Optional | cannot be null | [Control](control-properties-options-properties-multi.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/multi")                           |
| [rating](#rating)                         | `boolean` | Optional | cannot be null | [Control](control-properties-options-properties-rating.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/rating")                         |
| [placeholder](#placeholder)               | `string`  | Optional | cannot be null | [Control](control-properties-options-properties-placeholder.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/placeholder")               |
| [drop-placeholder](#drop-placeholder)     | `string`  | Optional | cannot be null | [Control](control-properties-options-properties-drop-placeholder.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/drop-placeholder")     |
| [allowMultipleFiles](#allowmultiplefiles) | `boolean` | Optional | cannot be null | [Control](control-properties-options-properties-allowmultiplefiles.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/allowMultipleFiles") |
| [acceptedFileType](#acceptedfiletype)     | `string`  | Optional | cannot be null | [Control](control-properties-options-properties-acceptedfiletype.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/acceptedFileType")     |
| [enumTitles](#enumtitles)                 | `object`  | Optional | cannot be null | [Control](control-properties-options-properties-titles-for-enum.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/enumTitles")            |
| [radiobuttons](#radiobuttons)             | `boolean` | Optional | cannot be null | [Control](control-properties-options-properties-radiobuttons.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/radiobuttons")             |
| [stacked](#stacked)                       | `boolean` | Optional | cannot be null | [Control](control-properties-options-properties-stacked.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/stacked")                       |
| [buttons](#buttons)                       | Merged    | Optional | cannot be null | [Control](control-properties-options-properties-buttons.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/buttons")                       |
| [switch](#switch)                         | `boolean` | Optional | cannot be null | [Control](control-properties-options-properties-switches.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/switch")                       |
| [append](#append)                         | `string`  | Optional | cannot be null | [Control](control-properties-options-properties-append.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/append")                         |
| [tags](#tags)                             | `object`  | Optional | cannot be null | [Control](control-properties-options-properties-tags.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/tags")                             |
| [autocomplete](#autocomplete)             | `string`  | Optional | cannot be null | [Control](control-properties-options-properties-autocomplete.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/autocomplete")             |
| [textAlign](#textalign)                   | `string`  | Optional | cannot be null | [Control](control-properties-options-properties-textalign.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/textAlign")                   |
| [cssClass](#cssclass)                     | `string`  | Optional | cannot be null | [Control](control-properties-options-properties-cssclass.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/cssClass")                     |
| [hidden](#hidden)                         | `boolean` | Optional | cannot be null | [Control](control-properties-options-properties-hidden.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/hidden")                         |

## label

Defines whether the fields label is activated

`label`

*   is optional

*   Type: `boolean`

*   cannot be null

*   defined in: [Control](control-properties-options-properties-label.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/label")

### label Type

`boolean`

### label Default Value

The default value is:

```json
true
```

## multi

If set true, textarea will be shown instead of textfield.
Alternatively can be set to the number of wanted lines

`multi`

*   is optional

*   Type: merged type ([Details](control-properties-options-properties-multi.md))

*   cannot be null

*   defined in: [Control](control-properties-options-properties-multi.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/multi")

### multi Type

merged type ([Details](control-properties-options-properties-multi.md))

one (and only one) of

*   [Untitled boolean in Control](control-properties-options-properties-multi-oneof-0.md "check type definition")

*   [Untitled integer in Control](control-properties-options-properties-multi-oneof-1.md "check type definition")

## rating

If set to true, numberfield will appear as star-rating-field

`rating`

*   is optional

*   Type: `boolean`

*   cannot be null

*   defined in: [Control](control-properties-options-properties-rating.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/rating")

### rating Type

`boolean`

## placeholder

Will be shown as placeholder in form fields, if supported by field

`placeholder`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Control](control-properties-options-properties-placeholder.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/placeholder")

### placeholder Type

`string`

## drop-placeholder

Will be shown as placeholder in file upload field when file drag and drop

`drop-placeholder`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Control](control-properties-options-properties-drop-placeholder.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/drop-placeholder")

### drop-placeholder Type

`string`

## allowMultipleFiles

Allows the upload of multiple files with fileupload

`allowMultipleFiles`

*   is optional

*   Type: `boolean`

*   cannot be null

*   defined in: [Control](control-properties-options-properties-allowmultiplefiles.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/allowMultipleFiles")

### allowMultipleFiles Type

`boolean`

## acceptedFileType

The accepted File Types

`acceptedFileType`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Control](control-properties-options-properties-acceptedfiletype.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/acceptedFileType")

### acceptedFileType Type

`string`

### acceptedFileType Examples

```json
"image/*"
```

```json
"image/jpeg, image/png, image/gif"
```

```json
".jpg, .png, .gif"
```

## enumTitles

If the text in a enums select field is supposed to differ from the keys, they can be specified as properties of this object. The value in the enum must be used as property name

`enumTitles`

*   is optional

*   Type: `object` ([Titles for enum](control-properties-options-properties-titles-for-enum.md))

*   cannot be null

*   defined in: [Control](control-properties-options-properties-titles-for-enum.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/enumTitles")

### enumTitles Type

`object` ([Titles for enum](control-properties-options-properties-titles-for-enum.md))

## radiobuttons

If set to true, a group of radiobuttons will be shown instead of the select field

`radiobuttons`

*   is optional

*   Type: `boolean`

*   cannot be null

*   defined in: [Control](control-properties-options-properties-radiobuttons.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/radiobuttons")

### radiobuttons Type

`boolean`

## stacked

Radiobutton-/Checkbox group will be stacked if set to true

`stacked`

*   is optional

*   Type: `boolean`

*   cannot be null

*   defined in: [Control](control-properties-options-properties-stacked.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/stacked")

### stacked Type

`boolean`

## buttons

Render fields that support it (Radiobuttons, Checkboxgroups) as Buttons

`buttons`

*   is optional

*   Type: merged type ([Buttons](control-properties-options-properties-buttons.md))

*   cannot be null

*   defined in: [Control](control-properties-options-properties-buttons.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/buttons")

### buttons Type

merged type ([Buttons](control-properties-options-properties-buttons.md))

one (and only one) of

*   [Untitled boolean in Control](control-properties-options-properties-buttons-oneof-0.md "check type definition")

*   [Bootstrap Button Variants](button-properties-bootstrap-button-variants.md "check type definition")

## switch

If set to true, the checkbox(-group) it was specified for will be rendered as switch(es)

`switch`

*   is optional

*   Type: `boolean` ([Switch(es)](control-properties-options-properties-switches.md))

*   cannot be null

*   defined in: [Control](control-properties-options-properties-switches.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/switch")

### switch Type

`boolean` ([Switch(es)](control-properties-options-properties-switches.md))

## append

Will be appended to field

`append`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Control](control-properties-options-properties-append.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/append")

### append Type

`string`

## tags

Will be rendered as tags-Field

`tags`

*   is optional

*   Type: `object` ([Details](control-properties-options-properties-tags.md))

*   cannot be null

*   defined in: [Control](control-properties-options-properties-tags.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/tags")

### tags Type

`object` ([Details](control-properties-options-properties-tags.md))

## autocomplete

Specifies what should be autocompleted by the browser. Possible values are listed here: <https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes/autocomplete#values>

`autocomplete`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Control](control-properties-options-properties-autocomplete.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/autocomplete")

### autocomplete Type

`string`

## textAlign

Set the text-align of input fields

`textAlign`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Control](control-properties-options-properties-textalign.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/textAlign")

### textAlign Type

`string`

### textAlign Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value      | Explanation |
| :--------- | :---------- |
| `"left"`   |             |
| `"right"`  |             |
| `"center"` |             |
| `"start"`  |             |
| `"end"`    |             |

## cssClass

The Controls CSS classes

`cssClass`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Control](control-properties-options-properties-cssclass.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/cssClass")

### cssClass Type

`string`

### cssClass Examples

```json
"bg-primary"
```

```json
"bg-info specialpart"
```

## hidden

Sets the visibility of the field to hidden. For example useful in combination with a DateTime field with default:"$now" to create a hidden timestamp.

`hidden`

*   is optional

*   Type: `boolean`

*   cannot be null

*   defined in: [Control](control-properties-options-properties-hidden.md "https://educorvi.github.io/vue_json_form/schemas/control.schema.json#/properties/options/properties/hidden")

### hidden Type

`boolean`
