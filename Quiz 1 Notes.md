§ Schema: a description  
of the data contents,  
structures and other  
aspects.  
§ External schema: what  
appl. programs and users  
see.  
§ Conceptual schema:  
description of the logical  
structure of data.  
§ Physical schema: file  
structures and indexes  
being used.


§ Relational database: a set of relations (tables)  
§ Relation: consists of  
• Instance : table content, with rows and columns.  
ü #Rows = cardinality, #fields = degree / arity.  
• Schema : table structure, with name and type of  
columns.  
ü E.G. Students(sid: char(8), name: char(16), login: char(8),  
age: int, gpa: float).  
§ More formally, a relation is a set of rows (or  
tuples)  
• What does this imply for each tuple?

§ A set of fields is a key for a relation if it is both:  
1. unique: no two distinct tuples can have same values  
in all key fields, and  
2. minimal: no subset of a key is a key.  
§ A relation can have more than one key  
• Candidate key: all keys of the relation  
• Primary key: one defined by DBA  
§ Superkey: 1 st condition holds but the 2 nd may  
not  
§ E.g., sid is a key for Students. What about  
name? The set {sid, gpa} is a superkey.

§ Foreign key : Set of fields in one relation that  
`refers’ to a tuple in another relation; a FK must  
correspond to a key (primary or candidate) of the  
other relation (like a `logical pointer’).  
• E.g. sid in Enrolled is a foreign key referring to Students:  
ü Enrolled(sid: char(8), cid: char(8), grade: char(2))  
• Referential integrity is achieved if all foreign key  
constraints are enforced, i.e., no dangling references.  
• Can you name a data model w/o referential integrity?

ER Model 

The “world” is described in terms of  
• entities  
• relationships  
• attributes

