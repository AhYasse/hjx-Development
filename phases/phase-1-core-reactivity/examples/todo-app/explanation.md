# Todo App Example Explanation

## Before (v0.1)
- Had to manually spread arrays
- Full re-render on any change
- No computed properties

## After (v1.0)
- Direct array mutations (push, splice, pop)
- Fine-grained updates (only changed parts re-render)
- Computed values with automatic caching
- Batched updates for multiple changes
