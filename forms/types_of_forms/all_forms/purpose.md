## Main form :

Main forms are the primary user interface where peoplce can view and interact with the data.

These forms provide various options like sections, tabs, sub grids, business rules, javascript, etc


## Quick Create Form :

Quick create forms in Dynamics 365 make it easy to enter data quickly. They support the same logic as regular forms, including scripts and business rules.

When creating an entity, you need to check _custom entities can be enabled to support these forms by selecting Allow Quick Create_ or _leverage quick create form if available_.


## Quick View Form :

A quick view form can be added to another form as a quick view control, allowing users to see related information without switching records. 

The quick view control is linked to a lookup field; if that field isn’t filled in, the control won’t show up. 

Do not support editing data, form scripts. Do not include header, footer, etc.


## Card Form :

Card forms in model-driven apps are designed for compact, mobile-friendly views. They show key information in a simplified format, like in the "My Active Accounts" view. Unlike other form types, card forms are added to views using the Read-only Grid control, not directly as app components