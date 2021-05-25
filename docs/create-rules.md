## json-rule-editor

### Create Decisions

Primarily, we are going to deal with two factors 1) Facts and 2) Decisions across this tool.

**_Facts_**

Its an entity or attribute helps to build your business decisions. It supports four data types such as number, string, array and object - inline with json rules engine.

**_Decisions_**

It is actually business rule conditions which contains the possible facts values and associated outcome type. You can define any number of business decision outcomes under single rule file.

_Note:_

> Its good practise to separate your business rules into different files based on the use cases.

Lets see the step by step process starting from creating facts to generating the ruleset file.

**_Step1: Create new ruleset file_**

1. Launch [json rule editor](https://www.json-rule-editor.com) or install locally via git clone
2. Click **Create button** (Note: Upload functioanlity is explained in next section)

   ![create new rule](https://asudbury.github.io/json-rule-editor-docs/images/create-upload.png)

**_Step2: Specify rule name_**

1. Specify rule name and click **Create button**

   ![rule name](https://asudbury.github.io/json-rule-editor-docs/images/create.png)

**_Step3: Add new fact_**

1. Click **Create Facts** button at information message panel

   ![rule name](https://asudbury.github.io/json-rule-editor-docs/images/fact1.png)

2. Give fact name and data type such as string, number or array

   ![rule name](https://asudbury.github.io/json-rule-editor-docs/images/fact2.png)

3. Add as many as fact you need to build your decisions

   ![rule name](https://asudbury.github.io/json-rule-editor-docs/images/fact3.png)

**_Step4: Add new decisions_**

Go to Decisions tab

1. Click **Create Decision** button at information message panel

   ![rule name](https://asudbury.github.io/json-rule-editor-docs/images/decision1.png)

2. Select all / any in **"Step 1: Add Toplevel"**

   ![rule name](https://asudbury.github.io/json-rule-editor-docs/images/decision2.png)

3. Select Add facts menu in **"Step 2: Add / Remove facts"**

4. Select the fact, operator and value

   ![rule name](https://asudbury.github.io/json-rule-editor-docs/images/decision3.png)

5. Add necessary facts and you will see something as below

   ![rule name](https://asudbury.github.io/json-rule-editor-docs/images/decision4.png)

6. Select the Add Outcome in **"Step 3: Add outcome""** and specify the type value.

   ![rule name](https://asudbury.github.io/json-rule-editor-docs/images/decision5.png)

7. Click **Add Rulecase** button.

   ![rule name](https://asudbury.github.io/json-rule-editor-docs/images/decision6.png)

**_Step5: Validate decisions_**

Go to Validate tab

1. Specify the values against facts
2. Click Validate Ruleset button

   ![rule name](https://asudbury.github.io/json-rule-editor-docs/images/validate.png)

_Note: Please keep in mind when adding facts and value_

> Incase expected values are not getting displayed, go to Decisions tab and cross check the values.
> Values are case sensitive and perform strict equality comparison ( === ).

**_Step5: Generate rule sheet_**

Go to Generate tab

1. Click generate button if all required decisions are added.

   ![rule name](https://asudbury.github.io/json-rule-editor-docs/images/generate.png)

_Note:_

> Json rule file will be generated at your default browser download folder.

[Next section - Implementation of Json rules in application](https://asudbury.github.io/json-rule-editor-docs/implementation.html)

[Go back to previous page](https://asudbury.github.io/json-rule-editor-docs/rule-engine.html)

[Go Home](https://asudbury.github.io/json-rule-editor-docs/)
