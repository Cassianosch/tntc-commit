## Commit Message Guidelines

In this document we will cover the guidelines for commit messages that must be followed by the developers.

### Summary

The guidelines listed below are based on [CM](https://www.conventionalcommits.org/en/v1.0.0/#specification), but with some tweaks to fit our needs.  These rules will help us create more descriptive commits so we can improve commit history consistency and automation.
  
    


### The commit messages should be structured as described below:
> type[module/scope(optional)]: description
>
> [body(optional)]
>
>[footer(optional)]  
  
##### Commits contain structural elements(types), so we can tell what is being changed.
1. **fix**           - Correcting an error in the code
2. **feat**          - Adding a new feature to the code
3. **refactor**      - Refactoring some part of the code, not adding a new feature or fixing a bug
3.1. **refactor!**   - Breaking change (! is for attention)
4. **revert**        -  Reversing some part of the code/commit
5. **Finish v0.0.1** - Creating a release commit
6. **style**         - CSS, formatting, missing semicolons, syntax adjustment
7. **test**          - Adding Tests
8. **perf**          - Adding or adjusting code that improves the app's performance
9. **ci**            - Deployment Process
10. **chore**        - Changing/Adding build-related tools
11. **docs**         - Updating Documentation  

#### Examples

> When adding new functionality (e.g.): **let users delete properties from listing page**

`feat[delete-properties]: Adding a way for users to delete properties from listing page` <br />
`feat: Adding a way for users to delete properties from listing page`

---

>There's a bug in the currency input, which doesn't have the currency mask, **but the input was designed to have the currency mask**.

`fix[shopping-cart]: Adding currency mask to the currency input`

---

> I thought of a way to improve the rendering time of the Properties page

`perf[properties]: list of all properties`<br />
`Improving loading time using server-side rendering`

---

> Removing support for node < 6

`refactor!: drop support for Node 6`<br />

---
> By default using [Smart Git](https://www.syntevo.com/smartgit/)
