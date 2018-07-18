# Tufts MIRA Metadata Application Profile
| UI Label | Attribute Name | Predicate | Type | Cardinality | Defintion |
| ------ | ------ | ------ | ------ | ------ | ------ |
| Abstract | abstract | ::RDF::Vocab::DC.abstract | string | multiple |A refinement of the description element, this element is used as a brief summary of the resource. For Tisch created content, this is mapped from the following: the **MARC 520** field, the Proquest **DISS_abstract element**, the Springer **AbstractSection[@ID]/Heading**element, and the first string in the **Description** column for an Excel based ingest.|
| Admin Set | *n/a* | ::Tufts::Vocab::Terms.admin_set_member | URI | **singular** |
| Accrual Policy | accrual_policy | ::RDF::Vocab::DC.accrualPolicy | string | **singluar** |
| Alternative Title | alternative_title | ::RDF::Vocab::DC.alternative | string | multiple |An alternative name for the resource. For Tisch created content this is mapped from the following: all **MARC 246** elements, and the Excel **Alternative_Title** heading.|
| Audience | audience | ::RDF::Vocab::DC.audience | string | **singluar** |
| Bibliographic Citation | bibliographic_citation | ::RDF::Vocab::DC.bibliographicCitation | string | multiple |The recommended property to describe the bibliographic citation information for a resource within its own metadata. This is an element refinement of dc:identifier, defined in the 'dcterms' namespace. The value of this property would hold details of the bibliographic item that contains the resource along with the position of the resource within it. Thus for a journal article it could capture the journal title, volume and issue numbers, pagination and publication date, or for a book chapter the book details and pagination. Other details of the resource, such as its title and creators, will be described using the usual Dublin Core properties. Optionally, but redundantly, these details may be included in the citation as well.  For more informatition see the [Dublin Core citation guidelines](http://dublincore.org/documents/dc-citation-guidelines/). Tisch creates this element for Excel based ingests via the **Bibliographic_Citation** column.|
| Contributor | contributor | ::RDF::Vocab::DC11.contributor | string | multiple |An entity responsible for making contributions to the resource. Examples of a Contributor include a person, an organization, or a service. |
| Corporate Name | corporate_name | ::RDF::Vocab::MADS.CorporateName | string | multiple |A corporate name used as a subject access point.  It is a Tufts loccally typed field that maps most closely to the **MARC 610** field. For Tisch created content it is mapped from all MARC 610 fields, and the **CorpName** column in Excel based ingests.  As local practice Tufts University also uses it to establish departments for theses and disertations.  As such, it is mapped from the Proquest **//DISS_inst_contact[1]** to a controlled vocabulary.|. 
| Created By | created_by | ::Tufts::Vocab::Terms.createdby | string | multiple |
| Creator | creator | ::RDF::Vocab::DC11.creator | string | multiple |
| Creator department | creator_dept | ::Tufts::Vocab::Terms.creatordept | string | multiple |
| Date Accepted | date_accepted | ::RDF::Vocab::DC.dateAccepted | string | multiple |
| Date Available | date_available | ::RDF::Vocab::DC.available | string | multiple |
| Date Copyrighted | date_copyrighted | ::RDF::Vocab::DC.dateCopyrighted | string | multiple |
| Date Created | date_created | ::RDF::Vocab::DC.created | string | multiple |
| Date Issued | date_issued | ::RDF::Vocab::EBUCore.dateIssued | string | multiple |
| Depositor | depositor | ::RDF::Vocab::relators.dpt | string | **singular** |
| Description | description | ::RDF::Vocab::DC11.description | string | multiple |
| Displays In | displays_in | ::Tufts::Vocab::Terms.displays_in | [controlled](../config/authorities/displays.yml) | multiple |
| Embargo Note | embargo_note | ::RDF::Vocab:: premis.TermOfRestriction | string | **singluar** |
| End Date | end_date | ::RDF::Vocab::PREMIS.hasEndDate | string | **singluar** |
| Extent | extent | ::RDF::Vocab::DC.extent | string | **singluar** |
| Format | format_label | ::RDF::Vocab::PREMIS.hasFormatName | string | multiple |
| Funder | funder | ::RDF::Vocab::relators.fnd | string | multiple |
| Genre | genre | ::RDF::Vocab::MADS.GenreForm | string | multiple |
| Has Format | has_format | ::RDF::Vocab::DC::hasFormat | string | multiple |
| Has Part | has_part | ::RDF::Vocab::DC::hasPart | string | multiple |
| Held By | held_by | ::RDF::Vocab::Bibframe.heldBy | string | multiple |
| Ingested<sup>[1](#system-dates)</sup> | date_uploaded | ::RDF::Vocab::DC.dateSubmitted | dateTime | multiple |
| Internal Note | internal_note | ::Tufts::Vocab::Terms.internal_note | string | **singluar** |
| Is Format Of | is_format_of | ::RDF::Vocab::DC::isFormatOf | string | multiple |
| Is Part Of | is_part_of | ::RDF::Vocab::DC::isPartOf | string | multiple |
| Is Replaced By | is_replaced_by | ::RDF::Vocab::DC.isReplacedBy | string | multiple |
| Language | language | ::RDF::Vocab::DC11.language | string | multiple |
| Legacy PID | legacy_pid | ::Tufts::Vocab::Terms.legacy_pid | string | **singluar** |
| License | license | ::RDF::Vocab::DC.rights| string | multiple |
| Modified<sup>[1](#system-dates)</sup> | date_modified | ::RDF::Vocab::DC.modified | dateTime | multiple |
| Permanent URL | identifier | ::RDF::Vocab::DC.identifier | string | singluar |
| Personal Name | personal_name | ::RDF::Vocab::MADS.PersonalName | string | multiple |
| Primary Date | primary_date | ::RDF::Vocab::DC11.date | string | multiple |
| Provenance | provenance | ::RDF::Vocab::DC.provenance | string | multiple |
| Publisher | publisher | ::RDF::Vocab::DC11.publisher | string | multiple |
| QR Note | qr_note | ::Tufts::Vocab::Terms.qr_note | string | multiple |
| QR Rejection Reason | rejection_reason | ::Tufts::Vocab::Terms.rejection_reason | string | multiple |
| QR Status | qr_status | ::Tufts::Vocab::Terms.qr_status | string | multiple |
| Replaces | replaces | ::RDF::Vocab::DC.replaces | string | multiple |
| Retention Period | retention_period | ::Tufts::Vocab::Terms.retention_period | string | multiple |
| Rights | rights_statement | ::RDF::Vocab::EDM.rights | [controlled](../config/authorities/rights_statements.yml) | **singluar** |
| Rights Holder | rights_holder | ::RDF::Vocab::DC.rightsHolder | string | multiple |
| Rights Note | rights_note | ::RDF::Vocab::DC11.rights | string | **singular** |
| Source | source | ::RDF::Vocab::DC.source | string | multiple |
| Spatial | geographic_name | ::RDF::Vocab::DC.spatial | string | multiple |
| Start Date | admin_start_date | ::Tufts::Vocab::Terms.start_date | string | multiple |
| Steward | steward | ::Tufts::Vocab::Terms.steward | string | **singluar** |
| Subject | subject | ::RDF::Vocab::DC11.subject | string | multiple |
| Table of Contents | table_of_contents | ::RDF::Vocab::DC.tableOfContents | string | multiple |
| Temporal | temporal | ::RDF::Vocab::DC.temporal | string | multiple |
| Title | title | ::RDF::Vocab::DC.title | string | **singluar** |
| Tufts License | tufts_license | ::RDF::Vocab::DC.license | string | **singluar** |
| Type | resource_type | ::RDF::Vocab::DC.type | [controlled](../config/authorities/resource_types.yml) | **singular** |
| Visiblity | *n/a* | Uses Hydra Access Controls | [controlled](https://github.com/curationexperts/epigaea/wiki/MIRA-XML-Import-Export-Format#valid-values-for-metadata-fields) | *n/a*  |

## System Dates
`Ingested` and `Modified` are both managed by the application and cannot be directly modified via the UI 
or importers.  `Ingested` represents the date that the work was initially created in the repository. 
`Modified` reflects the date the work was last updated via the UI or system process (import, template update, etc.).