# What is this?

This Git repository exists to provide a schema for the CHAI Applied Model Card. The Applied Model Card is a document that provides a structured format for documenting the development, deployment, and monitoring of AI models in health use cases. 

# How do I use this?

The schema is provided as an XML Schema Definition. We provide an example of a model card instance document in XML format. 

All text fields in the Applied Model Card allow Markdown formatting. This can be used to style text and add links, images, and more. The schema also includes a "Bibliography" element; the contents of this element should be a string conforming to the BibTeX format. 

Applications that wish to produce Applied Model Cards as PDFs should include the following custom metadata in each PDF:
- **`chaiMcXml`**: The Applied Model Card instance document, serialized as an XML string.
- **`chaiMcSoftwareId`**: An arbitrary string describing the application producing the PDF; this is used to trace bugs in Applied Model Card production back to the bugs' sources.

Users of this schema, and of the Applied Model Card itself, should do so with the understanding this product is in draft form and is not yet finalized. As such, the Applied Model Card schema is subject to changes; such changes will be made in a non-breaking manner. The changelog for this project can be viewed at https://github.com/coalition-for-health-ai/mc-schema/releases.
