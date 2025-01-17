---
title: 'Defining an API Specification'
order: 81.3
page_id: 'defining_api_specification'
warning: false
contextual_links:
  - type: section
    name: "Prerequisites"
  - type: link
    name: "Grouping requests in Collections"
    url: "/docs/sending-requests/intro-to-collections/"
  - type: section
    name: "Additional Resources"
  - type: subtitle
    name: "Related Blog Posts"
  - type: link
    name: "Create APIs directly within the Postman app"
    url: "https://blog.postman.com/postman-7-1-create-apis-directly-within-the-postman-app/"
  - type: section
    name: "Next Steps"
  - type: link
    name: "Managing APIs"
    url: "/docs/designing-and-developing-your-api/managing-apis/"
---

You can define the structure of your API using its specification. You can also generate a collection from a spec.

* [Editing your schema](#editing-your-schema)
* [Generating a collection](#generating-a-collection)

> You can also [sync an API spec from a GitHub repository](/docs/integrations/available-integrations/github/#syncing-your-api-schemas-on-github).

## Editing your schema

The __Define__ tab in your API will include a specification (either one you imported or a sample Postman added when you created the API).

The default schema format is Open API 3.0, with YAML as the default language. To use a different schema type or language, choose it from the drop-down list.

The left pane of the schema editor displays an outline of your schema. When you first open the editor, the top level of nodes will be expanded, and the rest of them collapsed. Click nodes to expand or collapse them. Click an element in the outline to jump to it in the editor. You can also click the outline button to hide or show the outline.

![Schema navigation](https://assets.postman.com/postman-docs/v8-api-builder-schema-outline.gif)

In the schema editor, when you hover over a '#ref' component and press the Command key, a popover displays the first 200 characters of the reference component. When you Command-click the reference component, it will jump to the reference location.

![Schema refs](https://assets.postman.com/postman-docs/v8-api-builder-ref-jump.jpg)

In the upper right of the schema editor are options to beautify the content, wrap text, copy, and search. When you finish editing your schema, click **Save**.

![Save Schema](https://assets.postman.com/postman-docs/v8-wrap-text2-v2.jpg)

> Postman will indicate [validation errors](/docs/designing-and-developing-your-api/validating-elements-against-schema/) as you work on your schema.

## Generating a collection

The Postman API Builder supports API-first development by providing the option to create a Postman collection directly from a schema. Once you have a saved schema, you will see a **Generate Collection** option on the right-hand side of the tabs:

![Schema Editor Options](https://assets.postman.com/postman-docs/v8-generate-collection-button2-v2.jpg)

To create a collection based on your schema, click **Generate Collection**. You can add the collection as documentation, a test suite, an integration test, a monitor, a mock server, or a contract test. The collection will appear in __Collections__ in the left sidebar.

![Generate Collection](https://assets.postman.com/postman-docs/v8-generate-collection-modal2.jpg)

You can also configure how the collection should be generated by clicking **Show advanced settings**.
