#  (ao-react-redux-form)

ao react form components - react and redux and redux-form are required

<dl>
<dt><a href="#AOButton">AOButton</a></dt>
<dd><p>Creates a button.</p>
</dd>
<dt><a href="#AOCheckbox">AOCheckbox</a></dt>
<dd><p>Creates a checkbox input.</p>
</dd>
<dt><a href="#AODateInput">AODateInput</a></dt>
<dd><p>Date Input - uses the default browser date picker.</p>
</dd>
<dt><a href="#AODialog">AODialog</a></dt>
<dd><p>Manages a dialog for the user.</p>
</dd>
<dt><a href="#AOFormElement">AOFormElement</a></dt>
<dd><p>Base class for all text, textarea, select, and radio button components. Handles the generation
of labels, setting some basic classes for .</p>
</dd>
<dt><a href="#AOFormLine">AOFormLine</a></dt>
<dd><p>A form line for grouping input values.</p>
</dd>
<dt><a href="#AORadioInput">AORadioInput</a></dt>
<dd><p>DISCLAIMER - THIS HASNT BEEN USED OR TESTED YET - so it might not create a radio input.</p>
</dd>
<dt><a href="#AOReadOnly">AOReadOnly</a></dt>
<dd><p>Creates an readonly field.</p>
</dd>
<dt><a href="#AOSelect">AOSelect</a></dt>
<dd><p>Creates an dropdown input.</p>
</dd>
<dt><a href="#AOTextArea">AOTextArea</a></dt>
<dd><p>DISCLAIMER - THS HAS NOT BEEN USED OR TESTED YET so it may not create a textarea input.</p>
</dd>
<dt><a href="#AOTextInput">AOTextInput</a></dt>
<dd><p>Creates a text input.</p>
</dd>
<dt><a href="#SectionHeading">SectionHeading</a></dt>
<dd><p>Creating a heading for a new section in the page.</p>
</dd>
<dt><a href="#WithFormProps">WithFormProps</a></dt>
<dd><p>Injects properties into all the descendents of component before they are rendered.</p>
</dd>
</dl>


<a name="AOButton"></a>

## AOButton

Creates a button.

### Properties

| Property | Type | Description | Default |
| -------- | ---- | ----------- | ------- |
| *caption* | string | text to display on the button | 
| *handlers* | objectOf | object to hold all the event handlers | `{}`
| *name* | string | name of the component must match the name in the redux store | 
| *id* | string | unique identifier | 
| *transition* | bool | indicates if the transition should occur | `false`


---

<a name="AOCheckbox"></a>

## AOCheckbox

Creates a checkbox input.

### Properties

| Property | Type | Description | Default |
| -------- | ---- | ----------- | ------- |
| *id* | string | the id of the component | 
| *name* | string | Expression to evaulate to the store field | 
| *label* | string | Text to display in the form | `''`
| *handlers* | objectOf | object of event handlers | `{}`
| *transition* | bool | indicates if the transition should occur | `false`
| *meta* | objectOf | redux-form meta properties | `{}`


---

<a name="AODateInput"></a>

## AODateInput

Date Input - uses the default browser date picker.

### Properties

| Property | Type | Description | Default |
| -------- | ---- | ----------- | ------- |
| *id* | string | the id of the component | 
| *name* | string | Expression to evaulate to the store field | 
| *handlers* | objectOf | object of event handlers | `{}`
| *transition* | bool | indicates if the transition should occur | `false`


---

<a name="AODialog"></a>

## AODialog

Manages a dialog for the user.

### Properties

| Property | Type | Description | Default |
| -------- | ---- | ----------- | ------- |
| *title* | string | The title of the dialog | `'Auto-Owners Insurance Company'`
| *isOpen* | bool | True if the dialog should be open.  Defaults to false. | `false`
| *onClose* | func | Function to call to set isOpen to false and trigger other affects.  Default funtion t | 
| *transition* | bool | indicates if the transition should occur | `false`

### import

```jsx
import { AODialog } from "ao-react-redux-form";
```

---

<a name="AOFormElement"></a>

## AOFormElement

Base class for all text, textarea, select, and radio button components. Handles the generation
of labels, setting some basic classes for .

### Properties

