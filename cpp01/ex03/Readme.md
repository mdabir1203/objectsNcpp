| Pointer | Reference |
|---------:|-----------:|
| A pointer is a variable that holds the memory address of another variable. For example: `int x = 10; int *p = &x; // p holds the address of x` | A reference is an alias, that is, another name for an already existing variable. For example: `int x = 10; int &r = x; // r is an alias for x` |
| A pointer needs to be dereferenced with the * operator to access the memory location it points to. For example: `int x = 10; int *p = &x; cout << *p << endl; // prints 10` | A reference can be used directly without any operator. For example: `int x = 10; int &r = x; cout << r << endl; // prints 10` |
| A pointer can be initialized in multiple steps or at once. For example: `int x = 10; int *p; p = &x; // OR int *p = &x;` | A reference must be initialized at once. For example: `int x = 10; int &r = x; // OR int &r; r = x; // This is incorrect` |
| A pointer can be re-assigned to point to another variable. For example: `int x = 10; int y = 20; int *p = &x; p = &y; // p now points to y` | A reference cannot be re-assigned and must always refer to the same variable. For example: `int x = 10; int y = 20; int &r = x; r = y; // This does not re-assign r, but assigns y to x` |
| A pointer has its own memory address and size on the stack. For example: `int x = 10; int *p = &x; cout << p << endl; // prints the address of x cout << &p << endl; // prints the address of p cout << sizeof(p) << endl; // prints the size of p` | A reference shares the same memory address with the original variable but also takes up some space on the stack. For example: `int x = 10; int &r = x; cout << &r << endl; // prints the address of x cout << sizeof(r) << endl; // prints the size of r` |
| A pointer can be assigned NULL directly. For example: `int *p = NULL; // p points to nothing` | A reference cannot be assigned NULL. For example: `int &r = NULL; // This is incorrect` |
| You can have a pointer to pointer offering extra levels of indirection. For example: `int x = 10; int *p = &x; int **q = &p; cout << **q << endl; // prints 10` | You can only have one level of indirection with references. For example: `int x = 10; int &r = x; int &&s = r; // This is incorrect` |


/** Usage of base class-> ->
    * Polymorphism and inheritance
    * Common Interface
    * Code Organization and maintainability
    * Abstraction and Encapsulation
    * Polymorphic Functionality
    * Flexibility and Extensibility
    * Code modularity
   Here I use abstract base class ->
        Compile-Time Error detection
        Dependency Inversion
        Design Flexibility
        Enforcing Contacts
 */
