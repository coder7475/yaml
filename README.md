# YAML

**The topics covered**:

- Introduction

- Syntax

- Properties / Data Types

- yaml tools

## What is YAML?

**YAML ain't markup language**.

YAML is:

- Data format used to exchange data

- similar to file formats like like toml or ini

- Similar to XML & JSON

- These files contain text data arranged in a hierarchical structure

- Store only data, not commands

- Storing is called **Data Serialization**

So YAML is a data serialization language.

## Data Serialization

- YAML serializes objects to files and deserializes files to object

## Benefits

- Lightweight
- Simple & Easy to Read
- Friendly readable and writable
- Strict syntax - indentation is important
- Easily convertible to JSON, XML
- Suitable for configuration settings
- Used in most languages
- Parsing is easy
- Powerful when representing complex data
- Simple to modify with any text editor
- Many tools available

## Disadvantages

- It is a new format introduced recently, and a learning curve exists.
- Not much popular other than XML and JSON
- It is very complex to represent configuration in the hierarchy of data

## What is the file extension?

yaml files are created with the extension `.yaml` or `.yml`. You can use any IDE or text editor to open this file.

## What is the YAML media type?

Media or MIME types are present in request headers with `Content-Type` and `Accept` during data transfer between systems.

According to IANA , there is no official MIME type for YAML document content.

However, it can be represented using MIME types such as `text/yaml`, `text/x-yaml`, or `application/x-yaml`.

During the transfer of YAML data between a client and a server, implementation vendors include MIME type settings specified in requests and responses over the internet. The commonly used MIME format type for YAML is `text/yaml`.

Following is the mime type for these documents

```bash
content-type: text/yaml
```

or

```bash
accepts: text/yaml
```

The other possible options include:

- text/yaml
- text/yml
- text/x-yaml
- application/yaml
- application/yml

The choice among these options depends on the browser and the supported programming language. For instance, **Chrome** accepts `application/yaml`.

## References

- [Complete YAML course](https://www.youtube.com/watch?v=IA90BTozdow&list=PL9gnSGHSqcnoqBXdMwUTRod4Gi3eac2Ak&index=6)

- [Doc](https://www.w3schools.io/file/yaml-introduction/)

## Tools

- [YAML Lint](https://www.yamllint.com/)

- [YAML to JSON](https://onlineyamltools.com/convert-yaml-to-json)