| Property | Type | Description | Default |
| -------- | ---- | ----------- | ------- |
| *aoUiType* | string | type of ao component to render from aoFieldTypes | 
| *label* | string | text to display as the label | `''`
| *showSpinner* | bool | used to determine if a spinner icon should display to the right of the field | `false`
| *spinnerClass* | string | css class to use for the spinner - used to set the size of the spinner | `''`
| *name* | string | name of the field - should match the field name in the redux store | 
| *id* | string | unique id for the field | 
| *lineSize* | string | ao_ui line size for the line - usually this is passed in for you via the WithFormProps component | `'M'`
| *uiSize* | string | ai_ui size for the field | `'L'`
| *addlClassName* | string | any additional css classes to be applied | `''`
| *transition* | bool | set this to true if you want to use transitions when a field becomes visible | `false`
| *value* | any | the display value for read only field | `''`
| *caption* | string | caption to display on a button | `''`
| *handlers* | objectOf | object of event handlers | `{}`
| *options* | arrayOf | the options for a select | `[]`

### import

```jsx
import { AOFormElement } from "ao-react-redux-form";
```

---

<a name="AOFormLine"></a>

## AOFormLine

A form line for grouping input values.

### Properties

| Property | Type | Description | Default |
| -------- | ---- | ----------- | ------- |
| *lineSize* | string | ao_ui line size to use - usually gets passed in for you via WithFormProps component | `'M'`

### import

```jsx
import { AOFormLine } from "ao-react-redux-form";
```

---

<a name="AORadioInput"></a>

## AORadioInput

DISCLAIMER - THIS HASNT BEEN USED OR TESTED YET - so it might not create a radio input.

### Properties

| Property | Type | Description | Default |
| -------- | ---- | ----------- | ------- |
| *id* | string | the id of the component | 
| *name* | string | Expression to evaulate to the store field | 
| *label* | string | Text to display in the form | `''`
| *handlers* | objectOf | object of event handlers | `{}`
| *transition* | bool | indicates if the transition should occur | `false`


---

<a name="AOReadOnly"></a>

## AOReadOnly

Creates an readonly field.

### Properties

| Property | Type | Description | Default |
| -------- | ---- | ----------- | ------- |
| *name* | string | name of the component must match the name in the redux store | 
| *id* | string | unique identifier | 
| *transition* | bool | indicates if the transition should occur | `false`
| *displayValue* | string | value to display | `''`


---

<a name="AOSelect"></a>

## AOSelect

Creates an dropdown input.

### Properties

| Property | Type | Description | Default |
| -------- | ---- | ----------- | ------- |
| *name* | string | name of the component must match the name in the redux store | 
| *id* | string | unique identifier | 
| *transition* | bool | indicates if the transition should occur | `false`
| *handlers* | objectOf | object to hold all the event handlers | `{}`
| *label* |  |  | `''`


---

<a name="AOTextArea"></a>

## AOTextArea

DISCLAIMER - THS HAS NOT BEEN USED OR TESTED YET so it may not create a textarea input.

### Properties

| Property | Type | Description | Default |
| -------- | ---- | ----------- | ------- |
| *name* | string | name of the component must match the name in the redux store | 


---

<a name="AOTextInput"></a>

## AOTextInput

Creates a text input.

### Properties

| Property | Type | Description | Default |
| -------- | ---- | ----------- | ------- |
| *name* | string | name of the component must match the name in the redux store | 
| *id* | string | unique identifier | 
| *transition* | bool | indicates if the transition should occur | `false`
| *handlers* | objectOf | object to hold all the event handlers | `{}`


---

<a name="SectionHeading"></a>

## SectionHeading

Creating a heading for a new section in the page.

### Properties

| Property | Type | Description | Default |
| -------- | ---- | ----------- | ------- |
| *addlClassName* | string | additional css class to apply, ao_ui class ao-heading-400 is already set | `''`
| *heading* | string | the text you need to display as the heading | 

### import

```jsx
import { SectionHeading } from "ao-react-redux-form";
```

---

<a name="WithFormProps"></a>

## WithFormProps

Injects properties into all the descendents of component before they are rendered.

### Properties

| Property | Type | Description | Default |
| -------- | ---- | ----------- | ------- |
| *lineSize* |  |  | `'M'`

### import

```jsx
import { WithFormProps } from "ao-react-redux-form";
```

---


