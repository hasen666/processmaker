---
description: >-
  Add a control from which the Request participant can insert more than three
  lines of text.
---

# Textarea Control Settings

## Control Description

The Textarea control allows the [Request](../../../../using-processmaker/requests/what-is-a-request.md) participant to insert more than three lines of text. Configure the Textarea control to accept one of the following data types:

* **Text:** The control accepts alphanumeric characters.
* **Integer:** The control accepts integers.
* **Decimal:** The control accepts any number, both positive and negative.
* **Datetime:** The control accepts a datetime, which is includes both date and time components.
* **Date:** The control accepts a date.

Though this control displays a vertical scroll bar if more than three lines are inserted, the input box can be expanded as necessary. To do this, click the lower right-hand corner of the input box of the Textarea control, hold, and then drag to enlarge or shrink the control size as necessary. Release when you have adjusted the Textarea control to your required size.

{% hint style="info" %}
This control is not available for [Display](../types-for-screens.md#display)-type ProcessMaker Screens. See [Screen Types](../types-for-screens.md).
{% endhint %}

## Add the Control to a ProcessMaker Screen <a id="add-the-control-to-a-processmaker-screen"></a>

{% hint style="info" %}
Your ProcessMaker user account or group membership must have the following permissions to add a control to a ProcessMaker Screen unless your user account has the **Make this user a Super Admin** setting selected:

* Screens: View Screens
* Screens: Edit Screens

See the ProcessMaker [Screens](../../../../processmaker-administration/permission-descriptions-for-users-and-groups.md#screens) permissions or ask your ProcessMaker Administrator for assistance.
{% endhint %}

Follow these steps to add this control to the ProcessMaker Screen:

1. [Create a new ProcessMaker Screen](../../manage-forms/create-a-new-form.md) or click the **Edit** icon![](../../../../.gitbook/assets/edit-icon.png)to edit the selected Screen. The ProcessMaker Screen is in [Design mode](../screens-builder-modes.md#editor-mode).
2. View the ProcessMaker Screen page to which to add the control.
3. Locate the **Textarea** icon![](../../../../.gitbook/assets/textarea-control-screens-builder-processes.png)in the panel to the left of the Screens Builder canvas.
4. Drag the **Textarea** icon into the Screens Builder canvas. Existing controls on the Screens Builder canvas adjust positioning based on where you drag the control.
5. Place into the Screens Builder canvas where you want the control to display on the ProcessMaker Screen.

   ![](../../../../.gitbook/assets/textarea-control-placed-screens-builder-processes.png)

6. Configure the Textarea control. See [Settings](textarea-control-settings.md#inspector-settings).
7. Validate that the control is configured correctly. See [Validate Your Screen](../validate-your-screen.md#validate-a-processmaker-screen).

Below is a Textarea control in [Preview mode](../screens-builder-modes.md#preview-mode).

![Textarea control in Preview mode](../../../../.gitbook/assets/textarea-control-placed-screens-builder-processes%20%281%29.png)

## Delete the Control from a ProcessMaker Screen

{% hint style="warning" %}
Deleting a control also deletes configuration for that control. If you add another control, it will have default settings.
{% endhint %}

Click the **Delete** icon![](../../../../.gitbook/assets/delete-screen-control-screens-builder-processes.png)for the control to delete it.

## Settings <a id="inspector-settings"></a>

{% hint style="info" %}
Your user account or group membership must have the following permissions to edit a ProcessMaker Screen control:

* Screens: View Screens
* Screens: Edit Screens

See the ProcessMaker [Screens](../../../../processmaker-administration/permission-descriptions-for-users-and-groups.md#screens) permissions or ask your ProcessMaker Administrator for assistance.
{% endhint %}

The Textarea control has the following panels that contain settings:

* \*\*\*\*[**Variable** panel](textarea-control-settings.md#variable-panel-settings)
* \*\*\*\*[**Configuration** panel](textarea-control-settings.md#configuration-panel-settings)
* \*\*\*\*[**Design** panel](textarea-control-settings.md#design-panel-settings)
* \*\*\*\*[**Advanced** panel](textarea-control-settings.md#advanced-panel-settings)

### Variable Panel Settings

Click the control while in [Design](../screens-builder-modes.md#design-mode) mode, and then click the **Variable** panel that is on the right-side of the Screens Builder canvas.

Below are settings for the Textarea control in the **Variable** panel:

* **Variable Name:** Enter a unique name containing at least one letter that represents this control's value. Use the **Variable Name** value in the following ways:

  * Reference this control by its **Variable Name** setting's value. The **Data Preview** panel in [Preview mode](../screens-builder-modes.md#preview-mode) corresponds the Textarea control's textual content with that Textarea control's **Variable Name** value. In the example below, `TextareaControl` is the **Variable Name** setting's value. ![](../../../../.gitbook/assets/textarea-preview-screens-builder-processes.png) 
  * Reference this control's value in a different Screens Builder control. To do so, use mustache syntax and reference this control's **Variable Name** value in the target control. Example: `{{ TextareaControl }}`.
  * Reference this value in [**Visibility Rule** setting expressions](expression-syntax-components-for-show-if-control-settings.md).

  This is a required setting.

* **Data Type:** Select one of the following data type options this control accepts when the form user enters content into this control:

  * **Text:** This control accepts alphanumeric characters.
  * **Integer:** This control accepts integers.
  * **Decimal:** This control accepts any number, both positive and negative.
  * **Datetime:** This control accepts a datetime, which is includes both date and time components.
  * **Date:** The control accepts a date.

  This is a required setting. The following message displays below the control if the Request participant enters content that does not comply with this control's data type: **The format is invalid.**.

* **Validation Rules:** Enter the validation rules the Request participant must comply with to properly enter a valid value into this control. This setting has no default value. See [Validation Rules for "Validation" Control Settings](validation-rules-for-validation-control-settings.md).
* **Read Only:** Select to indicate that the Textarea control cannot be edited. This option is not selected by default.

### Configuration Panel Settings

Click the control while in [Design](../screens-builder-modes.md#design-mode) mode, and then click the **Configuration** panel that is on the right-side of the Screens Builder canvas.

Below are settings for the Textarea control in the **Configuration** panel:

* **Label:** Enter the text label that displays for this control. **New TextArea** is the default value.
* **Placeholder:** Enter the placeholder text that displays in this control when no value has been provided. This setting has no default value.
* **Helper Text:** Enter text that provides additional guidance on this control's use. This setting has no default value.
* **Rich Text:** Select the **Rich Text** checkbox to display the What-You-See-Is-What-You-Get \(WYSIWYG\) rich text editor to allow the Request participant can enter rich text. This option is not selected by default.
* **Rows:** The number of rows to provide for input. **2** is the default value.

### Design Panel Settings

Click the control while in [Design](../screens-builder-modes.md#design-mode) mode, and then click the **Design** panel that is on the right-side of the Screens Builder canvas.

Below are settings for the Textarea control in the **Design** panel:

* **Text Color:** Select to specify the text color that displays in this control.
* **Background Color:** Select to specify the background color of this control.

### Advanced Panel Settings

Click the control while in [Design](../screens-builder-modes.md#design-mode) mode, and then click the **Advanced** panel that is on the right-side of the Screens Builder canvas.

Below are settings for the Textarea control in the **Advanced** panel:

* **Visibility Rule:** Enter an expression that indicates the condition\(s\) under which this control displays. See [Expression Syntax Components for "Visibility Rule" Control Settings](expression-syntax-components-for-show-if-control-settings.md#expression-syntax-components-for-show-if-control-settings). If this setting does not have an expression, then this control displays by default.
* **CSS Selector Name:** Enter the value to represent this control in custom CSS syntax when in [Custom CSS](../add-custom-css-to-a-screen.md#add-custom-css-to-a-processmaker-screen) mode. As a best practice, use the same **CSS Selector Name** value on different controls of the same type to apply the same custom CSS style to all those controls.

## Related Topics <a id="related-topics"></a>

{% page-ref page="../types-for-screens.md" %}

{% page-ref page="../validate-your-screen.md" %}

{% page-ref page="./" %}

{% page-ref page="processmaker-collection-controls/collection-select-control-settings.md" %}

{% page-ref page="processmaker-collection-controls/collection-record-control-settings.md" %}

{% page-ref page="rich-text-control-settings.md" %}

{% page-ref page="line-input-control-settings.md" %}

{% page-ref page="select-list-control-settings.md" %}

{% page-ref page="select-control-settings.md" %}

{% page-ref page="radio-group-control-settings.md" %}

{% page-ref page="checkbox-control-settings.md" %}

{% page-ref page="date-picker-control-settings.md" %}

{% page-ref page="page-navigation-button-control-settings.md" %}

{% page-ref page="multi-column-button-control-settings.md" %}

{% page-ref page="record-list-control-settings.md" %}

{% page-ref page="image-control-settings.md" %}

{% page-ref page="submit-button-control-settings.md" %}

{% page-ref page="file-upload-control-settings.md" %}

{% page-ref page="file-download-control-settings.md" %}

{% page-ref page="expression-syntax-components-for-show-if-control-settings.md" %}
