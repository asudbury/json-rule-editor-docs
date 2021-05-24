## json-rule-editor

### Implementation of Json rules in application

**_Step1: Install json-rules-engine_**

1. Install json-rules-engine from [npm](https://www.npmjs.com/package/json-rules-engine)

   `npm install json-rules-engine`

**_Step2: Place the json rule file_**

1. Place the generated rule file (as generated in [previous section](https://asudbury.github.io/json-rule-editor/docs/create-rules.html)) in your `src/` directory

for ex: `src/rules/Employee-Salary.json`

**_Step3: Pass json rule and input into json-rules-engine library_**

1. Import json rules engine
2. Import json rule file
3. Pass the **decisions** property of json rule and input parameters into Json rule engine as mentioned below

for ex:

lets create the file called rule-validation.js under src/validation/

    import { Engine } from 'json-rules-engine';

    // employeesalary is the json rule generated from rule editor

    import employeesalary from '../rules/Employee-Salary.json';

    const processEngine = (inputs, decisions) => {

      // Pass the decisions into Engine constructor
      const engine = new Engine(decisions);

     // Pass the inputs here
      return engine.run(inputs)
        .then(results => {
          console.log(results.events);
          return results.events
        })
    };

    // Creating input parameter
    const inputs = { designation: 'Manager', experience: 14 };


    // Pass the decisions property from employeesalary rule object
    processEngine(inputs, employeesalary.decisions);

_Note:_

> Please refer the [json rules engine](https://github.com/CacheControl/json-rules-engine) site
> to understand the features and advanced concepts.

[Next section - Manage existing rule](https://asudbury.github.io/json-rule-editor/docs/manage-rules.html)

[Go back to previous page](https://asudbury.github.io/json-rule-editor/docs/create-rules.html)

[Go Home](https://asudbury.github.io/json-rule-editor/docs/)
