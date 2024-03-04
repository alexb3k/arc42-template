# Building Block View

**Content**

The building block view shows the static decomposition of the system
into building blocks (modules, components, subsystems, classes,
interfaces, packages, libraries, frameworks, layers, partitions, tiers,
functions, macros, operations, data structures, …) as well as their
dependencies (relationships, associations, …)

This view is mandatory for every architecture documentation. In analogy
to a house this is the *floor plan*.

**Motivation**

Maintain an overview of your source code by making its structure
understandable through abstraction.

This allows you to communicate with your stakeholder on an abstract
level without disclosing implementation details.

**Form**

The building block view is a hierarchical collection of black boxes and
white boxes (see figure below) and their descriptions.

![Hierarchy of building blocks](images/05_building_blocks-EN.png)

**Level 1** is the white box description of the overall system together
with black box descriptions of all contained building blocks.

**Level 2** zooms into some building blocks of level 1. Thus it contains
the white box description of selected building blocks of level 1,
together with black box descriptions of their internal building blocks.

**Level 3** zooms into selected building blocks of level 2, and so on.

See [Building Block View](https://docs.arc42.org/section-5/) in the
arc42 documentation.

## Whitebox Overall System

Here you describe the decomposition of the overall system using the
following white box template. It contains

-   an overview diagram

-   a motivation for the decomposition

-   black box descriptions of the contained building blocks. For these
    we offer you alternatives:

    -   use *one* table for a short and pragmatic overview of all
        contained building blocks and their interfaces

    -   use a list of black box descriptions of the building blocks
        according to the black box template (see below). Depending on
        your choice of tool this list could be sub-chapters (in text
        files), sub-pages (in a Wiki) or nested elements (in a modeling
        tool).

-   (optional:) important interfaces, that are not explained in the
    black box templates of a building block, but are very important for
    understanding the white box. Since there are so many ways to specify
    interfaces why do not provide a specific template for them. In the
    worst case you have to specify and describe syntax, semantics,
    protocols, error handling, restrictions, versions, qualities,
    necessary compatibilities and many things more. In the best case you
    will get away with examples or simple signatures.

***&lt;Overview Diagram>***

Motivation  
*&lt;text explanation>*

Contained Building Blocks  
*&lt;Description of contained building block (black boxes)>*

Important Interfaces  
*&lt;Description of important interfaces>*

Insert your explanations of black boxes from level 1:

If you use tabular form you will only describe your black boxes with
name and responsibility according to the following schema:

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 66%" />
</colgroup>
<thead>
<tr class="header">
<th style="text-align: left;"><strong>Name</strong></th>
<th style="text-align: left;"><strong>Responsibility</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="text-align: left;"><p><em>&lt;black box 1&gt;</em></p></td>
<td style="text-align: left;"><p> <em>&lt;Text&gt;</em></p></td>
</tr>
<tr class="even">
<td style="text-align: left;"><p><em>&lt;black box 2&gt;</em></p></td>
<td style="text-align: left;"><p> <em>&lt;Text&gt;</em></p></td>
</tr>
</tbody>
</table>

If you use a list of black box descriptions then you fill in a separate
black box template for every important building block . Its headline is
the name of the black box.

### &lt;Name black box 1>

Here you describe &lt;black box 1> according the the following black box
template:

-   Purpose/Responsibility

-   Interface(s), when they are not extracted as separate paragraphs.
    This interfaces may include qualities and performance
    characteristics.

-   (Optional) Quality-/Performance characteristics of the black box,
    e.g.availability, run time behavior, ….

-   (Optional) directory/file location

-   (Optional) Fulfilled requirements (if you need traceability to
    requirements).

-   (Optional) Open issues/problems/risks

*&lt;Purpose/Responsibility>*

*&lt;Interface(s)>*

*&lt;(Optional) Quality/Performance Characteristics>*

*&lt;(Optional) Directory/File Location>*

*&lt;(Optional) Fulfilled Requirements>*

*&lt;(optional) Open Issues/Problems/Risks>*

### &lt;Name black box 2>

*&lt;black box template>*

### &lt;Name black box n>

*&lt;black box template>*

### &lt;Name interface 1>

…

### &lt;Name interface m>

## Level 2

Here you can specify the inner structure of (some) building blocks from
level 1 as white boxes.

You have to decide which building blocks of your system are important
enough to justify such a detailed description. Please prefer relevance
over completeness. Specify important, surprising, risky, complex or
volatile building blocks. Leave out normal, simple, boring or
standardized parts of your system

### White Box *&lt;building block 1>*

…describes the internal structure of *building block 1*.

*&lt;white box template>*

### White Box *&lt;building block 2>*

*&lt;white box template>*

…

### White Box *&lt;building block m>*

*&lt;white box template>*

## Level 3

Here you can specify the inner structure of (some) building blocks from
level 2 as white boxes.

When you need more detailed levels of your architecture please copy this
part of arc42 for additional levels.

### White Box &lt;\_building block x.1\_&gt;

Specifies the internal structure of *building block x.1*.

*&lt;white box template>*

### White Box &lt;\_building block x.2\_&gt;

*&lt;white box template>*

### White Box &lt;\_building block y.1\_&gt;

*&lt;white box template>*
