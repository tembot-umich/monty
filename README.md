# Queues, Stacks, and Heaps in C Programming

The Monty Project is an open-source project aimed at implementing data structures like queues, stacks, and heaps in C programming language. It provides a solid foundation for beginners to learn about these essential data structures.

# Data Structure
/**
 * struct stack_s - doubly linked list representation of a stack (or queue)
 * @n: integer
 * @prev: points to the previous element of the stack (or queue)
 * @next: points to the next element of the stack (or queue)
 *
 * Description: doubly linked list node structure
 * for stack, queues, LIFO, FIFO
 */
typedef struct stack_s
{
        int n;
        struct stack_s *prev;
        struct stack_s *next;
} stack_t;
/**
 * struct instruction_s - opcode and its function
 * @opcode: the opcode
 * @f: function to handle the opcode
 *
 * Description: opcode and its function
 * for stack, queues, LIFO, FIFO
 */
typedef struct instruction_s
{
        char *opcode;
        void (*f)(stack_t **stack, unsigned int line_number);
} instruction_t

The project is maintained by Humphrey Agesa and Bradley Gabriel on GitHub. You can access the source code and contribute to the project through the official repository: [https://github.com/agesage/monty](https://github.com/agesage/monty)