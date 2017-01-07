## OOPS - Understanding relationships such as Association, Aggregation, Composition and Dependency 

### Relationship 
A relationship defines the connection between objects. This explains how objects are connected to each other’s and how they will behave.

### Association
It represents a relationship between two or more objects where all objects have their own lifecycle and there is no owner. The name of an association specifies the nature of relationship between objects. This is represented by a solid line.

Let’s take an example of relationship between Teacher and Student. Multiple students can associate with a single teacher and a single student can associate with multiple teachers. But there is no ownership between the objects and both have their own lifecycle. Both can be created and deleted independently.

<img alt="resource not found" src="/resources/images/association-diagram.png" />

## Aggregation
It is a specialized form of Association where all object have their own lifecycle but there is ownership. This represents “whole-part or a-part-of” relationship. This is represented by a hollow diamond followed by a line.

<img alt="aggregation image" src="/resources/images/aggregation.png" />

Let’s take an example of relationship between Department and Teacher. A Teacher may belongs to multiple departments. Hence Teacher is a part of multiple departments. But if we delete a Department, Teacher Object will not destroy.

<img alt="aggregation relationship image" src="/resources/images/aggregation-diagram.png" />

## Composition
It is a specialized form of Aggregation. It is a strong type of Aggregation. In this relationship child objects does not have their lifecycle without Parent object. If a parent object is deleted, all its child objects will also be deleted. This represents “death” relationship. This is represented by a solid diamond followed by a line.

<img alt="composition image" src="/resources/images/composition.png" />

Let’s take an example of relationship between House and rooms. House can contain multiple rooms there is no independent life of room and any room cannot belongs to two different house if we delete the house room will automatically delete.

<img alt="composition relationship image" src="/resources/images/composition-diagram.png" />

Let’s take another example of relationship between Questions and options. Single questions can have multiple options and option cannot belong to multiple questions. If we delete questions options will be automatically deleted.

