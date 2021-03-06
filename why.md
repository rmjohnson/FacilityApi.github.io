# Why Facility?

**First things first:** Why would you use *any* API framework? What's the advantage of having a formal API definition?

## Why use an API definition?

An **API definition** provides a single canonical representation of your API. This is useful at every stage of development:

* **Designing:** Writing an API definition is a great way to work out your API design before you start writing code. Syntax checking minimizes typos, and the definition can be easily submitted for peer review.
* **Implementing:** Generate server code using your preferred web service framework so that your primary coding burden is the actual implementation. Generating data transfer objects and interfaces helps you avoid repeating yourself as you implement your API, especially when using strongly-typed languages.
* **Documenting:** Add comments to your API definition and generate attractive and continuously up-to-date documentation.
* **Consuming:** Generate client libraries in various programming languages, even languages you don't know, to maximize the usability of your API. At the same time, support for JSON over HTTP ensures that clients can use your API even without a client library.

## Why use Facility?

Other API frameworks already exist, most notably [OpenAPI](https://www.openapis.org/) (aka [Swagger](https://swagger.io/)).

Consider using Facility if our design goals line up with your expectations better than other frameworks:

* **Concise API specification.** A clear and concise specification is ideal for API designers, implementors, and consumers.
* **Comfortable file format.** The Facility Service Definition (FSD) file format uses a domain-specific language in an effort to make definitions easier to read and write, especially for developers comfortable with C-style languages.
* **Interoperability with other API platforms.** Service definitions can be imported from other API platforms such as [OpenAPI](https://openapis.org/specification), which allows developers to leverage Facility tools without having to adopt a different specification format. We can also export definitions for those platforms so that developers can leverage the tools supported by those platforms.
* **Keep it simple.** The FSD specification will be kept as simple as possible, even though that means that some APIs cannot be represented by it. Every new capability adds complexity to every tool that leverages an FSD, and a complex definition language can hinder the creation of new tools. Constraints can also free API designers from the paralysis of too many choices.
* **Multiple languages, platforms, and frameworks.** A Facility Service Definition can be used to generate code in various programming languages (C#, JavaScript, etc.) on various platforms (Windows, Linux, etc.) for use with various API frameworks (ASP.NET, Node, etc.).
* **Easy-to-write tooling.** The standard tools and libraries use C#, which can be used on Windows, Linux, and Mac. They work well with ASP.NET but can be used to generate code for any programming language, platform, or framework.
* **API documentation.** Tools can be used to generate accurate documentation from service definitions.
* **Don't repeat yourself.** As much as possible, the details of an API should not have to be entered more than once. By generating data, code, and documentation from an FSD, we minimize the amount of repetition needed.
* **Ongoing integration.** APIs change over time, so tools that permit ongoing integration of changes to an FSD are better than one-time scaffolding generators.
* **Semantic versioning.** Integration of non-breaking changes to the API should not result in breaking changes to clients or service implementations.
* **Various API methodologies.** Facility can be used to build RESTful services, RPC services, and everything in between.
* **JSON over HTTP.** Using JSON over HTTP makes it possible for existing libraries and tools to consume, implement, and monitor Facility APIs.
* **Flexible transport and encoding.** While optimized for JSON over HTTP, an FSD could be used with other encodings (e.g. Protocol Buffers) and transports (e.g. WebSockets), or even for simple in-process communication.

Still interested in Facility? Read about how to [get started](/start) or just start playing around with the [Facility Editor](/editor).
