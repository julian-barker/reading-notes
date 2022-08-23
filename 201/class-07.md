[Home](../README.md)

## Class 07

### Domain Modeling

- Domain modeling is creating a conceptual model in code that describes a problems properties such as entities, constraints, and behaviors
- A good model can help provide shared understanding between stakeholders by providing a common language

### HTML Tables

- As a best practice, tables should not be used to layout pages, because they are rigid and inflexible. They should only be used to present tabular data. In the past, some used to lay out pages with tables to to inadequate browser support for CSS
  - Negative side effects of improperly using tables are excessive tags, inaccessibility for people using screen readers, and lack of responsiveness
- The three main semantic tags within a table are:
  - `tr` - table row: contains elements that make up a row
  - `th` - stores elements within a heading row
  - `td` - stores elements within a main/normal row

### Objects

- A constructor is a function that creates an object, to avoid writing the same code over and over again to create additional instances of an object
- `this` seems to function more or less the same in constructors and object literals - ask Jacob tomorrow

### Prototypes

- Prototypes are basically models off which we can create objects, or instances of that prototype. They can nest in a hierarchy of other prototypes and inherit properties of higher prototypes.
- For example, you could have a Soldier protoype that has built in propoerties of age, MOS, and ID number. It might have methods for performing basic battle drills. You could then have a Mechanic prototype that inherits the properties of Soldier (it can perform all the same basic battle drills), but also has additional properties of unique skill identifiers and methods for doing mechanic tasks.
