# Tasks
> Describe the data the participant needs to map onto RDF and formulate the tasks accordingly. As we aim to assess the mapping language or tool, participants should be given some indication of the expected output. As such, we avoid participants being misled by the task descriptions.

> The example in this section assumes that participants will have to transform CSV and JSON files into RDF. However, one can easily replace those files with JSON, XML, or a relational database. This [folder](../assets/) contains the files used for this experiment.

You are provided with two CSV files ([employee.csv](../assets/employee.csv) and [project.csv](../assets/project.csv)) and one JSON file ([task.json](../assets/task.json)) containing data about employees, projects, and tasks. 

Your aim is to create mappings that transform this data into RDF triples according to the specifications below. The namespace of the vocabulary that we will use is `http://example.com/`s. This namespace is typically assigned to the namespace prefix ns in these tasks.

The following snippet informs the mapping processor which files to transform. You may copy/paste this into the tool or editor.

```turtle
@prefix ex: <http://example.com/> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
@prefix rml: <http://w3id.org/rml/> .

<#LS1>
    rml:referenceFormulation rml:CSV ;
    rml:source [ a rml:RelativePathSource ; rml:path "employee.csv" ; ]
.

<#LS2>
    rml:referenceFormulation rml:CSV ;
    rml:source [ a rml:RelativePathSource ; rml:path "project.csv" ; ]
.

<#LS3>
    rml:referenceFormulation rml:XPath ;
    rml:iterator "/tasks/task" ;
    rml:source [ a rml:RelativePathSource ; rml:path "task.xml" ; ]
.
```

## License information
<p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/chrdebru/kgc-user-study-protocol">The KGC Generation User Protocol</a> by <span property="cc:attributionName">Christophe Debruyne and Ademar Crotti Junior</span> is licensed under <a href="https://creativecommons.org/licenses/by-sa/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY-SA 4.0 <img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1" alt=""><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1" alt=""><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/sa.svg?ref=chooser-v1" alt=""></a></p>