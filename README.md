`.ewpmobility` Exchange File
============================

* [What is the status of this document?][statuses]
* [See the index of all other EWP Specifications][develhub]


Summary
-------

This document describes the `.ewpmobility` file format. This specialized file
format is intended for exchanging student mobility data, in a form strictly
compatible with EWP. `.ewpmobility` files might prove useful when moving
mobility data from one institution to another, i.e. when migrating to EWP
workflow.


Exporting
---------

`.ewpmobility` files are strictly compatible with Outgoing Mobility objects
used in EWP. Before you start exporting your data, you will be required to study
the structure of these objects.

 * Start be having a look at the [example.xml](example.xml) file.

 * Make sure you read [this introduction][mobility-workflow] to the EWP
   Mobility workflow.

 * Analyze the [structure of the Outgoing Mobility
   object](https://github.com/erasmus-without-paper/ewp-specs-api-omobilities/blob/stable-v3/response.xsd).
   You will need to understand its structure well and make sure your data is
   compatible with it. The `.ewpmobility` file is basically a wrapper for the
   Outgoing Mobility objects.

 * See [schema.xsd](schema.xsd) for the complete XML Schema of a valid
   `.ewpmobility` file. **Additional information can be found in XML Schema
   annotations.**

You SHOULD validate your file against the [schema](schema.xsd) before you send
it to your partner. We also recommend using the `.ewpmobility` file extension
(`.ewpmobility.gz` if compressed, etc.).


[develhub]: http://developers.erasmuswithoutpaper.eu/
[statuses]: https://github.com/erasmus-without-paper/ewp-specs-management#statuses
[registry-spec]: https://github.com/erasmus-without-paper/ewp-specs-api-registry
[discovery-api]: https://github.com/erasmus-without-paper/ewp-specs-api-discovery
[echo]: https://github.com/erasmus-without-paper/ewp-specs-api-echo
[error-handling]: https://github.com/erasmus-without-paper/ewp-specs-architecture#error-handling
[institutions-api]: https://github.com/erasmus-without-paper/ewp-specs-api-institutions
[mobility-workflow]: https://github.com/erasmus-without-paper/ewp-specs-mobility-flowcharts#common-workflow
