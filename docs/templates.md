Red Hat Developer Hub's Scaffolder, or "template engine" is one of its most powerful features. Templates help you quickly and consistently create new software components, services, documentation sites, or any other standard project types that your organization uses.

Think of Templates as pre-configured blueprints. Instead of manually setting up boilerplate code, configuration files, and repository structures every time you start something new, you can use a Template to generate the basic structure automatically.

---

## What is the Scaffolder?

The Scaffolder is the engine behind the Templates feature in RHDH. It takes a predefined template definition (which specifies things like input parameters, files to copy, and actions to run) and uses it to generate a new project based on your inputs.

From your perspective as an end-user, you interact with the Scaffolder through the RHDH UI by selecting a Template and filling out a form.

---

## Why Use Templates?

Using Templates in RHDH offers several key benefits:

- **Speed**: Go from idea to a basic working project structure in minutes, not hours.
- **Consistency**: Ensure new projects adhere to organizational standards, best practices, and required configurations from day one.
- **Reduced Boilerplate**: Avoid the tedious and error-prone process of copying and pasting code from existing projects.
- **Focus on Logic**: Spend less time on setup and more time on writing the unique logic for your new component or service.
- **Discoverability**: Easily find approved and recommended ways to start different types of projects within your organization.

---

## How to Use Templates

Using a Template in RHDH is a straightforward process:

**1. Navigate to the Create or Self-service Page**
In the RHDH catalog, look for a "Create" or "New Component" button or link, usually found in the main navigation or on the homepage. This will take you to the Scaffolder page.

**2. Browse the Available Templates**
The page will display a list of available Templates. These might be categorized (e.g., "Backend Services," "Frontend Applications," "Documentation Sites," "Libraries"). Browse or search to find the template that matches what you want to create.

**3. Select a Template to Use**
Click on the template you wish to use. You'll typically see a brief description of what the template generates.

**4. Fill Out the Form**
The Scaffolder will present you with a form. This form asks for specific information needed to customize the template, such as:

- The name of your new component/service.
- A description.
- The owner team or individual.
- Repository location (e.g., GitHub organization/group and repository name).
- Any specific configuration options relevant to that template (e.g., choice of language, framework options, database type).

Carefully fill in all the required fields.

**5. Review Your Choices and Create**
Before generating, you might get a summary of the information you provided. Review it to ensure everything is correct.

**6. Run the Scaffolder**
Click the "Create" or "Next" button to start the scaffolding process. RHDH will now use the template definition and your inputs to perform actions like:

- Creating a new repository in your chosen SCM (like GitHub, GitLab, Azure DevOps).
- Copying template files into the new repository.
- Replacing placeholder values in the files with your form inputs (e.g., inserting the component name into `package.json`).
- Registering the new component in the RHDH Catalog.
- Potentially running other custom actions (like setting up CI/CD pipelines, creating cloud resources, etc., depending on the template).

**7. Monitor Progress**
RHDH will show you the progress of the scaffolding process, listing the steps being executed.

**8. Access Your New Project**
Once the process is complete, you will typically be provided with links to:

- The new repository in your SCM.
- The newly registered component's page in the RHDH Catalog.

You can now clone the generated repository and start adding your unique application logic!


---

## Creating New Templates

Creating a new template involves following tasks:

1. Define the template structure and required parameters.
2. Implement the template logic in accordance with the Backstage framework guidelines.
3. Register the template with Red Hat Developer Hub.


---

## Additional Documentation

For more detailed instructions on writing templates and best practices, refer to the CBCF Backstage documentation:

- [Backstage Software Templates Guide](https://backstage.io/docs/features/software-templates/)
- [Best Practices for Templates](https://developers.redhat.com/articles/2025/03/17/10-tips-better-backstage-software-templates)


---

## In Summary

The Red Hat Developer Hub (RHDH) Scaffolder and its Templates feature are designed to make your life easier by automating the initial setup of standard project types. By leveraging Templates, you save time, ensure consistency, and can focus on building the core value of your new component or service.

Explore the available templates in RHDH and see how they can accelerate your development workflow.