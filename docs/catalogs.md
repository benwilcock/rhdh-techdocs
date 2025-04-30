The Software Catalog is a central place where developers can discover, explore, and understand all the software components, systems, and other assets that are available within your organization. Think of it as a comprehensive inventory of services, libraries, websites, coding projects, documentation, and more.

By using the software catalog, you can:

* Find existing software components you need to use or integrate with.
* Understand who owns a component and how to contact them.
* See the dependencies or technology stack used by a component.
* Quickly access documentation, APIs, and other relevant resources.
* Visualize relationships between components.

This guide will walk you through how to effectively use the Software Catalog.

---

## Accessing the Software Catalog

You can access the Software Catalog by clicking on the **Catalog** link in the main navigation menu of Red Hat Developer Hub.

---

## Navigating the Catalog

Upon landing on the Catalog page, you will see a list of registered software components.

### List View
Components are typically displayed in a list format, showing key information like name, type, and ownership.

### Filtering and Sorting
Use the available filters on the side or top of the page to narrow down the list based on criteria such as:

* Kind (e.g., Component, System, etc.)
* Type (e.g., document, model, database, file, etc.)
* Owner
* Tags

You can also sort the list by clicking the different columns.

### Search Bar
Use the search bar to quickly find components by name or description.

---

## Viewing Component Details

Clicking on a component in the list will take you to its detailed overview page. This page provides a wealth of information about the selected component, typically organized into different tabs or sections depending on your platform's plugins:

* **Overview**: A summary of the component, including its description, lifecycle status, and links to source code repositories.
* **API**: Details about any registered APIs provided or consumed by this component, including links to OpenAPI specifications or other API documentation.
* **Docs**: Links to technical documentation related to the component, often pulled directly from source code repositories (using TechDocs).
* **Dependencies**: A view showing components that this component depends on, and components that depend on this one.
* **Links**: Additional information about the component that can be found online etc.
* **Ownership**: Clearly states the team or individual responsible for maintaining the component.
* **Activity**: Recent activity related to the component, such as CI/CD build status or recent commits.

Explore the different sections on the component detail page to get a complete picture of its purpose, status, and related resources.

---

## Searching and Filtering

The search and filter capabilities are powerful tools for finding exactly what you need:

### Searching
Type keywords into the main search bar on the Catalog page. The search is usually performed across component names, descriptions, and potentially other metadata.

### Filtering
Use the filter options on the left-hand side. You can apply multiple filters simultaneously to refine your results. For example, you could filter to see only **Services** owned by the **Frontend Team**.

---

## Understanding Component Status and Metadata

Pay attention to the metadata associated with each component, as it provides important context:

* **Kind & Type**: Indicates what kind and type of software component it is (e.g., Service, Library, Website, Documentation, Users, etc.).
* **Owner**: The designated team or individual responsible for the component. This is crucial for knowing who to contact with questions or issues. (Note: Users and Groups are also software catalog items)
* **Lifecycle**: Shows the current stage of the component (e.g., Production, Experimental).
* **Tags**: Keywords or labels applied to the component for categorization and easier discovery.
* **Links**: Quick links to external resources like source code repositories, websites, etc.

---

## Adding an Entry to the Software Catalog

To add a new entry to the Software Catalog, you need to create a `catalog-info.yaml` file and register it with Red Hat Developer Hub. This file serves as the metadata descriptor for your software component.

### Steps to Create and Register a `catalog-info.yaml` File

1. **Create the `catalog-info.yaml` File**  
    In the root directory of your software project, create a file named `catalog-info.yaml` with the following structure: The file should include the `apiVersion`, which specifies the version of the Backstage API; the `kind`, which defines the type of entity such as `Component`, `System`, or `API`; the `metadata` section, which contains basic information like the name, description, and tags; and the `spec` section which provides details such as the type of component, ownership, and lifecycle stage. Below is a simplified example:

    ```yaml
    apiVersion: backstage.io/v1alpha1
    kind: Component
    metadata:
        name: my-software-component
        description: A brief description of your software component.
        tags:
             - example
             - service
        annotations:
             github.com/project-slug: my-org/my-repo
    spec:
        type: service
        owner: team-name
        lifecycle: production
    ```

2. **Push the File to Your Repository**  
    Commit and push the `catalog-info.yaml` file to the root of your project's source code repository.

3. **Register the File in Red Hat Developer Hub**  

    - Navigate to the **Create** or **Self-service** page in Red Hat Developer Hub.
    - Click on the **Register Existing Component** button.
    - Provide the URL to the `catalog-info.yaml` file in your repository (e.g., a GitHub URL).
    - Follow the prompts to complete the registration process.

4. **Verify the Registration**  
    Once registered, your software component will appear in the Software Catalog. You can view its details and ensure all metadata is accurate.

By following these steps, you can ensure your software component is discoverable and well-documented within your organization.

---

## In Summary
By leveraging the Software Catalog, you can efficiently navigate the landscape of your organization's software, find the components you need, and understand their context and ownership.

If you have questions about a specific component, the owner listed in the catalog is the best point of contact. For general questions about the Software Catalog itself, please refer to your internal Developer Hub documentation or support channels.