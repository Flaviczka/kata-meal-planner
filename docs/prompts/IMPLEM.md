# Implementation Workflow

## Objective

Guide the step-by-step implementation of features or tasks with proper planning, execution, and validation.

## Process

### 1. Analyze the Task

- Review the task requirements and acceptance criteria
- Identify dependencies on existing code, APIs, or database schema
- Consult PROJECT_BRIEF.md, ARCHITECTURE.md, and STACK.md for context

### 2. Break Down into Steps

- Split complex tasks into small, atomic sub-tasks
- Each step should be independently testable and committable
- Order steps by dependency (backend models → migrations → API → frontend)
- List all steps before starting implementation

### 3. Implement Each Step

- Implement one step at a time
- Follow coding standards and best practices from the stack (Laravel PSR, Nuxt 3 Composition API)
- Write clean, documented code with appropriate error handling
- Test the implementation locally

### 4. Commit After Each Step

- Write clear, descriptive commit messages following conventional commits format
- Example: `feat(backend): add Meal model with validation`
- Commit only working, tested code

### 5. Review and Validate

- After all steps are complete, review the full implementation
- Verify all acceptance criteria are met
- Check for code quality, security, and performance issues
- Suggest improvements if needed

## Example Flow

**Task**: Create meal CRUD API

**Steps**:

1. Create Meal migration with all fields
2. Create Meal model with relationships and validation
3. Create MealController with CRUD methods
4. Add API routes with proper middleware
5. Write API tests
6. Update API documentation

**Execution**: Implement step 1 → commit → implement step 2 → commit → etc.
