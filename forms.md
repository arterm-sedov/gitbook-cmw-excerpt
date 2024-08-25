# Forms

{% hint style="success" %}
**Definition**

A form is a web page designed to enter and display data. You can place fields (associated with attributes), static text, and visual elements on the form.
{% endhint %}

### View the Template Form List

The list of forms is provided for the record template, account template, role template, and organizational unit template.

{% hint style="info" %}
**Note**

In the process template, the form list is not available, and the forms are created and configured using the process diagram element properties.
{% endhint %}

1. Open a record template, account template, role template, or organizational unit template.
2. Select the **Forms** tab.
3. The list of forms in the template opens.
4. You can perform the following operations in the form list:

* **Select** — check a box in the first column to select a form.
* **Open** — double-click a form row to [configure ](forms.md#configure-the-form)the existging form.
* **Create** — [configure ](forms.md#configure-the-form)a new form.
* **Delete** — slecect a form and click **Delete** to delete the form. Confirm the deletion.
* **Default** — select a form and click this button to set the selected form as default for viewing the template records.
* **Search** <img src=".gitbook/assets/image (4).png" alt="" data-size="line">— click this button and enter keywords in the **Search** field. The rows containing the keywords will be shown.

<figure><img src=".gitbook/assets/form_list" alt="Template form list"><figcaption><p>Template form list</p></figcaption></figure>

### Configure the form

Use the form designer to configure the form layout, properties, and elements.

1. Open the template [form list](forms.md#viewing-the-template-form-list).
2. Click **Create** or double click a form in the list.
3.  The form designer appears with the following items:

    1. **Elements panel** — drag the elements from the panel onto the form: attributes, buttons, embedded forms, and visual elements. You can also edit and create elements. See [Use the Elements Panel](forms.md#element-pane-operations).
    2. **Form layout** — sets the form's visual appearance.
    3. **Properties panel** — view and configure the properties of the selected element.
    4. Buttons:
       * **Save** — save the form.
       * **Clear** — remove all elements from the form layout.
       * **Clone** — create a form duplicate.
       * **Configure template** <img src=".gitbook/assets/image (5).png" alt="" data-size="line"> — go to the template **Properties** page.
       * **Relations** <img src=".gitbook/assets/2023-07-16_16h51_08.png" alt="" data-size="line"> — view a list of application objects that use the form.

    <figure><img src=".gitbook/assets/form_designer" alt="Form designer"><figcaption></figcaption></figure>
4. To set the form properties, click an empty layout area and configure the properties using the properties panel:
   * **Display name** — the form name that will be displayed in its header when viewing template records.
   * **System name** — a unique form name, for use in scripts, expressions, and scenarios.
   * **Is default** — check this box to display this form by default when viewing template records.
   * **Type**:
     * **Public** — select this type for the form to be viewed using the form selection dropdown next to the form title.
     * **Internal** — select this type for the form to be displayed only if it is embedded in another form or is set as a record form (eg. for process start, record creation, dialogues).
5. Drag the [elements](forms.md#form-elements) from the elements panel to the form layout.
6. To set a form element properties, select it in the layout and configure the properties in the properties panel.
7. If needed edit or create attributes, buttons, or forms [using the elements panel](forms.md#element-pane-operations).
8. Click **Save**.
9. If needed [edit the form rules](forms.md#editing-the-form).

### Form Elements <a href="#form-elements" id="form-elements"></a>

You can place the following elements on the form from the [elements panel](forms.md#element-pane-operations).

* **Region** — contains all other form elements. You can drag other elements only onto the area. The form must have at least one region. There can be several areas on a form.
* **Tabs** — arrange form elements on several tabs.
* **Columns** — arrange elements in several columns.
* **Static text** — arbitrary text with HTML formatting.
* **Attribute field** — when you drag an attribute to the form layout, a field associated with the attribute is created. Field properties correspond to the associated attribute type.
* **Embedded form** — you can drag another form onto the form layout to embed it into the current form.
* **Button area** — provided for each form and each area. Buttons can be placed only in the button areas.
* **Button group** — combines buttons into a dropdown.
* **Button Separator** — visually separates buttons within button areas.

### Use the Elements Panel <a href="#element-pane-operations" id="element-pane-operations"></a>

Use the elements panel to:

* Drag and drop elements on the form layout.
* Search for elements.
* Filter element list by element type.
* Create and edit attributes, buttons, and forms.

#### Create an Attribute <a href="#creating-an-attribute" id="creating-an-attribute"></a>

1. In the elements panel:
   * Hover over the **Attributes** heading to create an attribute in the current template, or…
   * Hover over the template name in the element list to create an attribute in the corresponding template.
2. Click the **Add Attribute** button that appears.
3. The attribute creation window appears.

<figure><img src=".gitbook/assets/form_designer_create_attribute" alt="Creating an attribute using the form designer"><figcaption><p>Creating an attribute using the form designer</p></figcaption></figure>

#### Edit an Attribute, Button, or Form <a href="#editing-an-attribute-button-or-form" id="editing-an-attribute-button-or-form"></a>

1. Hover the mouse pointer over an attribute, button, or form name in the elements panel.
2. Click the **Edit Attribute**, **Edit Button**, or **Edit Form** button that appears.
3. The attribute properties window, the button designer, or the form designer appears.

<figure><img src=".gitbook/assets/form_designer_edit_form" alt="Editing a form using the form designer"><figcaption><p>Editing a form using the form designer</p></figcaption></figure>

#### Create a Button <a href="#creating-a-button" id="creating-a-button"></a>

1. In the elements panel, hover over the **Buttons** heading.
2. Click the **Add button** button that appears.
3. The [button designer](buttons/button-designer.md) appears.
4. Configure and save the button.

<figure><img src=".gitbook/assets/form_designer_create_button" alt="Creating a button in the form designer"><figcaption><p>Creating a button in the form designer</p></figcaption></figure>

### Clone the Form <a href="#cloning-a-form" id="cloning-a-form"></a>

1. Click **Clone**.
2. In the form cloning window, enter the form **name** and **system name**.
3. Click **Save**.
4. The new form opens in the form designer.

<figure><img src=".gitbook/assets/2023-07-16_16h52_06.png" alt="Form cloning"><figcaption><p>Form cloning</p></figcaption></figure>

### Edit the Form Rules <a href="#editing-the-form-rules" id="editing-the-form-rules"></a>

1. Click the selector button next to the form title in the designer.
2. Select **Form rules** from the dropdown.
3. The rule designer for the form is displayed.
4. Edit the form rules.
5. Click **Save**.

<figure><img src=".gitbook/assets/form_designer_goto_form_rules" alt="Form rules designer jump menu"><figcaption><p>Form rules designer jump menu</p></figcaption></figure>
