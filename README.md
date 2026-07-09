# Resources and Access in the Cloud - Google Cloud resource hierarchy | Google Skills for Partners

---

## Metadata

- **URL:** https://partner.skills.google/paths/20/course_sessions/39706059/video/630069
- **Lesson type:** `video`
- **Path ID:** `20`
- **Container type:** `course_sessions`
- **Container ID:** `39706059`
- **Lesson ID:** `630069`
- **Generated:** 2026-07-09 17:48:35

---

## Screenshot

![Full Page Screenshot](screenshot.png)

---

## Page Text

Partner
4
navigate_next
Professional Cloud DevOps Engineer Certification
navigate_next
Google Cloud Fundamentals: Core Infrastructure
navigate_next
Google Cloud resource hierarchy
Previous
Next
Recertify in 3 simple steps:
Link your Google Skills and certification account profiles using the same email to get started.
Instantly see which certifications are eligible for renewal.
Complete courses and skill badges to renew your certifications automatically.

By clicking "Accept", I consent to share my name, email, and course completion data with Google Skills' certification partner, CM Connect, to receive continuing education credit for certification renewal.

---

## Images

### Image 1

![Google Skills for Partners](https://cdn.qwiklabs.com/lqJbxogu4tSLez1OvjDcIO8rwow6cPLwvrfIdmQLf6U%3D)

Source: https://cdn.qwiklabs.com/lqJbxogu4tSLez1OvjDcIO8rwow6cPLwvrfIdmQLf6U%3D

### Image 2

![Current streak count](https://cdn.qwiklabs.com/assets/gamification/streak_icon-21476b37c13f49828a5aaa2d86c4d3378cca4117.svg)

Source: https://cdn.qwiklabs.com/assets/gamification/streak_icon-21476b37c13f49828a5aaa2d86c4d3378cca4117.svg

---

## YouTube Video

**Video ID:** `ecVv1L_TEo8`

[Open YouTube Video](https://www.youtube.com/watch?v=ecVv1L_TEo8)

<iframe width="560" height="315" src="https://www.youtube.com/embed/ecVv1L_TEo8" title="YouTube video player" frameborder="0" allowfullscreen></iframe>

---

## Transcript

### 00:00

In this section of the course we’ll look at the functional structure of Google Cloud.

### 00:05

Google Cloud’s resource hierarchy contains four levels, and starting from the bottom up they are: resources, projects, folders, and an organization node.

### 00:17

At the first level are resources.

### 00:20

These represent virtual machines, Cloud Storage buckets, tables in BigQuery, or anything else in Google Cloud.

### 00:29

Resources are organized into projects, which sit on the second level.

### 00:34

Projects can be organized into folders, or even subfolders.

### 00:37

These sit at the third level.

### 00:40

And then at the top level is an organization node, which encompasses all the projects, folders, and resources in your organization.

### 00:47

It’s important to understand this resource hierarchy because it directly relates to how policies are managed and applied when you use Google Cloud.

### 00:57

Policies can be defined at the project, folder, and organization node levels.

### 01:02

Some Google Cloud services allow policies to be applied to individual resources, too.

### 01:09

Policies are also inherited downward.

### 01:11

This means that if you apply a policy to a folder, it will also apply to all of the projects within that folder.

### 01:17

Let’s take a look at the second level of the resource hierarchy, projects, in a little more detail.

### 01:24

Projects are the basis for enabling and using Google Cloud services, like managing APIs, enabling billing, adding and removing collaborators, and enabling other Google services.

### 01:36

Each project is a separate entity under the organization node, and each resource belongs to exactly one project.

### 01:44

Projects can have different owners and users because they’re billed and managed separately.

### 01:49

Each Google Cloud project has three identifying attributes: a project ID, a project name, and a project number.

### 01:57

The project ID is a globally unique identifier assigned by Google that can’t be changed after creation.

### 02:04

They’re what we refer to as being immutable.

### 02:08

Project IDs are used in different contexts to inform Google Cloud of the exact project to work with.

### 02:15

Project names, however, are user-created.

### 02:17

They don’t have to be unique and they can be changed at any time, so they are not immutable.

### 02:23

Google Cloud also assigns each project a unique project number.

### 02:27

It’s helpful to know that these Google-generated numbers exist, but we won’t explore them much in this course.

### 02:32

They’re mainly used internally by Google Cloud to keep track of resources.

### 02:38

Google Cloud’s Resource Manager tool is designed to programmatically help you manage projects.

### 02:43

It’s an API that can gather a list of all the projects associated with an account, create new projects, update existing projects, and delete projects.

### 02:53

It can even recover projects that were previously deleted,and can be accessed through the RPC API and the REST API.

### 03:02

The third level of the Google Cloud resource hierarchy is folders.

### 03:06

Folders let you assign policies to resources at a level of granularity you choose.

### 03:11

The resources in a folder inherit policies and permissions assigned to that folder.

### 03:16

A folder can contain projects, other folders, or a combination of both.

### 03:22

You can use folders to group projects under an organization in a hierarchy.

### 03:26

For example, your organization might contain multiple departments, each with its own set Google Cloud resources.

### 03:33

Folders allow you to group these resources on a per-department basis.

### 03:38

Folders also give teams the ability to delegate administrative rights so that they can work independently.

### 03:44

As previously mentioned, the resources in a folder inherit policies and permissions from that folder.

### 03:51

For example, if you have two different projects that are administered by the same team, you can put policies into a common folder so they have the same permissions.

### 04:01

Doing it the other way--putting duplicate copies of those policies on both projects–could be tedious and error-prone.

### 04:08

if you needed to change permissions on both resources, you would now have to do that in two places instead of just one.

### 04:15

To use folders, you must have an organization node, which is the very topmost resource in the Google Cloud hierarchy.

### 04:21

Everything else attached to that account goes under this node, which includes folders, projects, and other resources.

### 04:30

There are some special roles associated with this top-level organization node.

### 04:34

For example, you can designate an organization policy administrator so that only people with privilege can change policies.

### 04:43

You can also assign a project creator role, which is a great way to control who can create projects and, therefore, who can spend money.

### 04:51

How a new organization node is created depends on whether your company is also a Google Workspace customer.

### 04:56

If you have a Workspace domain, Google Cloud projects will automatically belong to your organization node.

### 05:03

Otherwise, you can use Cloud Identity, Google’s identity, access, application, and endpoint management platform, to generate one.

### 05:11

Once created, a new organization node will let anyone in the domain create projects and billing accounts, just as they could before.

### 05:20

folders underneath it and put projects into it.

### 05:23

Both folders and projects are considered to be “children” of the organization node.

### 00:00

In this section of the course we’ll look at the functional structure of Google Cloud. 00:05 Google Cloud’s resource hierarchy contains four levels, and starting from the bottom up they are: resources, projects, folders, and an organization node. 00:17 At the first level are resources. 00:20 These represent virtual machines, Cloud Storage buckets, tables in BigQuery, or anything else in Google Cloud. 00:29 Resources are organized into projects, which sit on the second level. 00:34 Projects can be organized into folders, or even subfolders. 00:37 These sit at the third level. 00:40 And then at the top level is an organization node, which encompasses all the projects, folders, and resources in your organization. 00:47 It’s important to understand this resource hierarchy because it directly relates to how policies are managed and applied when you use Google Cloud. 00:57 Policies can be defined at the project, folder, and organization node levels. 01:02 Some Google Cloud services allow policies to be applied to individual resources, too. 01:09 Policies are also inherited downward. 01:11 This means that if you apply a policy to a folder, it will also apply to all of the projects within that folder. 01:17 Let’s take a look at the second level of the resource hierarchy, projects, in a little more detail. 01:24 Projects are the basis for enabling and using Google Cloud services, like managing APIs, enabling billing, adding and removing collaborators, and enabling other Google services. 01:36 Each project is a separate entity under the organization node, and each resource belongs to exactly one project. 01:44 Projects can have different owners and users because they’re billed and managed separately. 01:49 Each Google Cloud project has three identifying attributes: a project ID, a project name, and a project number. 01:57 The project ID is a globally unique identifier assigned by Google that can’t be changed after creation. 02:04 They’re what we refer to as being immutable. 02:08 Project IDs are used in different contexts to inform Google Cloud of the exact project to work with. 02:15 Project names, however, are user-created. 02:17 They don’t have to be unique and they can be changed at any time, so they are not immutable. 02:23 Google Cloud also assigns each project a unique project number. 02:27 It’s helpful to know that these Google-generated numbers exist, but we won’t explore them much in this course. 02:32 They’re mainly used internally by Google Cloud to keep track of resources. 02:38 Google Cloud’s Resource Manager tool is designed to programmatically help you manage projects. 02:43 It’s an API that can gather a list of all the projects associated with an account, create new projects, update existing projects, and delete projects. 02:53 It can even recover projects that were previously deleted,and can be accessed through the RPC API and the REST API. 03:02 The third level of the Google Cloud resource hierarchy is folders. 03:06 Folders let you assign policies to resources at a level of granularity you choose. 03:11 The resources in a folder inherit policies and permissions assigned to that folder. 03:16 A folder can contain projects, other folders, or a combination of both. 03:22 You can use folders to group projects under an organization in a hierarchy. 03:26 For example, your organization might contain multiple departments, each with its own set Google Cloud resources. 03:33 Folders allow you to group these resources on a per-department basis. 03:38 Folders also give teams the ability to delegate administrative rights so that they can work independently. 03:44 As previously mentioned, the resources in a folder inherit policies and permissions from that folder. 03:51 For example, if you have two different projects that are administered by the same team, you can put policies into a common folder so they have the same permissions. 04:01 Doing it the other way--putting duplicate copies of those policies on both projects–could be tedious and error-prone. 04:08 if you needed to change permissions on both resources, you would now have to do that in two places instead of just one. 04:15 To use folders, you must have an organization node, which is the very topmost resource in the Google Cloud hierarchy. 04:21 Everything else attached to that account goes under this node, which includes folders, projects, and other resources. 04:30 There are some special roles associated with this top-level organization node. 04:34 For example, you can designate an organization policy administrator so that only people with privilege can change policies. 04:43 You can also assign a project creator role, which is a great way to control who can create projects and, therefore, who can spend money. 04:51 How a new organization node is created depends on whether your company is also a Google Workspace customer. 04:56 If you have a Workspace domain, Google Cloud projects will automatically belong to your organization node. 05:03 Otherwise, you can use Cloud Identity, Google’s identity, access, application, and endpoint management platform, to generate one. 05:11 Once created, a new organization node will let anyone in the domain create projects and billing accounts, just as they could before. 05:20 folders underneath it and put projects into it. 05:23 Both folders and projects are considered to be “children” of the organization node.

---

## Main Resources

### youtube

- [Youtube](https://www.youtube.com/@googlecloud)

### videos

- [Resource](https://reportingwidget.google.com/widget/54?cid=1&url=https://partner.skills.google/paths/20/course_templates/60/video/630069?)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=ar)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=de)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=en)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=es)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=fr)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=fr_CA)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=he)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=id)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=it)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=ja)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=ko)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=pl)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=pt_BR)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=pt_PT)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=ru)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=tr)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=uk)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=zh)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/video/630069?locale=zh_TW)
- [Course Introduction](https://partner.skills.google/paths/20/course_sessions/39706059/video/630060)
- [Cloud computing overview](https://partner.skills.google/paths/20/course_sessions/39706059/video/630061)
- [IaaS and PaaS](https://partner.skills.google/paths/20/course_sessions/39706059/video/630062)
- [The Google Cloud network](https://partner.skills.google/paths/20/course_sessions/39706059/video/630063)
- [Environmental impact](https://partner.skills.google/paths/20/course_sessions/39706059/video/630064)
- [Security](https://partner.skills.google/paths/20/course_sessions/39706059/video/630065)
- [Open source ecosystems](https://partner.skills.google/paths/20/course_sessions/39706059/video/630066)
- [Pricing and billing](https://partner.skills.google/paths/20/course_sessions/39706059/video/630067)
- [Google Cloud resource hierarchy](https://partner.skills.google/paths/20/course_sessions/39706059/video/630069)
- [Identity and Access Management (IAM)](https://partner.skills.google/paths/20/course_sessions/39706059/video/630070)
- [Service accounts](https://partner.skills.google/paths/20/course_sessions/39706059/video/630071)
- [Cloud Identity](https://partner.skills.google/paths/20/course_sessions/39706059/video/630072)
- [Interacting with Google Cloud](https://partner.skills.google/paths/20/course_sessions/39706059/video/630073)
- [Virtual Private Cloud networking](https://partner.skills.google/paths/20/course_sessions/39706059/video/630076)
- [Compute Engine](https://partner.skills.google/paths/20/course_sessions/39706059/video/630077)
- [Scaling virtual machines](https://partner.skills.google/paths/20/course_sessions/39706059/video/630078)
- [Important VPC compatibilities](https://partner.skills.google/paths/20/course_sessions/39706059/video/630079)
- [Cloud Load Balancing](https://partner.skills.google/paths/20/course_sessions/39706059/video/630080)
- [Cloud DNS and Cloud CDN](https://partner.skills.google/paths/20/course_sessions/39706059/video/630081)
- [Connecting networks to Google VPC](https://partner.skills.google/paths/20/course_sessions/39706059/video/630082)
- [Google Cloud storage options](https://partner.skills.google/paths/20/course_sessions/39706059/video/630085)
- [Cloud Storage](https://partner.skills.google/paths/20/course_sessions/39706059/video/630086)
- [Cloud Storage: Storage classes and data transfer](https://partner.skills.google/paths/20/course_sessions/39706059/video/630087)
- [Cloud SQL](https://partner.skills.google/paths/20/course_sessions/39706059/video/630088)
- [Spanner](https://partner.skills.google/paths/20/course_sessions/39706059/video/630089)
- [Firestore](https://partner.skills.google/paths/20/course_sessions/39706059/video/630090)
- [Bigtable](https://partner.skills.google/paths/20/course_sessions/39706059/video/630091)
- [Comparing storage options](https://partner.skills.google/paths/20/course_sessions/39706059/video/630092)
- [Introduction to containers](https://partner.skills.google/paths/20/course_sessions/39706059/video/630095)
- [Kubernetes](https://partner.skills.google/paths/20/course_sessions/39706059/video/630096)
- [Google Kubernetes Engine](https://partner.skills.google/paths/20/course_sessions/39706059/video/630097)
- [Cloud Run](https://partner.skills.google/paths/20/course_sessions/39706059/video/630099)
- [Development in the cloud](https://partner.skills.google/paths/20/course_sessions/39706059/video/630100)
- [Prompt Engineering](https://partner.skills.google/paths/20/course_sessions/39706059/video/630103)
- [Course summary](https://partner.skills.google/paths/20/course_sessions/39706059/video/630105)
- [Resource](https://partner.skills.google/paths/20/course_sessions/39706059/video/630070)

### labs

- [Resource](https://support.google.com/qwiklabs/contact/Google_Skills_Partner)
- [Google Cloud Fundamentals: Getting Started with Cloud Marketplace](https://partner.skills.google/paths/20/course_sessions/39706059/labs/630074)
- [Get Started with Virtual Private Cloud Networking and Compute Engine](https://partner.skills.google/paths/20/course_sessions/39706059/labs/630083)
- [Google Cloud Fundamentals: Getting Started with Cloud Storage and Cloud SQL](https://partner.skills.google/paths/20/course_sessions/39706059/labs/630093)
- [Hello Cloud Run](https://partner.skills.google/paths/20/course_sessions/39706059/labs/630101)

### external_links

- [Resource](https://partner.skills.google/)
- [Professional Cloud DevOps Engineer Certification](https://partner.skills.google/paths/20)
- [Google Cloud Fundamentals: Core Infrastructure](https://partner.skills.google/paths/20/course_templates/60)
- [Dashboard](https://partner.skills.google/)
- [Catalog](https://partner.skills.google/catalog)
- [Paths](https://partner.skills.google/paths)
- [Subscriptions](https://partner.skills.google/subscriptions)
- [Activities](https://partner.skills.google/profile/stay_on_track)
- [Achievements](https://partner.skills.google/profile/badges)
- [Resource](https://reportingwidget.google.com/widget/54?cid=1&url=https%3A%2F%2Fpartner.skills.google%2Fpaths%2F20%2Fcourse_templates%2F60%2Fvideo%2F630069%3F)
- [Resource](https://partner.skills.google/profile/activity)
- [Resource](https://partner.skills.google/my_account/profile)
- [Programs](https://partner.skills.google/my_account/programs)
- [Overview](https://partner.skills.google/paths/20/course_templates/60)
- [Quiz](https://partner.skills.google/paths/20/course_sessions/39706059/quizzes/630068)
- [Quiz](https://partner.skills.google/paths/20/course_sessions/39706059/quizzes/630075)
- [Quiz](https://partner.skills.google/paths/20/course_sessions/39706059/quizzes/630084)
- [Quiz](https://partner.skills.google/paths/20/course_sessions/39706059/quizzes/630094)
- [Quiz](https://partner.skills.google/paths/20/course_sessions/39706059/quizzes/630098)
- [Quiz](https://partner.skills.google/paths/20/course_sessions/39706059/quizzes/630102)
- [Quiz](https://partner.skills.google/paths/20/course_sessions/39706059/quizzes/630104)
- [Course resources](https://partner.skills.google/paths/20/course_sessions/39706059/documents/630106)
- [Claim credential](https://partner.skills.google/paths/20/course_templates/60/badge)
- [Course Survey
      Recommended](https://partner.skills.google/paths/20/course_templates/60/course_surveys/0)
- [Resource](https://partner.skills.google/paths/20/course_sessions/39706059/quizzes/630068)
- [Resource](https://partner.skills.google/paths/20/course_templates/60/preview)

---

## Embedded Frames / HTML Media

### Google Cloud resource hierarchy

- **Tag:** `iframe`
- **Source:** https://www.youtube.com/embed/ecVv1L_TEo8?playsinline=1&controls=2&modestbranding=1&iv_load_policy=3&rel=0&enablejsapi=1&autoplay=0&origin=https%3A%2F%2Fpartner.skills.google&widgetid=1&forigin=https%3A%2F%2Fpartner.skills.google%2Fpaths%2F20%2Fcourse_templates%2F60%2Fvideo%2F630069&aoriginsup=1&vf=1

---

## Headings

- **H3**: Transcript
- **H2**: Recertify in 3 simple steps:
- **H1**: A newer version of this course is available. Your progress will carry over if you choose to upgrade. However, your completion percentage may change if the new version has added or removed any learning activities. Click the preview button to see the course changes before upgrading.
---

## Code Blocks / Commands

_No code blocks found._
---

## Tables

_No tables found._
---

## Useful Buttons

- search
---

## Plugin Extra Data

```json
{
  "content_kind": "video"
}
```


---

## Raw Files

- [page.html](page.html)
- [page_text.txt](page_text.txt)
- [session.json](session.json)
- [headings.json](headings.json)
- [links.json](links.json)
- [images.json](images.json)
- [resources.json](resources.json)
- [youtube_links.json](youtube_links.json)
- [transcript.json](transcript.json)
- [transcript.txt](transcript.txt)
- [plugin_extra.json](plugin_extra.json)
- [screenshot.png](screenshot.png)
