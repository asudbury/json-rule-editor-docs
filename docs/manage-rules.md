## json-rule-editor

### Updating existing rules:

To edit / view / validate the existing rule files, upload the ruleset directory, where you maintain the rule files like application src directory or anything else, or drag and drop the appropriate files into rule editor.

_Note:_

> There is no restrictions in place to limit the number of files to be imported.
> However, it wouldn’t allow you to import / create the duplicate rule name to avoid confusion. (File names are case sensitive)

We will take the same example _"Employee Salary"_ for this section, lets assume there is a ask from business to add another fact called _"employee type"_ (contractor or permanent) to decide the salary criteria. We will see below how to update the existing rules in such situation.

**_Step1: Upload existing rules_**

1. Launch [json rule editor](https://www.json-rule-editor.com) or install locally via git clone
2. Select the _‘Choose ruleset directory’_ to select directory or drag and drop the rule files.
3. Click **Upload** button

   ![upload](https://asudbury.github.io/json-rule-editor-docs/images/upload.png)

**_Step2: Add new fact_**

Go to Employee-Salary rule. If you have just only one rule file, its selected by default

1. Click **Add icon** at top right corner of tool bar.
2. Give new fact name and data type.

   ![add new fact](https://asudbury.github.io/json-rule-editor-docs/images/update-fact1.png)

3. Click **Add Facts** button

   ![add new fact](https://asudbury.github.io/json-rule-editor-docs/images/update-fact2.png)

**_Step3: Update the existing decisions with new fact_**

Go to Decisions tab

1. Click **View Conditions** of outcome you want to modify.
2. Click **edit icon** at top right corner of decision panel displayed.

   ![update decision](https://asudbury.github.io/json-rule-editor-docs/images/update-decisions1.png)

3. Select the top node in decision panel where you want to add additional fact. In this case, select **all** top node as highlighted in red circle

   ![update decision](https://asudbury.github.io/json-rule-editor-docs/images/update-decisions2.png)

4. Select Add facts menu in **"Step 2: Add / Remove facts"** and fill in the new fact value

   ![update decision](https://asudbury.github.io/json-rule-editor-docs/images/update-decisions3.png)

5. Click **Edit Rulecase** button

_Note:_

> If you want to edit existing fact value in decision, like, changing the experience fact from 10 to 11 or 12 years. you have to delete the particular fact by
> selecting the _node_ and Click **Remove** in **"Step 2: Add / Remove facts"**

**_Step4: Add new decision with new fact_**

We will add one more new decision to handle another employment type say **Contractor** with different salary outcome.

1. Click **Add icon** at right corner of tool bar.
2. Repeat the steps of creating new decisions as mentioned in the [Step 4: here](https://asudbury.github.io/json-rule-editor-docs/create-rules.html)
3. Add all three facts like designation, experience and type

   ![update decision](https://asudbury.github.io/json-rule-editor-docs/images/update-decisions4.png)

4. Specify the outcome value to this new decisions and Click 'Add Rulecase' button

   ![update decision](https://asudbury.github.io/json-rule-editor-docs/images/update-decisions5.png)

**_Step5: Validate decisions_**

Go to Validate tab

1. Specify the values against facts
2. Click validate button to verify new values are returning for employee type _'Contractor'_

   ![rule name](https://asudbury.github.io/json-rule-editor-docs/images/update-validate.png)

**_Step5: Generate rule sheet_**

Go to Generate tab

1. Click generate button if you are happy to proceed.

_Note:_

> Json rule file will be generated at your default browser download folder.

**Caution:**

> Please be careful when you remove / edit fact name under Facts tab in the existing rule file.
> The updated changes of facts wouldn't be reflected into the decision conditions.
> Also, it might impact the validation functionality as well as existing decisison functionalities.

[Next section - More examples in Decisions](https://asudbury.github.io/json-rule-editor-docs/decisions.html)

[Go back to previous page](https://asudbury.github.io/json-rule-editor-docs/implementation.html)

[Go Home](https://asudbury.github.io/json-rule-editor-docs/)
