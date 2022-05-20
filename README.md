<div about="#" typeof="owl:Ontology">

# An Interaction Design Ontology

  - Author  
    [<span property="foaf:name">Dorian
    Tay­lor</span>](http://doriantaylor.com/person/dorian-taylor#me)
  - Created  
    January 23, 2012
  - Updated  
    December 18, 2013
  - Namespace URI  
    <https://vocab.methodandstructure.com/interaction-design#>
  - Preferred Namespace Prefix  
    ixd

This vocabulary defines a number of concepts peculiar to interaction
design which are not accounted for by other vocabularies.

![](https://vocab.methodandstructure.com/interaction-design-classes)

The purpose of the interaction design ontology is to codify a model for
the set of artifacts and relationships between them that are used to
take a project from a pile of stakeholder requirements and user research
to a distinct set of interactions and interfaces to be designed.

The interaction design ontology unifies and extends the following
vocabularies:

  - [A Process Model
    Ontology](https://vocab.methodandstructure.com/process-model#)
  - [FOAF](http://xmlns.com/foaf/0.1/)
  - [The Bibliographic Ontology](http://purl.org/ontology/bibo/)
  - [DCMI Types](http://purl.org/dc/dcmitype/)

As with the other vocabularies on this site, the canonical
representation is the machine-readable data embedded into this
specification. It is also, however, available in
[RDF/XML](https://vocab.methodandstructure.com/1.rdf) and
[N3](https://vocab.methodandstructure.com/1.n3) formats.

</div>

## Classes

### Personas and Scenarios

The overarching purpose of the scenario and persona classes is to be
able to pick them out from larger pools of documents or representations
of agents. This way it's possible to mix real people and organizations
into scenarios with fake personas and still be able to tell them apart.

<div id="Persona" about="[ixd:Persona]" typeof="owl:Class">

#### Persona

A persona is a fictional agent for use in interaction design scenarios.

> ixd:Persona is a decorator class for instances of other foaf:Agent
> classes. Use this class in conjunction with something like foaf:Person
> or org:FormalOrganization to denote that it is fictional.

  - Subclass of:  
    [foaf:Agent](http://xmlns.com/foaf/0.1/Agent)

[Back to Top](https://vocab.methodandstructure.com/interaction-design#)

</div>

<div id="Scenario" about="[ixd:Scenario]" typeof="owl:Class">

#### Scenario

A scenario is a document that depicts the steps toward the achievement
of one or more user goals.

  - Subclass of:  
    [foaf:Document](http://xmlns.com/foaf/0.1/Document)

[Back to Top](https://vocab.methodandstructure.com/interaction-design#)

</div>

<div id="Vignette" about="[ixd:Vignette]" typeof="owl:Class">

#### Vignette

A vignette is a short part of a scenario that isolates one single
interaction.

  - Subclass of:  
    [bibo:DocumentPart](http://purl.org/ontology/bibo/DocumentPart)

[Back to Top](https://vocab.methodandstructure.com/interaction-design#)

</div>

<div id="Branch" about="[ixd:Branch]" typeof="owl:Class">

#### Branch

A branch represents a potential change in state in the scenario, such as
the user making a choice, or some exogenous event.

[Back to Top](https://vocab.methodandstructure.com/interaction-design#)

</div>

### Interactions and Interfaces

The purpose of a scenario is to distill out the interactions, so we can
further distill those interactions into interfaces, from which we can
extrapolate technical entailments, and finally, construct the result.

<div id="Interaction" about="[ixd:Interaction]" typeof="owl:Class">

#### Interaction

An interaction is a particular kind of event wherein an agent uses an
interface to change the state of a system.

  - Subclass of:  
    [pm:Action](https://vocab.methodandstructure.com/process-model#)

[Back to Top](https://vocab.methodandstructure.com/interaction-design#)

</div>

<div id="Interface" about="[ixd:Interface]" typeof="owl:Class">

#### Interface

An interface is some kind of artifact that mediates interactions.

> It is conceivable that ixd:Interface could be used to describe, in
> addition to software user interfaces: ABIs, APIs, file formats,
> protocols, natural languages, and physical interfaces that genuinely
> have to do with physics, like electrical plug/socket systems.

  - Subclass of:  
    [dctype:InteractiveResource](http://purl.org/dc/dcmitype/InteractiveResource)

[Back to Top](https://vocab.methodandstructure.com/interaction-design#)

</div>

## Properties

Ain't got none yet.

> Should we have ixd:material-context and ixd:incidental-context? A
> material context would be one that is necessary to complete an
> interaction, whereas an incidental context would be one that was
> chosen for the narrative continuity of the scenario. Furthermore,
> contexts like "at the office" or "using smartphone" could be reused in
> both material and incidental castings, even across different vignettes
> in the same scenario.

<div id="goal" about="[ixd:goal]" typeof="owl:ObjectProperty">

#### goal

Personas have objectives.

  - Domain:  
    [ixd:Persona](https://vocab.methodandstructure.com/interaction-design#Persona)

[Back to Top](https://vocab.methodandstructure.com/interaction-design#)

</div>
