# Configuring a Form

Use the form designer to configure the form layout, properties, and elements.

### Opening the Form Designer <a href="#opening-the-form-designer" id="opening-the-form-designer"></a>

1. Open the template [form list](viewing-the-template-form-list.md).
2. Double-click a form row.
3. The form designer appears.
4. Configure the form.

<figure><img src="../.gitbook/assets/form_designer" alt="Form designer"><figcaption><p>Form designer</p></figcaption></figure>

### Form Designer Elements <a href="#form-designer-elements" id="form-designer-elements"></a>

1. Element panel — a palette of elements to drag onto the form: attributes and visual elements. See [Element Panel Operations](form-designer.md#element-pane-operations). Use this panel to:
   * Drag and drop elements on the form layout.
   * Search for elements.
   * Filter element list by element type.
   * Create and edit attributes, buttons, and forms.
2. Form layout sets the form's visual appearance.
3. Properties panel — view and configure the properties of the selected element.
4. Buttons:
   * **Save** — save the form.
   * **Clear** — remove all elements from the form layout.
   * **Clone** — create a form duplicate.
   * **Configure template** <i class="fa-light fa-gear"></i> — go to the template **Properties** page.
   * **Relations** <i class="fa-brands fa-connectdevelop"></i> — view a list of application objects that use the form.

### Form Properties <a href="#form-properties" id="form-properties"></a>

1. **Display name** — the form name that will be displayed in its header when viewing template records.
2. **System name** — a unique form name, for use in scripts, expressions, and scenarios.
3. **Is default** — check this box to display this form by default when viewing template records.
4. **Type**:
   * **Public** — select this type for the form to be viewed using the form selection dropdown next to the form title.
   * **Internal** — select this type for the form to be displayed only if it is embedded in another form or is set as a record form (eg. for process start, record creation, dialogues).

### Form Elements <a href="#form-elements" id="form-elements"></a>

You can place the following elements on the form.

* **Region** — contains all other form elements. You can drag other elements only onto the area. The form must have at least one region. There can be several areas on a form.
* **Tabs** — arrange form elements on several tabs.
* **Columns** — arrange elements in several columns.
* **Static text** — arbitrary text with HTML formatting.
* **Attribute field** — when you drag an attribute to the form layout, a field associated with the attribute is created. Field properties correspond to the associated attribute type.
* **Embedded form** — you can drag another form onto the form layout to embed it into the current form.
* **Button area** — provided for each form and each area. Buttons can be placed only in the button areas.
* **Button group** — combines buttons into a dropdown.
* **Button Separator** — visually separates buttons within button areas.

### Editing the Form <a href="#editing-the-form" id="editing-the-form"></a>

1. Drag the required elements from the elements panel to the form layout.
2. To set the form properties, click an empty layout area and configure the properties using the properties panel.
3. To set the properties of a form element, select it in the layout and configure the properties in the properties panel.
4. Click **Save**.

### Editing the Form Rules <a href="#editing-the-form-rules" id="editing-the-form-rules"></a>

1. Click the selector button next to the form title in the designer.
2. Select **Form Rules** from the dropdown.
3. The rule builder for the form is displayed.
4. Edit the form rules.
5. Click **Save**.

<figure><img src="../.gitbook/assets/form_designer_goto_form_rules" alt="Form rules designer jump menu"><figcaption><p>Form rules designer jump menu</p></figcaption></figure>

### Element Pane Operations <a href="#element-pane-operations" id="element-pane-operations"></a>

#### Creating an Attribute <a href="#creating-an-attribute" id="creating-an-attribute"></a>

1. In the element pane:
   * Hover over the **Attributes** heading to create an attribute in the current template, or…
   * Hover over the template name in the element list to create an attribute in the corresponding template.
2. Click the **Add Attribute** button that appears.
3. The attribute creation window appears.

<figure><img src="../.gitbook/assets/form_designer_create_attribute" alt="Creating an attribute using the form designer"><figcaption><p>Creating an attribute using the form designer</p></figcaption></figure>

#### Editing an Attribute, Button, or Form <a href="#editing-an-attribute-button-or-form" id="editing-an-attribute-button-or-form"></a>

1. Hover the mouse pointer over an attribute, button, or form name in the elements panel.
2. Click **Edit Attribute**, **Edit Button**, or **Edit Form** button that appears.
3. The attribute properties window, the button designer, or the form designer appears.

<figure><img src="../.gitbook/assets/form_designer_edit_form" alt="Editing a form using the form designer"><figcaption><p>Editing a form using the form designer</p></figcaption></figure>

#### Creating a Button <a href="#creating-a-button" id="creating-a-button"></a>

1. In the element pane, hover over the **Buttons** heading.
2. Click the **Add button** button that appears.
3. The [button designer](../buttons/button-designer.md) appears.
4. Configure and save the button.

<figure><img src="../.gitbook/assets/form_designer_create_button" alt="Creating a button in the form designer"><figcaption><p>Creating a button in the form designer</p></figcaption></figure>

### Cloning a Form <a href="#cloning-a-form" id="cloning-a-form"></a>

1. Click **Clone**.
2. In the form cloning window, enter the form **name** and **system name**.
3. Click **Save**.
4. The new form opens in the form designer.

<figure><img src="../.gitbook/assets/form_designer_clone_form" alt="Form cloning"><figcaption><p>Form cloning</p></figcaption></figure>

### Related Articles <a href="#related-articles" id="related-articles"></a>

[**Viewing the Template Form List**](viewing-the-template-form-list.md)

[**Creating a Form**](creating-a-form.md)

[**Configuring a Buton**](../buttons/button-designer.md)
