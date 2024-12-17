# KG Generation User Study
Knowledge graph generation from (semi-)structured data is challenging, and facilitating user evolvement is an issue frequently brought up within this community. We cannot deny the progress we have made with respect to (declarative) knowledge generation languages and tools to help build such mappings. However, it is surprising that no two studies report on similar protocols. This heterogeneity does not allow for the comparison of knowledge graph generation languages, techniques, and tools. This paper first analyses the various studies that report on studies involving users to identify the points of comparison. These gaps include inconsistencies in task design, participant selection, and evaluation metrics. We then use these to propose and introduce a protocol designed to address this challenge. Where possible, we draw and take elements from the literature we deem fit for such a protocol. The protocol, as such, allows for the comparison of languages and techniques for the RDF Mapping Language's core functionality, which is covered by most of the other state-of-the-art techniques and tools. We also propose how the protocol can be amended to compare extensions (of RML). This protocol provides an important step towards a more comparable evaluation of knowledge graph generation user studies. 

This repository is constructed as follows:

* The `assets` directory contains the CSV and JSON files for the tasks used in the protocol.
* The `pre-questionnaire` directory contains the self-assessment form.
* The `post-questionnaire` directory contains the questionnaires on mental workload and usability.
* The `tasks` directory contains the description of the tasks.
* [`Protocol.md`](./Protocol.md) contains the base protocol.

## Variants

This protocol can be used for comparing different KGC languages and tools.

* When comparing languages, techniques, or tools. One can provide the same tasks to two different groups. One can compare different mapping languages (e.g., ShExML vs. RML), compare editors vs. "bare bones"  languages (e.g., RMLEditor vs. RML executed from a terminal), compare languages and abstractions of languages (e.g., RML vs. YARRRML), and even different editors and languages.

* When the aim is to compare support for an advanced KGC requirement such as named graphs, collections and containers, or RDF* (among others), then one can take this protocol as is for one group, and only change the last two tasks for the second in which those requirements are covered, with the first three tasks giving a comparable baseline, unless the extension covered another aspect such as storing the resulting trip.

* When the aim is to such compare support across languages, techniques, or tools, then the protocol must be amended for both. Again, the first three tasks must remain unchanged as to ensure some comparative baseline with literature. This approach can be used to compare the languages and tools for more advanced KGC requirements such as named graphs, RDF collections and containers, and function calls, among others. 

Participants are assumed to have access to prepared "resources" or "environments" to focus on the tasks. In the case of RML, for instance, the logical sources would be provided in the tool or for them to copy and paste. This allows researchers to assess the languages and tools with respect to these aspects by giving one group the prepared artifacts and requesting the other to formulate the logical sources themselves. We deem this a special case of comparing a baseline with an extension as described above, but where the five tasks remain unchanged.

# License Information

<p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/chrdebru/kgc-user-study-protocol">The KGC Generation User Protocol</a> by <span property="cc:attributionName">Christophe Debruyne and Ademar Crotti Junior</span> is licensed under <a href="https://creativecommons.org/licenses/by-sa/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY-SA 4.0 <img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1" alt=""><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1" alt=""><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/sa.svg?ref=chooser-v1" alt=""></a></p>