See example [Software Requirements Specification](https://krazytech.com/projects/sample-software-requirements-specificationsrs-report-airline-database) document for more detail.


### Purpose
The purpose of this document is to build a web page that lists jobs that our troops qualify for after completing the VetsWhoCode curriculum.


### Project Scope
The purpose of the jobs listing is to have a list of jobs accessible to our graduates. The jobs list will be created nightly at RemoteGig.io and made available via a json endpoint. This JSON endpoint will then be consumed and displayed by VetsWho.code.


### Technical Implementation

The fields from the endpoint are as follows:



*   url: string; this is the url of the job posting
*   title: string; title of the job
*   description: string; description of the job
*   company: string; company associated with the job listing
*   created_at: datetime; this is a Ruby on Rails convention and is the datetime the record was created in Rails
*   updated_at: datetime; this is a Ruby on Rails convention and is the datetime the record was updated in Rails. In this case the created_at and updated_at will most likely be identical
*   tag_list: array; this an array of keywords that appear in either the job title or description. You can [view the tag list here](https://github.com/marklocklear/remote_gig/blob/master/app/models/job.rb#L36) along with the logic to add tags in the add_tags method just belong the tag list (line 57)

You can see an example of job data at https://remotegig.io/jobs.json

### Design and Implementation

TBA


### System Features

TBA
