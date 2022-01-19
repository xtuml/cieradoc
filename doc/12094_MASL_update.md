## MASL Jay Project update (1/19/21)

### 6 Remaining work required

#### 6.1 Translation Support (needed to start beta testing)

##### 6.1.1 Structural

- Polymorphic events (#12257)
- Assigner state machines
- Port messages with return types
- Type system
  - Named UDTs
  - Constraints
  - Array types
- Deferred operations
- Complex default values (expressions)

##### 6.1.2 Statements

- For statements (with range flavors)
- Erase statements (specific to dictionary types)

##### 6.1.3 Expressions

- Range expression
- Logical XOR
- Additional binary operators (not_in, concat, etc.)
- Additional unary operators (abs, etc.)
- Implicit unlink expressions
- Link expression (what is the type??)
- Where clauses
- Ordered selections
- Correlated nav
- Create with ID values
- Create unique
- Find only expressions (check uniqueness?)
- Structured type member access
- Array value access
- Remaining characteristics (including "class based" characteristics)
- Special literals (based numerics, ect.)
- Slice expression
- enumerator reference

#### 6.2 New architectural features

- Integrity checks (#12175)
- Support MASL C++ helper domains (#12186)
- Support MASL projects/independent domain compilation (#12104, #12106)
- Persistence (#12185)

#### 6.3 Testing

- Domain test
  - Calculator ALU domain
- Full system test
  - Multi-domain calculator model
- Unit testing
  - Test every statement type
  - Test every expression type
  - Test manipulating variables of every data type

Unit test strategy:

- Write abstract unit test class which compiles and executes a MASL example
- Use grammar and MASL language spec as a guide
- Write example model with action language to exercise construct
- Package each example into a unit test

#### 6.4 Additional tasks

- Code clean up, naming, packaging
- Document roadmap items
- User guide
- MASL release document/questions

#### 6.5 Schedule

- 6.1 done: 2/1
- 6.2 done: 3/1
- 6.3 done: 3/31
- 6.4 done: 3/31

### 7 Comments

- 6.1 is needed to release 3.0.0-beta
- 6.3 can begin right after 6.1
- 6.2, 6.4 can happen in conjunction with 6.3

- Testing is an area where outside help can really be leveraged
