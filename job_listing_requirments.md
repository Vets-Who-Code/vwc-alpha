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

Below is an example of a single element


```
[

```



1. `{`
    1. **<code>url: "[https://stackoverflow.com/jobs/163127/remote-sr-android-java-engineer-amazon-firetv-surge?a=SHSxpQYAcow](https://stackoverflow.com/jobs/163127/remote-sr-android-java-engineer-amazon-firetv-surge?a=SHSxpQYAcow)",</code></strong>
    2. <strong><code>title: "REMOTE Sr. Android Java Engineer, Amazon FireTV App Experience REQUIRED",</code></strong>
    3. <strong><code>description: "<p>Surge Forward is looking for a smart self-motivated experienced senior-level remote developer to work as a long-term independent contractor.< p><br><p>Experience Required: < p><br><p>- Required skills: Android Java developer experience developing and deploying an Android App fro Amazon Fire TV<br>- Project: This is for a Custom Android App for Amazon Fire TV< p><br><p><strong>Must be located in the US or Canada to be considered for this role. Sorry No Visas.< strong>< p><br><p>For immediate consideration email r<em>esume with tech stack under each job and include what versions of Angular you have coded in< em> (directly on the resume) as well as cell phone number and start date.< p>",</code></strong>
    4. <strong><code>company: "Surge",</code></strong>
    5. <strong><code>created_at: "2019-04-08T02:31:06.030Z",</code></strong>
    6. <strong><code>updated_at: "2019-04-08T02:31:06.030Z",</code></strong>
    7. <strong><code>tag_list: </code></strong>
    8. <code>[</code>
        1. <code>"angular",</code>
        2. <code>"java",</code>
        3. <code>"android"</code>
    9. <code>]</code>
2. <code>}</code>


### Design and Implementation

TBA


### System Features

TBA
