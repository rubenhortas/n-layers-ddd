Domain layer

All the logic of the domain, domain entities, etc.
It's good to have a specific assembly/project for entities.

At a general level, we can have a "Core" project of base classes and other horizontally reusable classes in all functional modules of the Domain.

For each functional MODULE of the application (in the example, in this case the called "MainModule"), we will implement all the logic of the module (Services, Specifications and Contracts of Repositories).

We need an isolated project for the "Entities of the Domain" where Entity-Framework generates our POCO/Self-entity tracking classes.

Each project with logical classes will have a Testing class project (Unit Tests) and we could have other integration and functional testing projects.