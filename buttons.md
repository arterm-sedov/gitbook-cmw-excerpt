# Buttons

{% hint style="success" %}
**Definition**

A button is an element on a [form](forms.md) or table that performs a configured action on a click.
{% endhint %}

## Use the Template's Button List

The list of buttons is available for all template types.

1. Open a template.
2. Go to the **Buttons** tab.
3. The list of buttons in the template opens.
4. Perform the following operations:
   * **Open** — double-click a button row to [configure ](buttons.md#opening-the-button-designer)the existing button.
   * **Create** — [configure ](buttons.md#opening-the-button-designer)a new button.
   * **Delete** — select a checkbox in the first column for a button and click **Delete**. Confirm the button deletion.
   * **Search** — click <img src=".gitbook/assets/image (4).png" alt="" data-size="line"> and enter keywords in the **Search** field. The rows containing the keywords will appear.

<figure><img src=".gitbook/assets/button_list (1)" alt="Template button list"><figcaption><p>Template button list</p></figcaption></figure>

## Configure the Button <a href="#opening-the-button-designer" id="opening-the-button-designer"></a>

Use the button designer to configure its appearance, behavior, and operation.

1. Open the template's [button list](buttons.md#use-the-templates-button-list).
2. Click **Create** or double-click a button in the list.
3. The button designer appears.
4. Configure the button display and operation using the following tabs:
   * [**Properties**](buttons.md#properties)
   * [**Script**](buttons.md#script)
   * [**Display condition**](buttons.md#display-condition)
   * [**Local variables**](buttons.md#local-variables)
   * [**Relations**](buttons.md#relations)
5. **Save** the button.

![Button designer — Properties tab](.gitbook/assets/button\_designer)

### Configure Button Properties <a href="#properties" id="properties"></a>

On the **Properties** tab, configure the general button settings.

* **Display name** — a label for the button. After placing the button within a button area (on a form or a table), you can change its display name on that button area, this change will not affect the name of the original button in the template.
* **System name** — a unique name used to identify the button in scripts, expressions, and scenarios.
* **Description** — a relevant description of the button's purpose.
* **Operation context** — defines the available operations, the operation execution context, and the ability to use the button on the corresponding forms and tables:
  * **Record** in a record template, account template, role template, or organizational unit template.
  * **User task** on a process diagram.
  * **Process** — process template or process instance.
  * **Account** — a record in an account template.
  * **Diagram** — a process diagram.
* **Operation** — the available operation set depends on the selected **operation context**. The following operations are available:
  * **C# script** — execute C# code configured on the [**Script** tab](buttons.md#script).
  * **Start process** — launch a process instance from the current or a new record.
  * **Stop process** — stop the current process instance.
  * **Start process from linked template** — launch the process from a record template linked to the current template.
  * **Export record** — export the record using an export template.
  * **Export table** — export a table in XLSX format.
  * **Archive** — archive a record or process instance.
  * **Unarchive** — unarchive a record or process instance.
  * **Create** — create a record.
  * **Create related record** — create a record in the template linked to the current template.
  * **Save** — save the current record.
  * **Delete** — delete a record or process instance.
  * **Reopen** — assign **In progress** status to the task.
  * **Complete task** — complete the current process task.
  * **Defer** — this operation will be implemented in future product versions.
  * **Accept** — set the current account as the task assignee.
  * **Migrate** — upgrade the process instance to the latest process diagram version.
  * **Generate new token** — create a new token on the selected process instance diagram element.
  * **Link to a template** — link the account to the selected account template.
  * **Unlink from the template** — unlink the account from the selected account template.
  * **Trigger the “Button clicked” event** — the button click will trigger the **Button clicked** event, for example, to run a script in the application.
  * **Edit** — configure the process diagram.

{% hint style="info" %}
**Operations** are executed on **records** in the record, account, role, and organizational unit templates, as well as on **process instances** in the process templates.
{% endhint %}

* **Save the record after execution** — select this checkbox to save the current record upon the button **operation** execution.
* **Skip validation** — if you select this checkbox, data validation won't be performed when entering and saving record data, and validation errors won't appear.
* **Operation result** — select an action to perform upon the **operation** execution:
  * **Refresh data** — reload the record data.
  * **Navigation** — go to an object specified in the **Navigate to** field:
    * **Related record** — go to a record linked to the process instance.
    * **Process instance** — go to a process instance associated with the **operation context**.
    * **Started process task** — go to the current user task of the process instance.
    * **Next task in the list** — go to the next user task of the process instance.
    * **Previous page** — go to the current table's preceding page.
    * **Diagram** — go to the process instance diagram.
    * **Table** — go to a table listing template records or process instances.
  * **Download document** — save the file generated using an export template.
* **Set form access mode:**
  * **Read** — on the button click the form will become read-only.
  * **Edit** — after clicking the button the user will be able to enter data into the form (subject to the appropriate permissions).
  * **No change** — use the original form access mode.
* **Show the button** — use this dropdown along with the **Set form access mode** dropdown.
  * **In edit mode** — the button will appear only when data entry in the form is allowed.
  * **In read mode** — the button will appear only when the form is read-only.
  * **Always** — the button will appear both in data entry and read-only modes.
* **Show the dialog** — if you select this checkbox, clicking the button will open the operation confirmation dialogue you configure:
  * **Configure the dialog** — go to the operation confirmation form designer. The element panel in this designer shows the operation **local variables** that you can drag and drop on the dialogue.

![Operation dialogue designer with a local variable](.gitbook/assets/button\_designer\_dialogue\_designer)

### Configure Button Script <a href="#script" id="script"></a>

On the **Script** tab, you can enter a C# script to execute on the button click.

To generate a C# script template, click **Generate C# template**.

![Button designer — Script tab with a C# script template](<.gitbook/assets/button\_designer\_script (1)>)

### Configure Button Display Condition <a href="#display-condition" id="display-condition"></a>

On the **Display condition** tab, you can configure a formula or N3 expression. The button will be displayed if the formula or N3 expression returns `true`. Otherwise, the button will be hidden.

![Button Designer — Display condition tab with a formula](<.gitbook/assets/button\_designer\_display\_condition (1)>)

### Configure Button Local Variables <a href="#local-variables" id="local-variables"></a>

On the **Local variables** tab, you can create variables to use in a C# script or scenario executed on the button click.

Local variables are essentially the attributes.

For each variable, you can set:

* **Display name** — a relevant variable name.
* **Data type** — variables have the same types as attributes.
* **Display format** — variables have the same display formats as attributes.
* **System name** — a unique variable name to use in scripts, expressions, and scenarios.
* **Description** — a relevant variable's purpose description.
* **Template** — can be set for the following variable types: **Record**, **Account**, **Role**, and **Organizational unit**.
* **Store multiple values** — you can select this checkbox for the following variable types: **File** (same as attribute types **Document** and **Image**), **Record**, **Account**, **Role**, and **Organizational unit**.

![Button Designer - Local Variables Tab](.gitbook/assets/button\_designer\_local\_variables)

### View Button Relations <a href="#relations" id="relations"></a>

The **Relations** tab displays the list of all application objects and resources associated with the button.

![Button designer — Relations tab](.gitbook/assets/button\_designer\_relations)

