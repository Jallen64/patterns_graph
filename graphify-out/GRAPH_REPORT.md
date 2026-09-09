# Graph Report - patterns_graph  (2026-09-08)

## Corpus Check
- Corpus is ~0 words - fits in a single context window. You may not need a graph.

## Summary
- 40 nodes · 41 edges · 8 communities (6 shown, 2 thin omitted)
- Extraction: 95% EXTRACTED · 5% INFERRED · 0% AMBIGUOUS · INFERRED: 2 edges (avg confidence: 0.85)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Structural Design Patterns
- Design Pattern Foundations
- Creational Design Patterns
- Behavioral Coordination Patterns
- Visitor Dispatch and Traversal
- Composition and Substitution Patterns
- Dependency Inversion Principle
- Interface Segregation Principle

## God Nodes (most connected - your core abstractions)
1. `Behavioral Design Patterns` - 10 edges
2. `Structural Design Patterns` - 7 edges
3. `Visitor` - 7 edges
4. `Creational Design Patterns` - 5 edges
5. `Template Method` - 5 edges
6. `Dive Into Design Patterns` - 4 edges
7. `Design Pattern` - 4 edges
8. `Favor Composition Over Inheritance` - 3 edges
9. `Strategy` - 3 edges
10. `Factory Method` - 2 edges

## Surprising Connections (you probably didn't know these)
- `Favor Composition Over Inheritance` --rationale_for--> `Design Pattern`  [EXTRACTED]
  design_patterns.pdf → design_patterns.pdf  _Bridges community 1 → community 5_
- `Command` --conceptually_related_to--> `Behavioral Design Patterns`  [EXTRACTED]
  design_patterns.pdf → design_patterns.pdf  _Bridges community 3 → community 4_
- `Strategy` --conceptually_related_to--> `Behavioral Design Patterns`  [EXTRACTED]
  design_patterns.pdf → design_patterns.pdf  _Bridges community 3 → community 5_
- `Factory Method` --conceptually_related_to--> `Template Method`  [EXTRACTED]
  design_patterns.pdf → design_patterns.pdf  _Bridges community 2 → community 5_
- `Visitor` --conceptually_related_to--> `Composite`  [EXTRACTED]
  design_patterns.pdf → design_patterns.pdf  _Bridges community 0 → community 4_

## Hyperedges (group relationships)
- **Creational Pattern Catalog** — design_patterns_factory_method, design_patterns_abstract_factory, design_patterns_builder, design_patterns_prototype, design_patterns_singleton [EXTRACTED 1.00]
- **Structural Pattern Catalog** — design_patterns_adapter, design_patterns_bridge, design_patterns_composite, design_patterns_decorator, design_patterns_facade, design_patterns_flyweight, design_patterns_proxy [EXTRACTED 1.00]
- **Behavioral Pattern Catalog** — design_patterns_chain_of_responsibility, design_patterns_command, design_patterns_iterator, design_patterns_mediator, design_patterns_memento, design_patterns_observer, design_patterns_state, design_patterns_strategy, design_patterns_template_method, design_patterns_visitor [EXTRACTED 1.00]

## Communities (8 total, 2 thin omitted)

### Community 0 - "Structural Design Patterns"
Cohesion: 0.25
Nodes (8): Adapter, Bridge, Composite, Decorator, Facade, Flyweight, Proxy, Structural Design Patterns

### Community 1 - "Design Pattern Foundations"
Cohesion: 0.25
Nodes (8): Design Pattern, Design Patterns: Elements of Reusable Object-Oriented Software, Dive Into Design Patterns, Encapsulate What Varies, Gang of Four, Object-Oriented Programming, Program to an Interface, Not an Implementation, Refactoring to Patterns

### Community 2 - "Creational Design Patterns"
Cohesion: 0.33
Nodes (6): Abstract Factory, Builder, Creational Design Patterns, Factory Method, Prototype, Singleton

### Community 3 - "Behavioral Coordination Patterns"
Cohesion: 0.33
Nodes (6): Behavioral Design Patterns, Chain of Responsibility, Mediator, Memento, Observer, State

### Community 4 - "Visitor Dispatch and Traversal"
Cohesion: 0.33
Nodes (6): Command, Double Dispatch, Iterator, Open/Closed Principle, Single Responsibility Principle, Visitor

### Community 5 - "Composition and Substitution Patterns"
Cohesion: 0.67
Nodes (4): Favor Composition Over Inheritance, Liskov Substitution Principle, Strategy, Template Method

## Knowledge Gaps
- **19 isolated node(s):** `Object-Oriented Programming`, `Abstract Factory`, `Builder`, `Prototype`, `Singleton` (+14 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **2 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Behavioral Design Patterns` connect `Behavioral Coordination Patterns` to `Visitor Dispatch and Traversal`, `Composition and Substitution Patterns`?**
  _High betweenness centrality (0.570) - this node is a cross-community bridge._
- **Why does `Visitor` connect `Visitor Dispatch and Traversal` to `Structural Design Patterns`, `Behavioral Coordination Patterns`?**
  _High betweenness centrality (0.423) - this node is a cross-community bridge._
- **Why does `Template Method` connect `Composition and Substitution Patterns` to `Creational Design Patterns`, `Behavioral Coordination Patterns`?**
  _High betweenness centrality (0.413) - this node is a cross-community bridge._
- **What connects `Object-Oriented Programming`, `Abstract Factory`, `Builder` to the rest of the system?**
  _19 weakly-connected nodes found - possible documentation gaps or missing edges._