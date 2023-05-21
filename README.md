# UFSCar Multilingual Abstracts Dataset

This repository contains a dataset of academic abstracts from the Universidade Federal de São Carlos (UFSCar). The dataset includes abstracts in multiple languages, collected from various academic publications.

## Data

The dataset is provided in JSON format, with each JSON object representing an individual academic work. Each object includes metadata about the work and the text of the abstract in each available language.

## Repository Structure

Below is the basic structure of the repository:

ufsc_repositorio
│ README.md - this file.
│ LICENSE - the license file.
│
└───data
│ dissertations.details.json - JSON file containing details of dissertations.
│ theses_details.json - JSON file containing details of theses.

### Structure of the JSON files

Each JSON object includes the following fields:

- `ID`: A unique identifier for the academic work. This is taken from the last section of the original URL.

- `dc.identifier.uri`: The URL of the academic work's details page.

- `Num Languages`: The number of unique languages in which the abstract is available.

- `Languages`: A list of the languages in which the abstract is available.

- A dictionary for each available language, where the key is the language code (for example, `eng` for English or `por` for Portuguese). Each dictionary includes metadata about the academic work, as well as the text of the abstract. Possible fields in this dictionary include:
  - `dc.type`: The type of the academic work.
  - `dc.publisher`: The publisher of the academic work.
  - `dc.title`: The title of the academic work.
  - `dc.rights.uri`: Information about the rights associated with the academic work.
  - `dc.date.accessioned`: The date when the academic work was added to the repository.
  - `dc.date.available`: The date when the academic work became available in the repository.
  - `dc.date.issued`: The date when the academic work was issued.
  - `dc.identifier.uri`: The URL of the academic work's details page.
  - `dc.description.abstract`: The abstract of the academic work.

### Example

Here is an example JSON object from the dataset:

```json
{
    "ID": "11668",
    "dc.identifier.uri": "https://repositorio.ufscar.br/handle/ufscar/11668?show=full",
    "Num Languages": 2,
    "Languages": ["por", "eng"],
    "por": {
        "dc.description.resumo": ["..."],
        ...
    },
    "eng": {
        "dc.description.abstract": ["..."],
        ...
    }
}


*Note that the Portuguese Abstract in the field "dc.description.resumo" as for English just use "dc.description.abstract".


## UFSCar Repository: Comprehensive Overview and Documentation (!WIP!)
Repository Overview
The UFSCar repository is an institutional digital repository for the Federal University of São Carlos (Universidade Federal de São Carlos - UFSCar), located in Brazil. The purpose of this repository is to provide open access to a variety of academic and scholarly works produced by the university's faculty, researchers, and students.

Repository Structure
Todo

##Accessing the Repository (Source)
The UFSCar repository can be accessed at http://repositorio.ufscar.br/. There is no need for authentication for viewing or downloading the items as the repository is publicly accessible. The repository supports browsing by community, collection, title, author, and date, as well as keyword search.




## Overview
The UFSCar Repository follows the Dublin Core Metadata Initiative (DCMI) standard for metadata. This is a set of vocabulary terms that can be used to describe resources for the purposes of discovery. The elements can be used in a resource description record to provide core information about the resource.

In the case of UFSCar Repository, these resources are academic papers, dissertations, and theses submitted to the Universidade Federal de São Carlos (UFSCar).

## Elements of the Metadata (From Source)
The key elements of the metadata used by the UFSCar Repository are:

dc.contributor.author: The name of the author or authors of the document. It contains both the author's name and their ID or URI for identifying them.
dc.date.accessioned: The date the item was added to the repository.
dc.date.available: The date the item became publicly available in the repository.
dc.date.issued: The date the document was officially issued or published.
dc.identifier.citation: The correct citation for the document.
dc.identifier.uri: The unique resource identifier (URI) of the document, which usually points to its location in the repository.
dc.description.abstract: An abstract or summary of the document's content.
dc.description.sponsorship: Any sponsors or funding entities for the research.
dc.language.iso: The ISO 639 language code of the language in which the document was written.
dc.publisher: The entity responsible for making the document available, usually the university or institution.
dc.rights.uri: Information about the rights held in and over the resource.
dc.subject: The subject or keywords associated with the document.
dc.title: The title of the document.
dc.title.alternative: An alternative title for the document, usually in a different language.
dc.type: The type or nature of the document content.
dc.contributor.advisor1: The primary advisor or supervisor for the research.
dc.description.resumo: The abstract or summary of the document in another language.
dc.publisher.initials: The initials of the publisher.
dc.publisher.program: The academic program to which the document belongs.
dc.subject.cnpq: The subject classification according to the National Council for Scientific and Technological Development (CNPq) of Brazil.
dc.ufscar.embargo: Information about any access restrictions to the document.
dc.publisher.address: The address of the publisher.
dc.contributor.authorlattes: The Lattes Platform (Plataforma Lattes) ID of the author, a database of curricula, institutions and research groups in the areas of Science and Technology in Brazil.
Additional Resources

The repository also contains information about the files associated with the document, including their names, sizes, formats, and descriptions. This information helps users to understand what kind of content is included in the repository item and in what format it is available.


## License (*Repo): Apache License 2.0 (Data licenses on dc.rights.uri).


