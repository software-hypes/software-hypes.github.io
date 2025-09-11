# Object-Relational Mappers

## The Promise

ORMs promised to **let developers "just think in objects" without worrying about SQL details**. 

For teams that didn’t want to write raw queries, this was liberating.

Some things were good:
- **Boilerplate Elimination**: CRUD operations became trivial, especially in frameworks like Django, Rails, Hibernate, etc.
- **Language-Integrated Queries**: Developers could use their language (Python, Java, Ruby, etc.) without context-switching to SQL.


## The Reality

- Performance Overhead: ORMs sometimes generate very inefficient SQL (N+1 queries, unnecessary joins, giant selects).

- Leaky Abstractions: Complex queries don’t map neatly onto objects. Developers eventually had to learn SQL anyway.

- Loss of Control: Optimizing database interactions often required “dropping down” to raw SQL — defeating the purpose of the abstraction.

- Schema Mismatch: The “object world” and “relational world” are fundamentally different (the object-relational impedance mismatch).

