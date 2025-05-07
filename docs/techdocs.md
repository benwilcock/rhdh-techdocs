TechDocs is a documentation feature integrated into the Red Hat Developer Hub. It allows developers to create, manage, and view technical documentation directly within the developer portal. By centralizing documentation, TechDocs ensures that teams have easy access to up-to-date information, improving collaboration and reducing time spent searching for resources.

![A TechDocs List in RHDH](./images/rhdh-techdocs.jpg){ width="850" }

## Why Use TechDocs?

* **Centralized Documentation**: All your technical documentation in one place.
* **Improved Collaboration**: Teams can easily share and update documentation.
* **Streamlined Onboarding**: New developers can quickly access the information they need.
* **Version Control**: Documentation is tied to your codebase, ensuring consistency.

## Finding TechDocs in the Application

To access TechDocs (using the left hand navigation):

1. Click on the "Docs" button in the left hand navigation
1. The default view is to show only documents owned by you
1. To expand the list click "All" under "My Org"
1. To filter the view, use the "Owner" and "Tags" filters
1. Click on the TechDoc you'd like to view. It will open in the main window.

To access TechDocs (using search):

1. Use the search bar and enter a search term.
1. If there are lots of results click "View full results ->" and then click "Documentation" in the Results type section.
1. If the search was successful, documents matching your query will be listed.

## Writing Your Own TechDocs

Follow these steps to create and integrate your TechDocs:

### 1. Create a Documentation File

Write your documentation using Markdown syntax. Save the file in your repository, typically under a `<root>/docs/index.md` name if this is your first TechDoc in a set. For example:

```markdown
# My Application Documentation

## Overview
This application does X, Y, and Z.

## Getting Started
1. Clone the repository.
2. Install dependencies.
3. Run the application.

## API Reference
- Endpoint: `/api/v1/resource`
- Method: `GET`
```

### 2. Create an `mkdocs.yaml` File

To structure your TechDocs, create an `mkdocs.yaml` file in the root of your repository. This file defines the configuration for your documentation site. For example:

```yaml
site_name: "My Application"
docs_dir: docs
nav:
  - "About My Application": index.md
```

Ensure that the `nav` section matches the preferred structure of your documentation site.

### 3. Update Your `catalog-info.yaml`

Add the following section to your `catalog-info.yaml` file to link your TechDocs:

```yaml
metadata:
    name: my-application
    description: Documentation for My Application
spec:
    type: service
    owner: team-name
    lifecycle: production
    links:
        - url: ./docs
```

### 3. Verify and Publish

1. Push your changes to the repository.
1. Ensure your service is registered in the Red Hat Developer Hub (see the [Adding An Entry To The Software Catalog](catalogs.md#adding-an-entry-to-the-software-catalog)).
1. Navigate to the component in the portal and verify that the "Docs" tab displays your TechDocs.

## Additional Tips

* **Keep It Simple**: Write clear and concise documentation.
* **Use Headings**: Organize content with headings for better readability.
* **Update Regularly**: Keep your documentation in sync with your codebase.
* **Leverage Markdown Features**: Use lists, tables, and links to enhance your documentation.
* **Add Some Flair!**: Use the [TechDocs extensions](extensions.md) to add a little sparkle to your documentation.

By following this guide, you can ensure that your TechDocs are well-integrated and provide value to your team.

