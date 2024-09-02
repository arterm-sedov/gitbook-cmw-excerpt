---
layout:
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Forms

{% hint style="success" %}
**Definition**

A form is a web page designed to enter and display data. You can place fields (associated with attributes), static text, and visual elements on the form.
{% endhint %}

## Use the the Template's Form List

The list of forms is provided for the record template, account template, role template, and organizational unit template.

{% hint style="info" %}
**Note**

In the process template, the form list is not available, and the forms are created and configured using the process diagram element properties.
{% endhint %}

1. Open a record template, account template, role template, or organizational unit template.
2. Go to the **Forms** tab.
3. The list of forms in the template opens.
4. Perform the following operations:
   * **Select** — select a checkbox in the first column to select a form.
   * **Open** — double-click a form row to [configure ](forms.md#configure-the-form)the existging form.
   * **Create** — [configure ](forms.md#configure-the-form)a new form.
   * **Delete** — slecect a form and click **Delete**. Confirm the form deletion.
   * **Set as default** — select a form and click **Default** to set the form as default for viewing the template records.
   * **Search** — click <img src=".gitbook/assets/image (4).png" alt="" data-size="line"> and enter keywords in the **Search** field. The rows containing the keywords will be shown.

<figure><img src=".gitbook/assets/form_list" alt="Template form list"><figcaption><p>Template form list</p></figcaption></figure>

## Configure the Form

Use the form designer to configure the form layout, properties, and elements.

1. Open the template's [form list](forms.md#viewing-the-template-form-list).
2. Click **Create** or double-click a form in the list.
3. The form designer appears with the following items:\
   \
   **(1) Elements pane** — drag the elements from the pane onto the form: attributes, buttons, embedded forms, and visual elements. You can also edit and create elements [using the elements pane](forms.md#element-pane-operations).\
   **(2) Form layout** — sets the form's visual appearance.\
   **(3) Properties pane** — view and configure the properties of the selected element.\
   **(4) Buttons**
   * **Save** — save the form.
   * **Clear** — remove all elements from the form layout.
   * **Clone** — create a form duplicate.
   * **Configure template** <img src=".gitbook/assets/image (5).png" alt="" data-size="line"> — go to the template **Properties** page.
   *   **Relations** <img src=".gitbook/assets/2023-07-16_16h51_08.png" alt="" data-size="line"> — view a list of application objects that use the form.\


       <figure><img src=".gitbook/assets/form_designer" alt="Form designer"><figcaption></figcaption></figure>
4. To set the form properties, click an empty layout area and configure the properties using the properties pane:
   * **Display name** — a title displayed in the form header when viewing template records.
   * **System name** — a unique name to identify the form in scripts, expressions, and scenarios.
   * **Is default** — select this checkbox to display the form by default when viewing template records.
   * **Type**:
     * **Public** — select this type for the form to be viewed using the form selection dropdown next to the form title.
     * **Internal** — select this type for the form to be displayed only if it is embedded in another form or is set as a record form (eg. for process start, record creation, dialogues).
5. Use the elements pane to:
   * Drag the [elements](forms.md#form-elements) from the elements pane to the form layout.
   * Click <img src=".gitbook/assets/image (4).png" alt="" data-size="line"> to search for elements.
   * Click <img src=".gitbook/assets/image (6).png" alt="" data-size="line"> to filter the element list by element type.
   * [Create](forms.md#creating-an-attribute) or [edit](forms.md#editing-an-attribute-button-or-form) attributes, buttons, and forms.
6. To set a form element properties, select it in the layout and configure the properties in the properties pane.
7. **Save** the form.
8. If needed [configure the form rules](forms.md#editing-the-form).

### Form Elements <a href="#form-elements" id="form-elements"></a>

You can place the following elements on the form from the [elements pane](forms.md#configure-the-form).

* **Area** — contains all other form elements. Always place other elements in an area. The form must have at least one area. There can be several areas on a form.
* **Tabs** — arrange form elements on several tabs.
* **Columns** — arrange elements in several columns.
* **Static text** — displays arbitrary text with HTML formatting.
* **Attribute field** — drag an attribute to the form layout to create a field associated with the attribute. Field properties correspond to the associated attribute type.
* **Embedded form** — drag another form onto the form layout to embed it into the current form.
* **Button group** — combines buttons into a dropdown.
* **Button separator** — visually separates buttons within button areas.

{% hint style="info" %}
A **button area** is provided for each form and area. Always place **buttons**, **button groups**, and **button separators** in the button areas and not anywhere elsese on the form.
{% endhint %}

### Configure an Attribute, Button, or Embedded Form using the Elements Pane <a href="#creating-an-attribute" id="creating-an-attribute"></a>

#### Create an Attribute  <a href="#creating-an-attribute" id="creating-an-attribute"></a>

1. In the elements pane:
   * To create an attribute in the current template, hover over the **Attributes** heading , or…
   * To create an attribute in the corresponding template, hover over the template name in the element list.
2. Click the **Add Attribute** button that appears.
3. The attribute properties window appears.
4. Configure and save the attribute

<figure><img src=".gitbook/assets/form_designer_create_attribute" alt="Creating an attribute using the form designer"><figcaption><p>Creating an attribute using the form designer</p></figcaption></figure>

#### Create a Button <a href="#creating-a-button" id="creating-a-button"></a>

1. In the elements pane, hover over the **Buttons** heading.
2. Click the **Add button** button that appears.
3. The [button designer](buttons.md#opening-the-button-designer) appears.
4. Configure and save the button.

<figure><img src=".gitbook/assets/form_designer_create_button" alt="Creating a button in the form designer"><figcaption><p>Creating a button in the form designer</p></figcaption></figure>

#### Edit an Attribute, Button, or Embedded Form <a href="#editing-an-attribute-button-or-form" id="editing-an-attribute-button-or-form"></a>

1. Hover the mouse pointer over an attribute, button, or form name in the elements pane.
2. Click the **Edit attribute**, **Edit button**, or **Edit form** button that appears.
3. The attribute properties window, button designer, or form designer appears.
4. Configure and save the element.

<figure><img src=".gitbook/assets/form_designer_edit_form" alt="Editing a form using the form designer"><figcaption><p>Editing an embedded form using the form designer</p></figcaption></figure>

## Clone the Form <a href="#cloning-a-form" id="cloning-a-form"></a>

1. In the form designer, click **Clone**.
2. In the form cloning window, enter the form **name** and **system name**.
3. **Save** the cloned form.
4. The new form opens in the form designer.

<figure><img src=".gitbook/assets/2023-07-16_16h52_06.png" alt="Form cloning"><figcaption><p>Form cloning</p></figcaption></figure>

## Configure the Form Rules <a href="#editing-the-form-rules" id="editing-the-form-rules"></a>

1. In the designer, click the selector button next to the form title.
2. Select **Form rules** from the dropdown.
3. The rule designer for the form is displayed.
4. Edit the form rules.
5. **Save** the form rules.

<figure><img src=".gitbook/assets/form_designer_goto_form_rules" alt="Form rules designer jump menu"><figcaption><p>Form rules designer jump menu</p></figcaption></figure>
